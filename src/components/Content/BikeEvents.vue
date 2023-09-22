<script>
export default {
  data() {
    return {
      events: [
        {
          date: "22",
          imageSrc: "src/assets/img/event1.jpg",
          title: "New Jersey Cycling Event 2023",
          dateTime: "28-04-1994 @ 07:30",
          location: "New Jersey",
          buttonText: "Bicycle Race",
        },
        {
          date: "22",
          imageSrc: "src/assets/img/event2.jpg",
          title: "Another Cycling Event",
          dateTime: "30-04-1994 @ 08:00",
          location: "Some Other Place",
          buttonText: "Race for Fun",
        },
        {
          date: "22",
          imageSrc: "src/assets/img/event3.jpg",
          title: "New Jersey Cycling Event 2023",
          dateTime: "28-04-1994 @ 07:30",
          location: "New Jersey",
          buttonText: "Bicycle Race",
        },
        {
          date: "22",
          imageSrc: "src/assets/img/event4.jpg",
          title: "Another Cycling Event",
          dateTime: "30-04-1994 @ 08:00",
          location: "Some Other Place",
          buttonText: "Race for Fun",
        },
        {
          date: "22",
          imageSrc: "src/assets/img/event5.jpg",
          title: "New Jersey Cycling Event 2023",
          dateTime: "28-04-1994 @ 07:30",
          location: "New Jersey",
          buttonText: "Bicycle Race",
        },
        {
          date: "22",
          imageSrc: "src/assets/img/event6.jpg",
          title: "Another Cycling Event",
          dateTime: "30-04-1994 @ 08:00",
          location: "Some Other Place",
          buttonText: "Race for Fun",
        },
        {
          date: "22",
          imageSrc: "src/assets/img/event7.jpg",
          title: "New Jersey Cycling Event 2023",
          dateTime: "28-04-1994 @ 07:30",
          location: "New Jersey",
          buttonText: "Bicycle Race",
        },
        {
          date: "22",
          imageSrc: "src/assets/img/event8.jpg",
          title: "Another Cycling Event",
          dateTime: "30-04-1994 @ 08:00",
          location: "Some Other Place",
          buttonText: "Race for Fun",
        },
        {
          date: "22",
          imageSrc: "src/assets/img/event9.jpg",
          title: "New Jersey Cycling Event 2023",
          dateTime: "28-04-1994 @ 07:30",
          location: "New Jersey",
          buttonText: "Bicycle Race",
        },
        {
          date: "22",
          imageSrc: "src/assets/img/event10.jpg",
          title: "Another Cycling Event",
          dateTime: "30-04-1994 @ 08:00",
          location: "Some Other Place",
          buttonText: "Race for Fun",
        },
      ],
    };
  },
};
</script>

<template>
  <div class="container mt-4">
    <div class="text-center mb-4">
      <h1>Don't Miss Our Events!</h1>
      <h5>Get the amazing cycling experience</h5>
    </div>
    <div class="row">
      <div class="col-md-4 mb-4" v-for="(event, index) in events" :key="index">
        <div class="card">
          <div class="date-badge">
            <i class="fas fa-calendar-alt"></i>{{ event.date }}
          </div>
          <img
            :src="event.imageSrc"
            class="card-img-top"
            :alt="'Card image ' + index"
          />
          <div class="card-body">
            <h5 class="card-title">{{ event.title }}</h5>
            <ul class="event-details">
              <li><i class="fas fa-clock"></i> {{ event.dateTime }}</li>
              <li><i class="fas fa-map-marker-alt"></i>{{ event.location }}</li>
            </ul>
            <span class="custom-button">{{ event.buttonText }}</span>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.date-badge {
  position: absolute;
  top: 10px;
  left: 10px;
  background-color: white;
  color: black;
  font-weight: bold;
  padding: 5px;
}
.event-details {
  list-style: none;
  padding: 0;
}

.event-details li i {
  margin-right: 5px;
}
.custom-button {
  display: inline-block;
  padding: 5px 5px;
  background-color: #f0f0f0;
  color: #333;
  border-radius: 5px;
  cursor: pointer;
}

.custom-button:hover {
  background-color: #e0e0e0;
}

h1 {
  font-size: 3rem;
  font-weight: 700;
  color: black;
}
</style>
