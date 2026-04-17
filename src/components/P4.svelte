<!-- @component
P4 component
 -->
<script lang="ts">
  import Logo from "./Logo.svelte";
</script>

<div class="pcard collapse collapse-arrow">
  <input type="checkbox" name="P4" id="P4" checked />
  <div class="collapse-title flex justify-between items-center">
    <h1 class="pcard-header">P4 - Med-Fi Prototype</h1>
    <h2 class="pcard-date">3/27/26</h2>
  </div>
  <div class="pcard-content pcard-body collapse-content">
    <Logo />

    <!-- Section 1: Implemented Flows -->
    <p class="pheading">Implemented Flows</p>

    <!-- Flow A -->
    <p class="font-semibold">a) Restaurant Discovery</p>
    <p class="pbody">
      The Restaurant Discovery flow is designed for single users that want to
      easily and quickly search for a restaurant near or an option they have in
      mind and rate it as an option depending on their dietary restriction. Once
      the options are displayed our algorithm will rate based on accessibility
      and give pointers or flags to look out for depending on dietary
      restrictions.
    </p>

    <!-- Flow B -->
    <p class="font-semibold">b) Party Creation</p>
    <p class="pbody">
      This flow is intended to reduce the social friction when choosing
      restaurants to go in groups, especially reducing the discomfort for people
      with strict dietary restrictions and/or budget restrictions to share it
      with the group. This allows the creation of a party including name and
      zipcode for all members and also the creator inputs their personal budget
      and dietary restrictions as well. Then they can share the party through a
      link and then decide when to compute the results, which locks the party
      and displays the result along with a recommendation from the algorithm
      based on the group's sensibilities.
    </p>

    <!-- Flow C -->
    <p class="font-semibold">c) Party Viewing as a Member (complex)</p>
    <p class="pbody">
      When a user joins a party through a shared link, it appears in their
      Joined Parties tab, provided they have already submitted their
      preferences. Tapping on a party shows one of two states: if the creator
      has computed the results, the final recommendation and results are
      displayed; if the creator has not yet closed the party, the results remain
      pending and the member must wait.
    </p>

    <!-- Section 2: Prototype in Figma -->
    <p class="pheading">Prototype in Figma</p>

    <p class="font-semibold">Interactive Prototype</p>
    <iframe
      class="h-auto aspect-video"
      width="100%"
      src="https://embed.figma.com/proto/15mgqxKDiOYfHkykBzMnf0/P4----MedFi-Prototype?node-id=1-5&p=f&scaling=scale-down&content-scaling=fixed&page-id=0%3A1&starting-point-node-id=1%3A9&show-proto-sidebar=1&embed-host=share"
      title="P4 Interactive Prototype"
      frameborder="0"
      allowfullscreen
    ></iframe>

    <p class="font-semibold">Static Mockup</p>
    <iframe
      class="h-auto aspect-video"
      width="100%"
      src="https://embed.figma.com/design/15mgqxKDiOYfHkykBzMnf0/P4----MedFi-Prototype?node-id=0-1&embed-host=share"
      title="P4 Static Mockup"
      frameborder="0"
      allowfullscreen
    ></iframe>
  </div>
</div>
