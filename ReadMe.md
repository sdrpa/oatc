## Welcome to Open ATC

The goal of project is to build a set of open source ATC modules to be shared across other applications.
The modules are written in [Swift](https://swift.org), cross-platform compatible (Linux, OS X and iOS) providing a level of OS independence to enhance portability.

Official project website is [oatc.io](http://oatc.io)

## Core modules

- [**AircraftKit**](https://github.com/sdrpa/aircraftkit) - Aircraft performance library. Loads and parses aircraft data from XML.

- [**AirspaceKit**](https://github.com/sdrpa/airspacekit) - Contains code to load and parse airspace model from disk (boundary, navigation points, sectors, layers ...)

- [**ATCKit**](https://github.com/sdrpa/atckit) - Provides base ATC structures which are required for almost all other OATC modules.

- [**ATCSIM**](https://github.com/sdrpa/atcsim) - Simulation library. Simulates air traffic flow from a scenario.

- [**FDPS**](https://github.com/sdrpa/fdps) - Flight Data Processing System. (FDPServer, FDPClient ...)

- [**Measure**](https://github.com/sdrpa/measure) - Unit-safe numeric types. Provide compiler help to make sure that only numerics with the same unit-of-measure can be combined.

- [**Projection**](https://github.com/sdrpa/projection), [**PROJ4**](https://github.com/sdrpa/proj4) - Swift wrapper for [PROJ.4](https://github.com/OSGeo/proj.4) (Cartographic Projections Library). Makes it easy to use OATC with all commonly used projections.

### Other modules:

- [**FoundationKit**](https://github.com/sdrpa/foundationkit) - Contains various extensions to Apple's Foundation framework

- [**JSON**](https://github.com/sdrpa/json) - JSON parsing library. Extracted in order to keep other modules independent of JSON implementation. In future, [SE-0166 Swift Archival & Serialization](https://github.com/apple/swift-evolution/blob/master/proposals/0166-swift-archival-serialization.md) should probably be used.

- [**Mathematics**](https://github.com/sdrpa/mathematics), [**BlueSocket**](https://github.com/IBM-Swift/BlueSocket) (network communication) 

### Sample Applications
Sample applications using core modules to help you get started:

- [**Map Editor (OATCME)**](https://github.com/sdrpa/oatcme) - Create and edit map layers which can be read by [AircraftKit](https://github.com/sdrpa/aircraftkit)
- [**Display**](https://github.com/sdrpa/display-macos) - 2D display prototype using different modules ([AirspaceKit](https://github.com/sdrpa/airspacekit), [ATCKit](https://github.com/sdrpa/atckit), [Measure](https://github.com/sdrpa/measure), [Projection](https://github.com/sdrpa/projection)...).
- [**Simulation**](https://github.com/sdrpa/simulation-macos) - Interface to [ATCSIM](https://github.com/sdrpa/atcsim) module. It takes role of FDPS and Tracker simulating real traffic flow.

[**Data repository**](https://github.com/sdrpa/oatcdata) contains sample data (Aircraft, Airspace, Scenario) so you quickly check what format is currently suported for the particular module.

## Source and Contributions

If you would like to contribute, please create a pull request to propose and collaborate on changes to a repository.

## License

This software is licensed under [GPLv3](https://www.gnu.org/licenses/gpl.txt). For third-party libraries that are used in a module, please check Credits.md file inside the particular module.
