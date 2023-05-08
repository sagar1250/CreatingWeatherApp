# CreatingWeatherApp

##index.html - code



<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>My Weather App</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-    KK94CHFLLe+nY2dmCWGMq91rCGa5gtU4mk92HdvYe+M/SXH301p5ILy+dN9+nJOZ" crossorigin="anonymous" />
</head>

<body>
    <nav class="navbar navbar-expand-lg bg-body-tertiary">
        <div class="container-fluid">
            <a class="navbar-brand" href="#">Weather App</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
          <span id="" class="navbar-toggler-icon"></span id="">
        </button>
            <div class="collapse navbar-collapse" id="navbarSupportedContent">
                <ul class="navbar-nav me-auto mb-2 mb-lg-0">
                    <li class="nav-item">
                        <a class="nav-link active" aria-current="page" href="#">Home</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">About this App</a>
                    </li>
                    <li class="nav-item dropdown">
                        <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                Locations
              </a>
                        <ul class="dropdown-menu">
                            <li><a class="dropdown-item" href="#">Delhi</a></li>
                            <li><a class="dropdown-item" href="#">Seattle</a></li>
                            <li>
                                <hr class="dropdown-divider" />
                            </li>
                            <li>
                                <a class="dropdown-item" href="#">Bangalore</a>
                            </li>
                        </ul>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link disabled">Usage Guide</a>
                    </li>
                </ul>
                <form class="d-flex" role="search">
                    <input id="city" class="form-control me-2" type="search" placeholder="Search" aria-label="Search" />
                    <button class="btn btn-outline-success" type="submit" id="submit">
              Search
            </button>
                </form>
            </div>
        </div>
    </nav>

    <div class="container">
        <h1 class="my-4 text-center">Weather for <span id="cityName"></span></h1>
        <main>
            <div class="row row-cols-1 row-cols-md-3 mb-3 text-center">
                <div class="col">
                    <div class="card mb-4 rounded-3 shadow-sm">
                        <div class="card-header py-3">
                            <h4 class="my-0 fw-normal">Temperature</h4>
                        </div>
                        <div class="card-body">
                            <h1 class="card-title pricing-card-title">
                                <small class="text-body-secondary fw-light"><sup><span id="temp2"></span><span>&#8451;</span></sup></small>
                            </h1>
                            <ul class="list-unstyled mt-3 mb-4">
                                <li>Temperature is <span id="temp"></span></li>
                                <li>Min Temperature is <span id="min_temp"></span></li>
                                <li>Max Temperature is <span id="max_temp"></span></li>

                            </ul>
                            <button type="button" class="w-100 btn btn-lg btn-outline-primary">
                  info
                </button>
                        </div>
                    </div>
                </div>
                <div class="col">
                    <div class="card mb-4 rounded-3 shadow-sm">
                        <div class="card-header py-3">
                            <h4 class="my-0 fw-normal">Humidity Info</h4>
                        </div>
                        <div class="card-body">
                            <h1 class="card-title pricing-card-title">
                                <span id="humidity2"></span><small class="text-body-secondary fw-light">%</small>
                            </h1>
                            <ul class="list-unstyled mt-3 mb-4">
                                <li>Humidity is <span id="humidity"></span></li>
                                <li>Cloud PCT is <span id="cloud_pct"></span></li>
                                <li>Feels Like <span id="feels_like"></span></li>
                            </ul>
                            <button type="button" class="w-100 btn btn-lg btn-primary">
                  info
                </button>
                        </div>
                    </div>
                </div>
                <div class="col">
                    <div class="card mb-4 rounded-3 shadow-sm border-primary">
                        <div class="card-header py-3 text-bg-primary border-primary">
                            <h4 class="my-0 fw-normal">Wind Info</h4>
                        </div>
                        <div class="card-body">
                            <h1 class="card-title pricing-card-title">
                                <span id="wind_speed2"></span><small class="text-body-secondary fw-light">km/hr</small>
                            </h1>
                            <ul class="list-unstyled mt-3 mb-4">
                                <!-- <li>Wind Degrees is <span id="wind_degrees"></span></li> -->
                                <li>Wind speed is <span id="wind_speed"></span></li>
                                <li>Sunrise Time is <span id="sunrise"></span></li>
                                <li>Sunset Time is <span id="sunset"></span></li>
                            </ul>
                            <button type="button" class="w-100 btn btn-lg btn-primary">
                  Info
                </button>
                        </div>
                    </div>
                </div>
            </div>

            <h2 class="display-6 text-center mb-4">
                Weather of other common places
            </h2>

            <div class="table-responsive">
                <table class="table text-center">
                    <thead>
                        <tr>
                            <th style="width: 34%"></th>
                            <th style="width: 22%">cloud_pct</th>
                            <th style="width: 22%">Feels_like</th>
                            <th style="width: 22%">Humidity</th>
                            <th style="width: 22%">Max_temp</th>
                            <th style="width: 22%">Min_temp</th>
                            <th style="width: 22%">Sunrise</th>
                            <th style="width: 22%">Sunset</th>
                            <th style="width: 22%">Temp</th>
                            <th style="width: 22%">Wind_degrees</th>
                            <th style="width: 22%">Wind_speed</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr>
                            <th scope="row" class="text-start">Shanghai</th>
                            <td>1</td>
                            <td>2</td>
                            <td>3</td>
                            <td>4</td>
                            <td>5</td>
                            <td>1</td>
                            <td>2</td>
                            <td>3</td>
                            <td>4</td>
                            <td>5</td>
                            <td>
                                <svg class="bi" width="24" height="24">
                    <use xlink:href="#check"></use>
                  </svg>
                            </td>
                            <td>
                                <svg class="bi" width="24" height="24">
                    <use xlink:href="#check"></use>
                  </svg>
                            </td>
                        </tr>
                        <tr>
                            <th scope="row" class="text-start">Boston</th>
                            <td>1</td>
                            <td>2</td>
                            <td>3</td>
                            <td>4</td>
                            <td>5</td>
                            <td>1</td>
                            <td>2</td>
                            <td>3</td>
                            <td>4</td>
                            <td>5</td>
                        </tr>
                    </tbody>

                    <tbody>
                        <tr>
                            <th scope="row" class="text-start">Lucknow</th>
                            < <td>1</td>
                                <td>2</td>
                                <td>3</td>
                                <td>4</td>
                                <td>5</td>
                                <td>1</td>
                                <td>2</td>
                                <td>3</td>
                                <td>4</td>
                                <td>5</td>
                        </tr>
                        <tr>
                            <th scope="row" class="text-start">Kolkata</th>
                            < <td>1</td>
                                <td>2</td>
                                <td>3</td>
                                <td>4</td>
                                <td>5</td>
                                <td>1</td>
                                <td>2</td>
                                <td>3</td>
                                <td>4</td>
                                <td>5</td>
                        </tr>
                    </tbody>
                </table>
            </div>
        </main>
    </div>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha3/dist/js/bootstrap.bundle.min.js" integrity="sha384-ENjdO4Dr2bkBIFxQpeoTz1HIcje39Wm4jDKdf19U8gI4ddQ3GYNS7NTKfAdVQSZe" crossorigin="anonymous"></script>
    <script src="script.js"></script>
