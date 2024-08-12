# IoT Temperature Monitoring System

This project simulates an IoT device that monitors room temperature and raises an alarm if the temperature exceeds a certain threshold. The system uses the MQTT protocol to transmit data and Flask to expose an API for the latest temperature readings.

## Components

1. **Publisher Program**: Reads temperature data from the DHT11 sensor and publishes it to an MQTT broker.
2. **Subscriber Program**: Subscribes to the temperature topic, checks if the temperature exceeds a threshold for 5 minutes, and logs the data.
3. **Server Program**: Exposes the latest temperature data via an HTTP API.

## Running the Programs

1. **Publisher Program**: Run `publisher.py` to start publishing temperature data.
2. **Subscriber Program**: Run `subscriber.py` to start monitoring temperature data.
3. **Server Program**: Run `server.py` to start the HTTP server.

## Testing

- The temperature is logged locally in `temperature_log.json`.
- The API endpoint can be accessed at `http://localhost:5000/temperature`.