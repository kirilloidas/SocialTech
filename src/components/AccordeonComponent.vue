<template>
  <div class="accordion" id="accordionExample">
    <div class="accordion-item">
      <h2 class="accordion-header" id="headingOne">
        <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#collapseOne" aria-expanded="true" aria-controls="collapseOne">
          The analysis
        </button>
      </h2>
      <div id="collapseOne" class="accordion-collapse collapse show" aria-labelledby="headingOne" data-bs-parent="#accordionExample">
        <ul class="secondary-list">
          <li class="secondary-list__item">
            Do you have one user in more than one variant of the same AB test?
          </li>
          <li class="secondary-list__item">
            Are you users actually getting the treatment we expect them to get?
          </li>
          <li class="secondary-list__item">
            Do we have enough users in our AB test? Are those users representative for the total population?
          </li>
        </ul>
      </div>
    </div>
    <div class="accordion-item">
      <h2 class="accordion-header" id="headingTwo">
        <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseTwo" aria-expanded="false" aria-controls="collapseTwo">
          Our data
        </button>
      </h2>
      <div id="collapseTwo" class="accordion-collapse collapse" aria-labelledby="headingTwo" data-bs-parent="#accordionExample">
        <ul class="secondary-list">
          <li class="secondary-list__item">
            Do you have one user in more than one variant of the same AB test?
          </li>
          <li class="secondary-list__item">
            Are you users actually getting the treatment we expect them to get?
          </li>
          <li class="secondary-list__item">
            Do we have enough users in our AB test? Are those users representative for the total population?
          </li>
        </ul>
      </div>
    </div>
    <div class="accordion-item">
      <h2 class="accordion-header" id="headingThree">
        <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseThree" aria-expanded="false" aria-controls="collapseThree">
          Our study case
        </button>
      </h2>
      <div id="collapseThree" class="accordion-collapse collapse" aria-labelledby="headingThree" data-bs-parent="#accordionExample">
        <ul class="secondary-list">
          <li class="secondary-list__item">
            Do you have one user in more than one variant of the same AB test?
          </li>
          <li class="secondary-list__item">
            Are you users actually getting the treatment we expect them to get?
          </li>
          <li class="secondary-list__item">
            Do we have enough users in our AB test? Are those users representative for the total population?
          </li>
        </ul>
      </div>
    </div>
    <div class="accordion-item">
      <h2 class="accordion-header" id="headingThree">
        <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseThree" aria-expanded="false" aria-controls="collapseThree">
          Hands on analyzing
        </button>
      </h2>
      <div id="collapseThree" class="accordion-collapse collapse" aria-labelledby="headingThree" data-bs-parent="#accordionExample">
        <ul class="secondary-list">
          <li class="secondary-list__item">
            Do you have one user in more than one variant of the same AB test?
          </li>
          <li class="secondary-list__item">
            Are you users actually getting the treatment we expect them to get?
          </li>
          <li class="secondary-list__item">
            Do we have enough users in our AB test? Are those users representative for the total population?
          </li>
        </ul>
      </div>
    </div>
    <div class="accordion-item">
      <h2 class="accordion-header" id="headingThree">
        <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseThree" aria-expanded="false" aria-controls="collapseThree">
          Initialization
        </button>
      </h2>
      <div id="collapseThree" class="accordion-collapse collapse" aria-labelledby="headingThree" data-bs-parent="#accordionExample">
        <ul class="secondary-list">
          <li class="secondary-list__item">
            Do you have one user in more than one variant of the same AB test?
          </li>
          <li class="secondary-list__item">
            Are you users actually getting the treatment we expect them to get?
          </li>
          <li class="secondary-list__item">
            Do we have enough users in our AB test? Are those users representative for the total population?
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>
<script setup>

</script>
<style lang="css" scoped>
.accordion {
  width: 600px;
  box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.02), 0px 4px 17px rgba(0, 0, 0, 0.14), 0px 4px 22px rgba(0, 0, 0, 0.12);
  border-radius: 8px;
  margin-left: auto;
  margin-right: auto;
}
.accordion-button {
  /* border: none !important; */
  color: #2B41B7;
  background: #FAF8F6;
  font-style: normal;
font-weight: 800;
font-size: 16px;
line-height: 24px;
}
.accordion-button.collapsed {
  /* border-bottom-image-width: 0; */
  background: white;
  color: #0D2A54;
}
.collapse {
  background: #FAF8F6;
  padding: 8px 24px 24px 12px;
}
.secondary-list {
  list-style-type: circle;
  margin-bottom: 0;
}
.secondary-list__item {
  font-style: normal;
font-weight: 600;
font-size: 14px;
line-height: 24px;
}
.secondary-list__item:not(:last-child) {
  margin-bottom: 8px;
}

@media screen and (max-width: 600px) {
  .accordion {
    width: 500px;
  }
}
@media screen and (max-width: 500px) {
  .accordion {
    width: 400px;
  }
}
@media screen and (max-width: 400px) {
  .accordion {
    width: 300px;
  }
}
</style>