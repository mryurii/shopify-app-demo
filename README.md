# README

* Ruby 2.6.3
* Rails 6.0.0.rc1
* Yarn 1.17.3
* Posgresql > 9.3
* Ngrok

Create DB container `docker run -d -p 60023:5432 --name shopify_app_demo -e POSTGRES_PASSWORD=shopify_app_demo postgres
`
Usage:
- `docker start shopify_app_demo`
- `docker stop shopify_app_demo`

Required env variables:
- SHOPIFY_API_KEY
- SHOPIFY_API_SECRET
- NGROK_HOST

Development:
- Start ngrok
- `rails db:setup`
- `rails s`
