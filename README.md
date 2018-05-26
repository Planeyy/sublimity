# Sublimity

A Java Library for bespoke concurrent system integrations.

## Example usage

```java
List<Integration> integrations = new ArrayList<>();
integrations.add(new PeopleEmployee());
IntegrationRunner integrationRunner = new IntegrationRunner(integrations, new StubScheduleChecker(), new ConsoleLogger());
Timer t = new Timer();
t.scheduleAtFixedRate(integrationRunner, 0, 1000);
```

## Versioning

Current version is 0.1

## Author

* **Josh Hunt** - *Initial work* - [Josh](https://github.com/huntjosh)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details
