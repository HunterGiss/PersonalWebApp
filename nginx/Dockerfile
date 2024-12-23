FROM nginx:1.26.2

# Remove default Nginx configuration
RUN rm /etc/nginx/conf.d/default.conf

# Add custom configuration for serving the React app
COPY nginx.conf /etc/nginx/conf.d/default.conf
