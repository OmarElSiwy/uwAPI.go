# Waterloo OpenData API v3 Go Client Library

## Overview

Welcome to the Waterloo OpenData API v3 Go Client Library! This library provides a simple and efficient way to access the rich datasets offered by the University of Waterloo's OpenData API using the Go programming language. Tailored for developers and data enthusiasts, our library interfaces seamlessly with the OpenData API, allowing easy access to a wide range of university data, from class schedules to campus locations.

## Features

- **Comprehensive Coverage**: Fully integrates with all endpoints of the Waterloo OpenData API v3, including class schedules, exam schedules, course catalogues, food services, holiday dates, important dates, locations, subjects, terms, and WCMS site information.
- **Ease of Use**: Simplified functions for all GET requests, streamlining the process of retrieving data.
- **Swagger Documentation Integration**: Adheres to the OpenAPI Specification v3 (OAS3) for easy understanding and maintenance.
- **Secure Communication**: Utilizes the `net/http` package for secure HTTPS communication with the API.
- **Efficient and Scalable**: Optimized for performance and scalability to handle data retrieval needs of any size.

## Getting Started

To start using the Waterloo OpenData API v3 Go Client Library, ensure you have Go installed on your system. You can then include this library in your project by importing it:

```go
import "github.com/OmarElSiwy/uwAPI.go"
```

## Usage

Here's a quick example to get you started:
```
package main

import (
    "fmt"
    "github.com/OmarElSiwy/uwAPI.go"
)

apiKey  = "" // FILL THIS IN USING YOUR OWN API KEY

func main() {
    // Get class schedules for a specific term
    termCode := "1209" // Example term code
    schedules, err := waterloo-opendata-v3.GetClassSchedules(termCode)
    if err != nil {
        log.Fatalf("Error retrieving class schedules: %s", err)
    }
    fmt.Println("Class Schedules:", schedules)
}
```

## Documentation

For detailed documentation, please refer to our Swagger documentation at /swagger/v1/swagger.json. This will provide you with comprehensive details about each endpoint, the expected request format, and the response structure.

## License

This library is distributed under the MIT license. See the LICENSE file for more information.
