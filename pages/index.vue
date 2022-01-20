<style scoped>
  .grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    column-gap: 1rem;
    row-gap: 2rem
  }
  .grid img {
    width: 100%;
    height: 200px;
    object-fit: cover
  }
  .grid > div {
    display: grid;
    grid-template-rows: auto auto 1fr auto;
    grid-gap: 1rem
  }
  .grid > div * {
    margin: 0
  }
  .placeholder {
    background-color: grey
  }
  h2 {
    margin-top: 4rem
  }
</style>

<template>
  <div class="maxWidth">
    <h1>
      An alumni is a former student of Solent University.
    </h1>
    <h2 id="how-we-can-help">
      How We Can Help
    </h2>
    <p>
      As a part of our global alumni community, you can take advantage of a range of benefits. Have a browse below to see what’s on offer, and remember to check back often for any newly added benefits.
    </p>
    <div class="grid">
      <div>
        <img src="https://www.solent.ac.uk/image-library/alumni/norway-alumni-event-5.jpg">
        <h3>
          Exclusive events
        </h3>
        <p>
          We run a range of events open to our alumni throughout the year from alumni reunions to guest lectures.
        </p>
        <a class="find-out-more" href="#">
          Find out more >
        </a>
      </div>
      <div>
        <img src="https://www.solent.ac.uk/image-library/alumni/postgrad-study.jpg">
        <h3>
          Discount on postgraduate study
        </h3>
        <p>
          If you're looking to further your studies, you could be eligible for up to a 50% reduction of tuition fees on a postgraduate degree or professional qualification.
        </p>
        <a class="find-out-more" href="#">
          Find out more >
        </a>
      </div>
      <div>
        <img src="https://www.solent.ac.uk/image-library/alumni/gym.jpg">
        <h3>
          Discounted gym prices
        </h3>
        <p>
          If you would like to use the gym, please pre-book via the Solent Gym app. Each gym session will be at the reduced price of £3 for alumni.
        </p>
        <a class="find-out-more" href="#">
          Find out more >
        </a>
      </div>
      <div>
        <img src="https://www.solent.ac.uk/image-library/alumni/careers-support.jpg">
        <h3>
          Careers support
        </h3>
        <p>
          Careers support from the University doesn't end after you leave. Whether you're looking for career advice or business support, we're here to help.
        </p>
        <a class="find-out-more" href="#">
          Find out more >
        </a>
      </div>
      <div>
        <img src="https://www.solent.ac.uk/image-library/alumni/library-2.jpg">
        <h3>
          Free library access
        </h3>
        <p>
          Students who have graduated from Solent University are entitled to free subscriber membership of the library.
        </p>
        <a class="find-out-more" href="#">
          Find out more >
        </a>
      </div>
      <div>
        <img src="https://www.solent.ac.uk/image-library/alumni/accommodation.jpg">
        <h3>
          Accommodation
        </h3>
        <p>
          If you're planning a stay in Southampton during the summer, we can offer low-cost accommodation in the student residences.
        </p>
        <a class="find-out-more" href="#">
          Find out more >
        </a>
      </div>
      <div>
        <img src="https://www.solent.ac.uk/image-library/alumni/sonar.jpg">
        <h3>
          Sonar Film
        </h3>
        <p>
          Sonar Film is a multi-award winning 96-seat cinema, voluntarily run by students. All films are £4 when you display a valid Solent student, staff or alumni ID card, and £4.50 for anyone else.
        </p>
        <a class="find-out-more" href="#">
          Find out more >
        </a>
      </div>
      <div>
        <img src="https://www.solent.ac.uk/image-library/alumni/transcripts.jpg">
        <h3>
          Transcripts and references
        </h3>
        <p>
          To request an academic reference, confirmation of attendance or a transcript of results, please contact alumni@solent.ac.uk and we'll make sure your details are passed on to the correct team.
        </p>
        <a class="find-out-more" href="#">
          Find out more >
        </a>
      </div>
      <div>
        <img src="https://www.solent.ac.uk/image-library/alumni/winter-grad-2016.JPG">
        <h3>
          Replacement degree certificates
        </h3>
        <p>
          Your degree certificate would have been awarded to you on completion of your qualification here at Solent University. Alumni are able to order replacement certificates online.
        </p>
        <a class="find-out-more" href="#">
          Find out more >
        </a>
      </div>
      <div>
        <img src="https://www.solent.ac.uk/image-library/alumni/solent-hoodie.jpg">
        <h3>
          University merchandise
        </h3>
        <p>
          Missing us? Buying branded goods is a great way to remember your time at Solent. Browse our online shop to pick up a memento. Our third party supplier, Campus Global Ltd will send out your goods within 14 days from receipt of your order. 10% of all merchandise sales (excluding 'class of' gifts) goes towards our Local Student Bursary Scheme.
        </p>
        <a class="find-out-more" href="#">
          Find out more >
        </a>
      </div>
      <div>
        <img src="https://www.solent.ac.uk/image-library/alumni/alumni-id-cards.jpg">
        <h3>
          Free alumni ID card
        </h3>
        <p>
          Use your alumni ID card to receive discounted entry at Sonar Film and the library, as well as discounted gym membership.
        </p>
        <a class="find-out-more" href="#">
          Find out more >
        </a>
      </div>
    </div>
    <h2 id="give-back">
      Give Back
    </h2>
    <p>
      As part of the Solent University alumni community, there are plenty of opportunities for you to get involved, both on and off campus. Alumni can help to inspire current and prospective students by taking part in mentoring schemes, sharing their industry experience, guest speaking or arranging work experience placements.
    </p>
    <div class="grid">
      <div>
        <img class="placeholder">
        <h3>
          Share your story
        </h3>
        <p>
          We are always keen to hear how your career has progressed. Fill out our alumni case study form and we will forward your story and details on to relevant university colleagues. If you've got a great story that could inspire Solent students, we'd love to share it on the site.
        </p>
        <a class="find-out-more" href="#">
          Find out more >
        </a>
      </div>
      <div>
        <img class="placeholder">
        <h3>
          Volunteer your time
        </h3>
        <p>
          As a Solent alum, you are a living example of the opportunities available to current students. From mentoring to acting as ambassador, guest lecturing and sharing your story, there's a range of activities you can help us with.
        </p>
        <a class="find-out-more" href="#">
          Find out more >
        </a>
      </div>
      <div>
        <img class="placeholder">
        <h3>
          Donate
        </h3>
        <p>
          Looking to give back to Solent? Charitable donations of any size can make a real difference. Your support will help us to provide excellent teaching facilities and learning opportunities to current and future students. It will also help to expand our research, reduce student hardship, and make a difference to almost every aspect of university life.
        </p>
        <a class="find-out-more" href="#">
          Find out more >
        </a>
      </div>
    </div>
    <h2 id="Events">
      Events
    </h2>
    <div class="grid">
      <div>
        <img class="placeholder">
        <h3>
          Event Title
        </h3>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. In tempor, turpis id mollis tristique, magna nisi lobortis justo, non porttitor nibh lorem a sem.
        </p>
        <a class="find-out-more" href="#">
          Find out more >
        </a>
      </div>
      <div>
        <img class="placeholder">
        <h3>
          Event Title
        </h3>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. In tempor, turpis id mollis tristique, magna nisi lobortis justo, non porttitor nibh lorem a sem.
        </p>
        <a class="find-out-more" href="#">
          Find out more >
        </a>
      </div>
      <div>
        <img class="placeholder">
        <h3>
          Event Title
        </h3>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. In tempor, turpis id mollis tristique, magna nisi lobortis justo, non porttitor nibh lorem a sem.
        </p>
        <a class="find-out-more" href="#">
          Find out more >
        </a>
      </div>
      <div>
        <img class="placeholder">
        <h3>
          Event Title
        </h3>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. In tempor, turpis id mollis tristique, magna nisi lobortis justo, non porttitor nibh lorem a sem.
        </p>
        <a class="find-out-more" href="#">
          Find out more >
        </a>
      </div>
    </div>
    <h2 id="Events">
      News
    </h2>
    <div class="grid">
      <div>
        <img class="placeholder">
        <h3>
          News Title
        </h3>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. In tempor, turpis id mollis tristique, magna nisi lobortis justo, non porttitor nibh lorem a sem.
        </p>
        <a class="find-out-more" href="#">
          Find out more >
        </a>
      </div>
      <div>
        <img class="placeholder">
        <h3>
          News Title
        </h3>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. In tempor, turpis id mollis tristique, magna nisi lobortis justo, non porttitor nibh lorem a sem.
        </p>
        <a class="find-out-more" href="#">
          Find out more >
        </a>
      </div>
      <div>
        <img class="placeholder">
        <h3>
          News Title
        </h3>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. In tempor, turpis id mollis tristique, magna nisi lobortis justo, non porttitor nibh lorem a sem.
        </p>
        <a class="find-out-more" href="#">
          Find out more >
        </a>
      </div>
      <div>
        <img class="placeholder">
        <h3>
          News Title
        </h3>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. In tempor, turpis id mollis tristique, magna nisi lobortis justo, non porttitor nibh lorem a sem.
        </p>
        <a class="find-out-more" href="#">
          Find out more >
        </a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  head () {
    return {
      title: 'Home',
      meta: [
        { hid: 'description', name: 'description', content: 'REPLACE' },
        { hid: 'og:title', property: 'og:title', content: 'Home' },
        { hid: 'og:description', property: 'og:description', content: 'REPLACE' },
        { hid: 'og:image', property: 'og:image', content: 'REPLACE' },
        { hid: 'twitter:title', name: 'twitter:title', content: 'Home' },
        { hid: 'twitter:description', name: 'twitter:description', content: 'REPLACE' },
        { hid: 'twitter:img', name: 'twitter:img', content: 'REPLACE' }
      ],
      link: [
        { hid: 'canonical', rel: 'canonical', href: 'REPLACE' }
      ]
    }
  }
}
</script>
