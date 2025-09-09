# IATA ONE Order: Simplifying Airline Retailing and Operations

The airline industry has long relied on fragmented systems—Passenger Name Records (PNRs), e-tickets, and Electronic Miscellaneous Documents (EMDs)—to manage reservations, delivery, and accounting. While these constructs have served the industry for decades, they are rooted in paper-based processes and have created inefficiencies, complexity, and high costs across the travel value chain.

IATA’s ONE Order standard addresses this challenge by consolidating these artifacts into a single, retail-centric Order. This unified record becomes the single source of truth, integrating booking, payment, fulfillment, and accounting information. For airlines, service providers, and customers, this represents a step-change in how travel is sold, delivered, and managed.

---

## Tech Stack

- **Java 17**: Modern, robust, and secure language for enterprise applications.
- **Spring Boot 3**: Rapid application development and production-ready features for RESTful APIs and microservices.
- **JAXB (Java Architecture for XML Binding)**: Used for generating Java POJOs from IATA XSD schemas, enabling XML data binding.
- **Maven**: Build automation and dependency management.
- **Lombok**: Reduces boilerplate code in Java classes.
- **Jakarta XML Bind & Activation**: For XML serialization/deserialization and data handling.
- **JUnit**: Testing framework for unit and integration tests.

---

## Project Structure

- `src/main/java/com/ia/iata/oneorder/` — JAXB-generated POJOs and main Java code
- `src/main/resources/xsd/` — IATA XSD schema files
- `src/main/resources/bindings.xml` — JAXB custom bindings
- `pom.xml` — Maven build configuration
- `README.md` — Project documentation

---

## How to Build & Generate POJOs

1. Place your IATA XSD files in `src/main/resources/xsd/`.
2. (Optional) Adjust `bindings.xml` for custom JAXB bindings.
3. Run:
   ```sh
   mvn clean compile
   ```
   This will generate Java classes in `src/main/java/com/ia/iata/oneorder/`.

---

## Key Features

- **Unified Order Model**: All travel documents consolidated into a single order.
- **Extensible Java POJOs**: Generated from official IATA schemas, ready for integration.
- **Spring Boot Ready**: Easily build REST APIs or microservices around the unified order model.

---

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.
