<script>
  import Logo from "./Logo.svelte";
</script>

<!-- @component
P5 component
 -->
<div class="pcard collapse collapse-arrow">
  <input type="checkbox" name="P5" id="P5" checked />
  <div class="collapse-title flex justify-between items-center">
    <h1 class="pcard-header">P5 - Final Prototype</h1>
    <h2 class="pcard-date">4/17/26</h2>
  </div>
  <div class="pcard-content collapse-content">
    <div class="pcard-body">
      <!-- Final Interactive Prototype -->
      <p class="pheading">Final Interactive Prototype</p>
      <Logo />
      <p class="pheading">Value Proposition</p>
      <p class="pbody">
        Grubable makes organizing food get-togethers easy by providing
        preference-inclusive recommendations.
      </p>

      <p class="pheading">Mockup</p>
      <p class="font-semibold">Interactive Prototype</p>
      <iframe
        class="h-auto aspect-video"
        width="100%"
        src="https://embed.figma.com/proto/DiIQnJZOLh1Ziq9liNfUV7/P5----Final-Prototype?scaling=scale-down&content-scaling=fixed&page-id=0%3A1&node-id=1-5&starting-point-node-id=1%3A9&show-proto-sidebar=1&embed-host=share"
        title="P5 Interactive Prototype"
        frameborder="0"
        allowfullscreen
      ></iframe>

      <p class="font-semibold">Static Mockup</p>
      <iframe
        class="h-auto aspect-video"
        width="100%"
        src="https://embed.figma.com/design/DiIQnJZOLh1Ziq9liNfUV7/P5----Final-Prototype?embed-host=share"
        title="P5 Static Mockup"
        frameborder="0"
        allowfullscreen
      ></iframe>

      <p class="font-semibold">Changes made</p>
      <table class="table">
        <thead>
          <tr>
            <th>Heuristic Violation</th>
            <th>Change</th>
            <th>Justification</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td class="align-top">
              <p class="pheading">Match Between System and Real World (2)</p>
            </td>
            <td class="align-top">
              <p class="pbody">
                Changed the label of the dietary restriction report in the form
                from “report” to “share anonymously.
              </p>
            </td>
            <td class="align-top">
              <p class="pbody">
                The word “report” is generally associated with a confession of
                something that went wrong, but we are trying to make people with
                restrictions feel included. Share is more welcoming.
              </p>
            </td>
          </tr>
        </tbody>
      </table>

      <p class="font-semibold">Changes not made</p>
      <p class="pbody">
        <!-- Changes not made content here -->
      </p>

      <!-- Partially Functioning Prototype -->
      <p class="pheading">Partially Functioning Prototype</p>

      <p class="font-semibold">GitHub repository</p>
      <p class="pbody">
        <!-- GitHub repository content here -->
      </p>

      <p class="font-semibold">Embedded demo video</p>
      <p class="pbody">
        <!-- Embedded demo video content here -->
      </p>

      <!-- Discussion -->
      <p class="pheading">Discussion</p>
      <p class="pbody">
        <!-- Discussion content here -->
      </p>
    </div>
  </div>
</div>
