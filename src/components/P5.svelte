<script>
  import Logo from "./Logo.svelte";
  import slider_old from "/p5/slider-old.png";
  import slider_new from "/p5/slider-new.png";
  import confirmation from "/p5/confirmation.png";
  import loading from "/p5/loading.png";
  import info from "/p5/info.png";
  import join_party from "/p5/join-party.png";
  import select_old from "/p5/select-old.png";
  import select_new from "/p5/select-new.png";
  import loading_two from "/p5/loading-two.png";
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
              <p class="font-semibold">
                Match Between System and Real World (2)
              </p>
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
          <tr>
            <td class="align-top">
              <p class="font-semibold">Visibility of System Status (3)</p>
            </td>
            <td class="align-top">
              <p class="pbody">Changed the budget selector from</p>
              <img src={slider_old} alt="Old slider" />
              <p class="pbody">to</p>
              <img src={slider_new} alt="New slider" />
            </td>
            <td class="align-top">
              <p class="pbody">
                The new design maintains flexibility but is easier for the user
                to keep track of what exactly they are choosing and the prices
                they are choosing. Improves feedback for the user.
              </p>
            </td>
          </tr>
          <tr>
            <td class="align-top">
              <p class="font-semibold">Error Prevention (3)</p>
            </td>
            <td class="align-top">
              <p class="pbody">
                Added confirmation dialogue before the party host chooses to
                compute the results of the party.
              </p>
              <img src={confirmation} alt="Confirmation" />
            </td>
            <td class="align-top">
              <p class="pbody">
                This extra dialogue helps with error prevention since finalizing
                a plan implies irreversible changes, and this box informs and
                makes the user conscious of the decision.
              </p>
            </td>
          </tr>
          <tr>
            <td class="align-top">
              <p class="font-semibold">Visibility of System Status (3)</p>
            </td>
            <td class="align-top">
              <p class="pbody">
                Added multiple loading screens, with a personalized loading
                indicator that includes the logo of the app.
              </p>
              <img src={loading} alt="Loading" />
            </td>
            <td class="align-top">
              <p class="pbody">
                This helps improve many of the points of feedback that indicated
                that there was a lack of feedback to the user when they took an
                action. The loading screens offer a time and space for users to
                process and be informed about what the app is doing.
              </p>
            </td>
          </tr>
          <tr>
            <td class="align-top">
              <p class="font-semibold">Visibility of System Status (2)</p>
            </td>
            <td class="align-top">
              <p class="pbody">
                We added a small and unintrusive text that indicates to the user
                where the rating comes from
              </p>
              <img src={info} alt="Info" />
            </td>
            <td class="align-top">
              <p class="pbody">
                Helps solve clarity regarding how restaurants are rated without
                adding a totally new screen or being very obtrusive.
              </p>
            </td>
          </tr>
          <tr>
            <td class="align-top">
              <p class="font-semibold">
                User Control and Freedom (3) & Error Prevention (2)
              </p>
            </td>
            <td class="align-top">
              <p class="pbody">Added join party code</p>
              <img src={join_party} alt="Join party" />
            </td>
            <td class="align-top">
              <p class="pbody">
                Allow joining with just a party link, which maximizes user
                engagement, streamlining onboarding.
              </p>
            </td>
          </tr>
          <tr>
            <td class="align-top">
              <p class="font-semibold">
                User Control & Freedom & Error Prevention [Severity: 4]
              </p>
            </td>
            <td class="align-top">
              <p class="pbody">From</p>
              <img src={select_old} alt="Old selection" />
              <p class="pbody">to</p>
              <img src={select_new} alt="New selection" />
            </td>
            <td class="align-top">
              <p class="pbody">
                Allow joining with just a party link, which maximizes user
                engagement, streamlining onboarding.
              </p>
            </td>
          </tr>
          <tr>
            <td class="align-top">
              <p class="font-semibold">Visibility of System Status (3)</p>
            </td>
            <td class="align-top">
              <img src={loading_two} alt="Loading" />
            </td>
            <td class="align-top">
              <p class="pbody">
                Added a loading indicator to tell the system is processing the
                query
              </p>
            </td>
          </tr>
        </tbody>
      </table>

      <p class="font-semibold">Changes not made</p>
      <table class="table">
        <thead>
          <tr>
            <th>Heuristic Violation</th>
            <th>Change Not Made</th>
            <th>Justification</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td class="align-top">
              <p class="font-semibold">Visibility of System Status</p>
            </td>
            <td class="align-top">
              <p class="pbody">
                We did not change Compatibility scores (97, 50, 43, 30) for each
                restaurant.
              </p>
            </td>
            <td class="align-top">
              <p class="pbody">
                As we are using a color gradient for each value, a score of 90
                indicates a top-rated restaurant, which we represent using green
                background.
              </p>
            </td>
          </tr>
          <tr>
            <td class="align-top">
              <p class="font-semibold">Consistency and Standards</p>
            </td>
            <td class="align-top">
              <p class="pbody">We did not change “Accept & Join” button.</p>
            </td>
            <td class="align-top">
              <p class="pbody">
                “Accept & Join” allows users to confirm their attendance and
                join the event in a single click, ensuring a smooth and
                efficient user experience.
              </p>
            </td>
          </tr>
        </tbody>
      </table>

      <!-- Partially Functioning Prototype -->
      <p class="pheading">Partially Functioning Prototype</p>

      <p class="font-semibold">GitHub repository</p>
      <p class="pbody">
        Code can be found <a
          class="underline hover:cursor-pointer text-blue-400"
          href="https://github.com/DesignStudio-HCI-Spring2026/p5-finalprototype-group5"
          target="_blank">here</a
        > once repository is made public by professor.
      </p>

      <p class="font-semibold">Demo</p>
      <iframe
        width="100%"
        class="h-auto aspect-video"
        src="https://www.youtube.com/embed/YwxvQCa16U4?si=O3aHzuWEX3C3sj2Y"
        title="Grubable P5 Demo"
        frameborder="0"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
        referrerpolicy="strict-origin-when-cross-origin"
        allowfullscreen
      ></iframe>

      <p class="font-semibold">Contributions</p>
      <p class="pbody">
        All team members contributed collaboratively to the development of the
        final Grubable prototype. Everyone played a role in all parts of the
        process, but some noteworthy contributions were as follows:
      </p>
      <ul class="plist">
        <li>
          <p class="pbody">
            Julian: dealt with scaffolding the initial app structure,
            implemented the base parties pages/create party flow and helped iron
            out final details on the prototype
          </p>
        </li>
        <li>
          <p class="pbody">
            Andrew: built the restaurants pages and flows, finalized the designs
            on figma
          </p>
        </li>
        <li>
          <p class="pbody">
            Sumon: compiled heuristic evals, implemented join party flow, and
            wrote the final report.
          </p>
        </li>
      </ul>

      <!-- Discussion -->
      <p class="pheading">Discussion</p>
      <p class="pbody">
        Through the user-centered design process (from emphasizing to testing),
        we learned that users with dietary restrictions need more than just
        access to menu information. They also need confidence, privacy, and a
        smoother way to participate in the group dining without feeling singled
        out. This insight shaped the direction of our prototype. Instead of
        focusing on the information delivery, we designed Grubable to support
        both individual decision making and social comfort through features like
        restaurant lookup, dietary flags, and anonymous party sharing. The
        process helped us better understand that a useful product must address
        both practical needs and emotional concerns.
      </p>
      <p class="pbody">
        At each stage of prototyping, we made tradeoffs among feature scope,
        usability, and technical feasibility. During the low-fidelity stage, we
        initially proposed many features that we believed would help people with
        dietary restrictions caused by diabetes and other health conditions.
        However, after conducting interviews with a diverse group of users,
        including professionals, students, older adults, and younger
        participants, we realized that users’ needs and preferences were broader
        and more varied than we had first assumed. As a result, in the
        mid-fidelity stage, we removed several features that had seemed
        essential at the beginning and focused instead on the features that were
        most strongly supported by user feedback. By the high-fidelity stage,
        our decisions were guided by user interviews, user perceptions, and
        heuristic evaluation. For example, rather than allowing users to join
        only through a shared party link, we included an “Enter Party Code”
        feature to better support privacy while still keeping onboarding simple.
        We also removed the profile feature to reduce complexity. Another
        important tradeoff came from heuristic evaluation feedback: instead of
        limiting users to only a few predefined dietary restriction options, we
        simplified the design to better support users in entering their own
        restrictions. In addition, we made several refinements in the revised
        mockup, such as adding a loading button and including a note explaining
        how restaurant scores are determined. As development continued, we
        placed greater emphasis on bug fixing, product testing, and error
        handling to make the final prototype more stable and polished. These
        tradeoffs helped us create a prototype that was focused, functional, and
        better aligned with real user needs.
      </p>
    </div>
  </div>
</div>
