## Setup Instructions

1. **Clone the repository:**

    ```
    git clone https://github.com/kelvinbiffileote/peppol-as4.git
    cd peppol-as4
    ```

2. **Generate a Java Keystore:**

    Generate a keystore and place it inside `oxalis/config/keystore` directory.

    ```
    keytool -genkeypair -alias your-key-alias -keyalg RSA -keysize 2048 -keystore oxalis/config/keystore/oxalis.jks -storepass your-keystore-password -keypass your-key-password -validity 365
    ```

3. **Update Configuration:**

    Update `oxalis/config/oxalis.conf` with your keystore details and any other configuration settings.

4. **Build and Run the Docker Containers:**

    ```
    docker-compose up -d
    ```

5. **Access Oxalis:**

    Once the containers are running, you can access the Oxalis Access Point at `http://localhost:8080`.

6. **Testing:**

    Use the inbound and outbound directories for testing message exchanges.