</body>

</html>






## script.js - code

const options = {
    method: 'GET',
    headers: {
        'X-RapidAPI-Key': '47f7b10910msh54245c99856fc89p1511ebjsn0be081069aa6',
        'X-RapidAPI-Host': 'weather-by-api-ninjas.p.rapidapi.com'
    }
};
const getWeather = (city) => {
    cityName.innerHTML = city
    fetch('https://weather-by-api-ninjas.p.rapidapi.com/v1/weather?city=' + city, options)
        .then(response => response.json())
        .then((response) => {
            console.log(response)
            cloud_pct.innerHTML = response.cloud_pct
            temp.innerHTML = response.temp
            temp2.innerHTML = response.temp
            feels_like.innerHTML = response.feels_like
            humidity.innerHTML = response.humidity
            humidity2.innerHTML = response.humidity
            min_temp.innerHTML = response.min_temp
            max_temp.innerHTML = response.max_temp
            wind_speed.innerHTML = response.wind_speed
            wind_speed2.innerHTML = response.wind_speed
            wind_degrees.innerHTML = response.wind_degrees
            sunrise.innerHTML = response.sunrise
            sunset.innerHTML = response.sunset

        })
        .catch(err => console.error(err));
}
submit.addEventListener("click", (e) => {
    e.preventDefault()
    getWeather(city.value)
})
getWeather("Delhi")



#Output


![WeatherOutPutPic](https://user-images.githubusercontent.com/67116952/233889262-c9149bd3-6b7c-440a-adc0-a5a82ee6e4da.png)


