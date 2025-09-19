# Use lightweight nginx
FROM nginx:alpine

# Copy custom nginx config if you need React Router support
COPY nginx.conf /etc/nginx/conf.d/default.conf

# Copy your prebuilt React app
COPY latest/ /usr/share/nginx/html

# Expose port 8080 for Cloud Run
EXPOSE 8080
CMD ["nginx", "-g", "daemon off;"]
