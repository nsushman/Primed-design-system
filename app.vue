<template>
  <div>
    <!-- Your page content here -->

    <button @click="toggleMode">Toggle Mode</button>

    <div>
      <!--Start of sample div-->
      <h1>Design System Guide</h1>

      <div class="section">
        <h2>Text Inputs</h2>
        <div class="control">
          <label for="text-input">Text Input:</label>
          <input type="text" id="text-input" placeholder="Enter text" />
        </div>
        <div class="control">
          <label for="textarea">Textarea:</label>
          <textarea id="textarea" placeholder="Enter text"></textarea>
        </div>
      </div>

      <div class="section">
        <h2>Select Dropdown</h2>
        <div class="control">
          <label for="select-dropdown">Select Dropdown:</label>
          <select id="select-dropdown">
            <option value="">Select an option</option>
            <option value="option1">Option 1</option>
            <option value="option2">Option 2</option>
            <option value="option3">Option 3</option>
          </select>
        </div>
      </div>

      <div class="section">
        <h2>Buttons</h2>
        <div class="control">
          <a href="#" class="button">Button</a>
        </div>
        <div class="control">
          <button class="button">Button</button>
        </div>
      </div>
    </div>
    <!--End of sample div-->

    <div>
      <!--Start of Main div-->
      <h1>H1 Major heading</h1>
      <h2>H2 Page heading</h2>
      <h3>H3 Section header</h3>
      <th>Table Header</th>
      <small>Small text</small>
    </div>
    <!--End of Main div-->
  </div>
</template>

<script>
export default {
  data() {
    return {
      isDarkMode: false,
    };
  },
  methods: {
    toggleMode() {
      this.isDarkMode = !this.isDarkMode;
      if (this.isDarkMode) {
        document.body.classList.add('dark-mode');
      } else {
        document.body.classList.remove('dark-mode');
      }
    },
  },
};
</script>

<style lang="css">
@import './app.scss';
</style>
