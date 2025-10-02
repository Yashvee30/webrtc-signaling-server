FROM coturn/coturn:latest

# Copy configuration file
COPY turnserver.conf /etc/coturn/turnserver.conf

# Expose ports
EXPOSE 3478 3478/udp
EXPOSE 5349 5349/udp
EXPOSE 49152-65535/udp

# Run coturn
CMD ["turnserver", "-c", "/etc/coturn/turnserver.conf"]
