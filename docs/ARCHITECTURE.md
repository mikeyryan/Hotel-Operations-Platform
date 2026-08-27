# Architecture

This document records the intended shape of the system. Technology choices other than Expo remain open until the MVP requirements are clearer.

## High-level components

```text
Expo mobile app
  |-- authentication
  |-- request and task screens
  |-- camera/photo selection
  |-- notifications
  |
Backend API
  |-- authorization and business rules
  |-- request lifecycle
  |-- audit/activity history
  |
Data services
  |-- relational database
  |-- private object storage for photos
  |-- analytics/AI pipeline (later)
```

## Suggested core entities

### User

`id`, `name`, `role`, `department`, `property_id`, `active`

### Property and location

`property_id`, `location_id`, `type`, `name`, `floor`, `room_number`

### Request

`id`, `title`, `description`, `category`, `priority`, `status`, `location_id`, `reporter_id`, `assignee_id`, `created_at`, `updated_at`, `completed_at`

### Attachment

`id`, `request_id`, `storage_key`, `media_type`, `created_by`, `created_at`

### Activity event

`id`, `request_id`, `actor_id`, `event_type`, `previous_value`, `new_value`, `created_at`

## Important design constraints

- Photos should be private and served through short-lived authorized links.
- Authorization must be enforced by the backend, not only hidden in the app UI.
- Every status, priority, and assignment change should create an audit event.
- AI output should be advisory and traceable; it should not silently change operational data.
- Hotel and employee information should not be placed in source code or public test data.

## Decisions still required

Use an Architecture Decision Record in the vault for each choice:

- Backend and database platform
- Authentication provider
- Photo storage
- Notification service
- Single-property versus multi-property data model
- Analytics and AI approach

