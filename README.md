
# Run FR24Feeder in a container.

## Requirements:
 - FR24Feeder config file with key.

## Steps to run:
1. Create image:

    ```docker create --name fr24feeder --restart always franspaco/fr24feeder```

2. Copy your config file:

    ```docker cp fr24feed.ini fr24feeder:/etc/fr24feed.ini```

3. Start container:

    ```docker start fr24feeder```