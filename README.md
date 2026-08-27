# Hotel Operations Platform

An AI-assisted mobile operations platform that helps hotel teams report issues, coordinate work, and learn from recurring operational patterns.

[中文项目简介](docs/README.zh-CN.md)

> Status: planning and early development. This is an experimental/student project and is not ready for production hotel operations.

## The problem

Hotel work is fast, physical, and distributed across rooms, floors, and departments. Requests can be lost in chat messages, phone calls, or paper notes. Managers may know that the same problems keep happening without having structured data to understand why.

## The vision

Give every staff member a quick way to report work—with a photo, location, and voice or text—then give managers one clear place to assign, monitor, and analyze it.

The product should eventually turn everyday operational activity into useful insight: recurring maintenance issues, workload imbalance, response-time bottlenecks, and trends by location or department.

## Who it serves

### Hotel staff

- Create a request with minimal typing
- Attach or capture a photo
- Choose a room or hotel location
- See assigned work and update its status
- Track requests they submitted

### Hotel managers

- View, search, and filter requests
- Assign work to staff or departments
- Monitor priority, ownership, and completion
- Review activity and response-time trends
- Generate summaries and reports

## MVP: the first useful version

The first version will focus on one complete workflow:

1. A staff member creates a request.
2. A manager reviews and assigns it.
3. An assignee changes it from `Open` to `In progress` to `Completed`.
4. Everyone involved can see the current status and history.

AI analytics, advanced reporting, and automation come after this workflow is reliable. See [MVP Scope](docs/MVP_SCOPE.md) and [Roadmap](docs/ROADMAP.md).

## Planned technology

| Area | Initial direction | Status |
|---|---|---|
| Mobile app | React Native with Expo | Selected |
| Backend | To be evaluated | Open decision |
| Database | To be evaluated | Open decision |
| Photo storage | To be evaluated | Open decision |
| Authentication | To be evaluated | Open decision |
| AI services | Added after useful data exists | Later phase |

## Documentation

- [Product Vision](docs/VISION.md)
- [中文项目简介](docs/README.zh-CN.md)
- [MVP Scope](docs/MVP_SCOPE.md)
- [User Flows](docs/USER_FLOWS.md)
- [Architecture](docs/ARCHITECTURE.md)
- [Roadmap](docs/ROADMAP.md)
- [Contributing](CONTRIBUTING.md)



## Project principles

- Fast enough to use during a busy shift
- Clear ownership and visible status
- Minimal typing for frontline staff
- Useful without AI; improved by AI later
- Privacy and role-based access designed from the beginning
- Small, testable releases instead of a large first launch

## License

No license has been selected yet. Until one is added, all rights are reserved by the repository owner.
