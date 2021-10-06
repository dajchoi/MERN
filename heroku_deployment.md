### Heroku Setup
###### in the front-end side 
write down
npm run build
//it will then create a build section

###### in the server side 
write down 
if (process.env.NODE_ENV === 'production) {
  app.use(express.static('front-end_side\build'));
}

###### in the cmd
heroku create app_name

//then create addons
write down
heroku addons:create ormongo:5mmap
