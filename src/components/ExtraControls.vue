<template>
  <div class="extra-controls">
    <div class="extra-controls--queue">
      <button class="control-button">
        <svg xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 100 100" height="20px">
          <path d="M25.3,32.9L5,48.6L5.2,17L25.3,32.9z M34.2,34.2h59.4c0.8,0,1.4-0.6,1.4-1.4c0-0.8-0.6-1.4-1.4-1.4H34.2  c-0.8,0-1.4,0.6-1.4,1.4C32.7,33.6,33.4,34.2,34.2,34.2z M93.6,55.7H6.6c-0.8,0-1.4,0.6-1.4,1.4c0,0.8,0.6,1.4,1.4,1.4h86.9  c0.8,0,1.4-0.6,1.4-1.4C95,56.4,94.4,55.7,93.6,55.7z M93.6,80.1H6.6c-0.8,0-1.4,0.6-1.4,1.4S5.8,83,6.6,83h86.9  c0.8,0,1.4-0.6,1.4-1.4S94.4,80.1,93.6,80.1z" /></svg>
      </button>
    </div>
    <div class="extra-controls--volume">
      <div class="volume-bar">
        <button class="volume-bar--icon control-button">
          <svg xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 100 100" width="20px" height="20px">
            <rect id="svgEditorBackground" x="0" y="0" width="100" height="125" style="fill:none;stroke:none;" />
            <g>
              <g>
                <path d="M47.1,82.3L24,61.3H8.8V38.8H24l23.1-20.9L47.1,82.3L47.1,82.3z M12.6,57.5h12.8l18,16.7V25.9l-18,16.6H12.6V57.5z" />
              </g>
              <g>
                <path d="M78.8,84.9l-3.0999999999999943,-2.200000000000003c6.900000000000006,-9.700000000000003,10.5,-21,10.5,-32.7c0,-11.700000000000003,-3.5999999999999943,-23,-10.400000000000006,-32.7l3.0999999999999943,-2.1999999999999993c7.300000000000011,10.3,11.100000000000009,22.400000000000002,11.100000000000009,34.900000000000006c0,12.5,-3.9000000000000057,24.599999999999994,-11.200000000000003,34.900000000000006Z" />
              </g>
              <g>
                <path d="M67.7,77.8l-3-2.2c5.6-7.5,8.5-16.3,8.5-25.6s-2.9-18.3-8.3-25.7l3-2.2c5.8,8,9,17.9,9,27.9C77,60,73.8,69.6,67.7,77.8z" />
              </g>
              <g>
                <path d="M57.8,70.7l-3.1-2.1c3.6-5.5,5.6-12,5.6-18.6c0-6.8-2-13.3-5.8-18.9l3.1-2.1c4.2,6.2,6.4,13.5,6.4,21    C63.9,57.4,61.8,64.5,57.8,70.7z" />
              </g>
            </g><text x="0" y="115" fill="#000000" font-size="5px" font-weight="bold" font-family="'Helvetica Neue', Helvetica, Arial-Unicode, Arial, Sans-serif"></text><text
              x="0" y="120" fill="#000000" font-size="5px" font-weight="bold" font-family="'Helvetica Neue', Helvetica, Arial-Unicode, Arial, Sans-serif"></text>
          </svg>
        </button>
        <div class="volume-bar__progress-bar progress-bar">
          <progress-bar/>
        </div>
      </div>
    </div>
  </div>
</template>


<script>
  import ProgressBar from './ProgressBar';

  export default {
    name: 'ExtraControls',
    components: {
      ProgressBar
    },
    data() {
      return {

      };
    },
  }

</script>
