<script>
  import brainstorm_1 from "/p3/brainstorm-1.png";
  import brainstorm_2 from "/p3/brainstorm-2.png";
  import brainstorm_3 from "/p3/brainstorm-3.png";
  import affinity from "/p3/affinity.png";
  import initial_1 from "/p3/1-initial.png";
  import board_1_1 from "/p3/1-board-1.png";
  import board_1_2 from "/p3/1-board-2.png";
  import board_2_1 from "/p3/2-board-1.png";
  import board_2_2 from "/p3/2-board-2.png";
  import board_2_3 from "/p3/2-board-3.png";
  import lofi_1 from "/p3/1-lofi.png";
  import components_1 from "/p3/1-components.png";
  import lofi_2 from "/p3/2-lofi.png";
  import components_2 from "/p3/2-components.png";
  import testing_1 from "/p3/1-testing.png";
</script>

<!-- @component
P2 component
 -->
<div class="pcard collapse collapse-arrow">
  <input type="checkbox" name="P2" id="P2" checked />
  <div class="collapse-title flex justify-between items-center">
    <h1 class="pcard-header">P3 - Lofi Prototyping + Testing</h1>
    <h2 class="pcard-date">2/18/26</h2>
  </div>
  <div class="pcard-content pcard-body collapse-content">
    <p class="pheading">Introduction</p>
    <ul class="plist">
      <li>
        <p>
          <span class="font-semibold">Solution Name:</span> GrubAble
        </p>
      </li>
      <li>
        <p>
          <span class="font-semibold">Team:</span> Andrew Lu, Julian Lucio Paredes,
          Sumon Kanti Dey
        </p>
      </li>
      <li>
        <p>
          <span class="font-semibold">Value proposition:</span> GrubAble helps people
          with strict dietary restrictions evaluate food options confidently and reduces
          the social pressure of explaining restrictions when dining with others.
        </p>
      </li>
      <li>
        <p>
          <span class="font-semibold">Mission statement:</span> Enable people with
          dietary restrictions to easily assess restaurants and menu items, access
          reliable insights from their community, and feel comfortable participating
          in group dining decisions without being singled out.
        </p>
      </li>
      <li>
        <p>
          <span class="font-semibold">Problem statement:</span> People with strict
          dietary restrictions lack a centralized, easy-to-use way to access trustworthy
          information about safe food options. In social situations, they often feel
          guilty for “holding the group back” or creating extra work when sharing
          their restrictions. This pressure can lead some people to stay quiet, take
          risks, or feel anxious later because they're unsure whether they ate something
          problematic during the day
        </p>
      </li>
      <li>
        <p>
          <span class="font-semibold">Solution overview:</span> The team considered
          two core ideas:
        </p>
        <ul class="plist-2">
          <li>
            Personalized chat assistant: A conversational interface that
            supports users day-to-day by: flagging potentially risky foods,
            suggesting safer meal options, and helping users assess risk based
            on their dietary profile and context.
          </li>
          <li>
            Restaurant ranking + anonymous group decision tool: A web-based
            experience that improves both accessibility and social comfort by:
            analyzing restaurant menus/websites and rating options based on
            dietary compatibility, allowing users to save and compare
            restaurants they're considering, and also supporting group outings
            through an anonymous poll, where each person enters their budget and
            dietary restrictions. The app then recommends restaurants using
            dietary compatibility, community ratings, and price, reducing the
            burden on the person with restrictions to repeatedly explain
            themselves or feel singled out.
          </li>
        </ul>
      </li>
    </ul>
    <p class="pheading">Brainstorming Session</p>
    <p class="pbody">
      Our brainstorming session was productive and helped us push beyond our
      comfort zones. Each team member spent 10 minutes sketching and ideating up
      to six solution concepts. Although none of us reached six, the activity
      generated strong discussion, and every idea contributed at least one
      feature we later considered as a group.
    </p>
    <p class="pbody">
      One of the biggest challenges was overcoming the self-imposed “creativity
      blockade.” Before we even finished sketching, we found ourselves
      pre-judging ideas and focusing on why they wouldn't work. Letting go of
      that early criticism was difficult, but once we managed it, the process
      became much more satisfying and yielded more original concepts.
    </p>
    <p class="pbody">
      It was also interesting that our sketches looked like an illegible mess to
      an outsider, but when we reviewed them together, each symbol gained clear
      meaning and purpose through group discussion.
    </p>
    <p class="pbody">Here is each teammates brainstorming session:</p>
    <img src={brainstorm_1} alt="Brainstorming 1" />
    <img src={brainstorm_2} alt="Brainstorming 2" />
    <img src={brainstorm_3} alt="Brainstorming 3" />

    <p class="pheading">Affinity Diagram</p>
    <p class="pbody">
      Then the team proceeded to create an affinity diagram to organize the
      feature ideas. The team decided on 4 main overarching categories and then
      each feature was connected to one or more of the categories.
    </p>
    <img src={affinity} alt="Affinity Diagram" />
    <p class="pbody">
      From the brainstorming session and the creation of the affinity diagram,
      the team singled out the two most promising ideas that will be developed
      in the following section.
    </p>

    <p class="pheading">First Idea: Party Manager + Restaurant Rater</p>
    <p class="font-semibold">Initial Description</p>
    <img src={initial_1} alt="Initial Brainstorming" />
    <p class="font-semibold">Task Storyboards</p>
    <img src={board_1_1} alt="Boards 1 & 2" />
    <img src={board_1_2} alt="Board 3" />
    <p class="font-semibold">Pros:</p>
    <ul class="plist">
      <li>
        Works across two key contexts: supports users both in social dining
        situations and when deciding alone ahead of time.
      </li>
      <li>
        Reduces pressure and builds community: lowers the burden of repeatedly
        disclosing restrictions while encouraging shared experiences and
        recommendations.
      </li>
      <li>
        Creates accountability incentives: a visible dietary-compatibility
        rating can motivate restaurants to take restrictions more seriously and
        improve transparency.
      </li>
      <li>
        Decision support, not medical advice: focuses on helping users compare
        options without requiring medical-grade certainty or making health
        claims.
      </li>
    </ul>
    <p class="font-semibold">Cons:</p>
    <ul class="plist">
      <li>
        Restaurant menu data is inconsistent: websites and menus can be
        incomplete, unclear, or formatted in ways that are difficult to parse
        reliably.
      </li>
      <li>
        Rating disagreements are likely: users may not align with a single
        scoring algorithm because risk tolerance varies by person and
        restriction severity.
      </li>
      <li>
        High UX bar: the tool must be extremely quick and easy to use, or people
        won't bother during real group planning.
      </li>
      <li>
        Cold-start problem for community input: meaningful community ratings and
        reviews take time to accumulate before the system feels trustworthy and
        robust.
      </li>
    </ul>

    <p class="pheading">Second Idea: Chatbot + Specialist-Backed System</p>
    <p class="pbody">Task 1: Quick Info Lookup</p>
    <img src={board_2_1} alt="Board 1" />
    <p class="pbody">Task 2: Context-Aware Recommendation</p>
    <img src={board_2_2} alt="Board 2" />
    <p class="pbody">
      Task 3: Multi-step, Risk-Sensitive, Specialist Involvement
    </p>
    <img src={board_2_3} alt="Board 3" />
    <p class="font-semibold">Pros:</p>
    <ul class="plist">
      <li>
        Tailors suggestions and warnings to the user's exact restrictions,
        severity, preferences, and “safe” brands/foods.
      </li>
      <li>
        Fast answers while reading menus, ingredients, or ordering reduces
        decision fatigue when you're out or busy.
      </li>
      <li>
        Adds day-to-day confidence; can log meals/snacks and help users reflect
        on what might have caused symptoms or discomfort later.
      </li>
      <li>
        Accessible and low barrier; a chat interface feels familiar and can be
        easier than navigating complex filters or long menus.
      </li>
    </ul>
    <p class="font-semibold">Cons:</p>
    <ul class="plist">
      <li>
        Menus and labels can be vague, and the assistant may miss hidden
        ingredients or cross-contamination risks may lead to misinformation
      </li>
      <li>
        Trust and safety concerns: users might treat it like medical advice, so
        the UX must be conservative with clear disclaimers and uncertainty
        handling.
      </li>
      <li>
        It depends on good input, if ingredient data is missing or users can't
        provide details, the assistant's usefulness drops.
      </li>
      <li>
        Privacy sensitivity: dietary profiles and meal logs are
        personal/health-adjacent data and require strong protections.
      </li>
      <li>
        Complex implementation: doing this well requires reliable retrieval
        (menus/labels), user profiling, logging, confidence scoring, and safety
        guardrails—not just "a chatbot."
      </li>
      <li>
        There is a risk of being “GPT wrapper” might feel like a thin layer on
        top of a generic LLM (without unique data, workflows, or features).
      </li>
    </ul>

    <p class="pheading">Lofi Sketch + Components</p>
    <p class="pbody">Idea 1</p>
    <img src={lofi_1} alt="Lofi Drawing" />
    <img src={components_1} alt="Components" />
    <p class="pbody">Idea 2</p>
    <img src={lofi_2} alt="Lofi Drawing" />
    <img src={components_2} alt="Components" />

    <p class="pheading">Usability Testing</p>
    <p class="pbody">Idea 1</p>
    <img src={testing_1} alt="Testing" />
    <p class="pbody">Idea 2</p>
    <p class="pbody">
      In order to evaluate the usability of our dietary support chatbot
      prototype, we conducted a pilot usability test with three participants.
      The purpose of this testing was to assess the clarity of navigation, task
      flow, risk communication, and overall trust in the system. Since the
      prototype was hand-sketched and low-fidelity, our primary focus was on
      interaction structure and user understanding rather than visual design or
      technical performance.
    </p>
    <p class="font-semibold">Participants:</p>
    <ul class="plist">
      <li>
        Participant #1 is a graduate student at Emory University. The
        participant frequently uses dining services on campus and regularly uses
        mobile apps.
      </li>
      <li>
        Participant #2 is also a graduate student at Emory University. The
        participant has experience using chatbot-based applications and
        demonstrated familiarity with mobile interface patterns.
      </li>
      <li>
        Participant #3 is a working professional. The participant regularly uses
        health and productivity apps and emphasized the importance of clarity,
        trust, and reliability in health-related tools.
      </li>
    </ul>
    <p class="font-semibold">Tasks Evaluated</p>
    <p class="pbody">
      Testing was conducted across three task complexity levels that correspond
      to the structure of the app.
    </p>
    <p class="font-semibold">Simple Task: Quick Food Safety Check</p>
    <p class="pbody">
      Participants were asked to imagine they were unsure whether a pasta dish
      contained gluten and to use the app to verify its safety.
    </p>
    <p class="pbody">This task evaluated:</p>
    <ul class="plist">
      <li>Discoverability of the “Quick Check” feature</li>
      <li>Clarity of the safe/unsafe result</li>
      <li>Understanding of suggested alternatives</li>
    </ul>
    <p class="font-semibold">Medium Task: Context-Aware Recommendation</p>
    <p class="pbody">
      Participants were asked to obtain a meal recommendation based on a dining
      location and dietary needs.
    </p>
    <p class="pbody">This task evaluated:</p>
    <ul class="plist">
      <li>Clarity of guided prompts</li>
      <li>Perceived helpfulness of recommendations</li>
      <li>Cognitive effort required</li>
    </ul>
    <p class="font-semibold">Complex Task: Risk-Sensitive Support</p>
    <p class="pbody">
      Participants were asked to imagine feeling unwell after eating and to use
      the app to seek guidance.
    </p>
    <p class="pbody">This task evaluated:</p>
    <ul class="plist">
      <li>Ability to locate the “Safety Support” feature</li>
      <li>Clarity of structured symptom input</li>
      <li>Emotional reaction to risk-level feedback</li>
      <li>Trust in the specialist (SME) escalation option</li>
    </ul>
    <p class="font-semibold">Procedure and Test Measures</p>
    <p class="pbody">
      User testing was conducted remotely via Zoom. Screens were shared through
      screen sharing, and participants verbally indicated where they would tap
      or interact. Each session lasted approximately 12-15 minutes. The goal was
      to evaluate navigation clarity, task understanding, and trust in the
      system rather than visual design.
    </p>
    <p class="pbody">Usability was assessed using the following measures:</p>
    <ul class="plist">
      <li>Task completion success</li>
      <li>Time to complete each task</li>
      <li>Navigation errors or hesitation points</li>
      <li>Verbal feedback during think-aloud</li>
      <li>Emotional reactions to safety and risk indicators</li>
    </ul>
    <p class="font-semibold">Results</p>
    <p class="pbody">
      Through usability testing, we identified both strengths and areas for
      improvement in our prototype.
    </p>
    <p class="pbody">
      Overall, participants found the three-task structure clear and logical.
      The distinction between Quick Check, Smart Suggest, and Safety Support was
      easy to understand. The Simple Task performed particularly well, as users
      appreciated the immediate safe/unsafe feedback and alternative
      suggestions.
    </p>
    <p class="pbody">
      Participants also responded positively to the presence of the specialist
      option. The professional participant specifically stated that having
      access to human support increased confidence in the system and made the AI
      feel more responsible.
    </p>
    <p class="pbody">
      One insight we gained was that the Medium Task required clearer
      instructions. Some participants hesitated when entering contextual
      information and were unsure how precise their input needed to be. Another
      insight was related to risk communication. When the system displayed “High
      Risk,” one participant expressed mild anxiety and suggested that the app
      should provide calming explanatory text alongside risk labels. Since the
      prototype was paper-based, participants occasionally expected interactive
      behaviors such as scrolling or swiping that were not possible. This
      highlighted the importance of clearly communicating prototype limitations
      before testing.
    </p>
    <p class="pheading">Market Research</p>
    <p class="pbody">
      For the market research, the team found three different apps/websites that
      can serve as either competition that drives GrubAble features to become
      even more differentiating or as partners that GrubAble would benefit from
      collaborating with or for them.
    </p>
    <p class="pbody">
      <span class="font-semibold">
        1. Find Me Gluten Free (FMGF) - Competitor:
      </span> It is a restaurant finder focused on gluten-free dining, built around
      community ratings/reviews and has the function to discover by location. The
      existence and use of FMGF proves real demand for restriction-specific restaurant
      discovery.
    </p>
    <p class="pbody">Grubable's differentiator:</p>
    <ul class="plist">
      <li>
        FMGF tackles only one restriction domain (gluten-free); GrubAble can aim
        to take on a broader problem space, i.e multi-restriction and budget
        constraints.
      </li>
      <li>
        Grubable's anonymous group decision flow is a different use case than
        solo discovery.
      </li>
    </ul>
    <p class="pbody">
      <span class="font-semibold">2. SafeTable - Competitor:</span> It is a restaurant
      guide rated on allergy-friendliness, based on their menus and food offerings.
      It has the feature where you input the name of the restaurant, it finds the
      restaurant, and tells you the rating which is color coded red, green, or yellow.
      It also takes in input from the user regarding various specific types of allergies.
    </p>
    <p class="pbody">
      It is very close conceptually to Grubable's “dietary-compatibility rating”
      but the differentiators are:
    </p>
    <ul class="plist">
      <li>
        GrubAble's anonymous group poll (budget + restrictions → recommendation)
        addresses a completely separate pain point; social discomfort.
      </li>
      <li>
        The app is often dysfunctional and unreliable, it also has no reviews.
        Although it finds the restaurant, it produces no real rating because it
        has to be “verified”. There is no explanation of how this rating is
        done.
      </li>
    </ul>
    <p class="pbody">
      <span class="font-semibold">3. OpenTable - Partner:</span> It is a reservations
      platform with an API ecosystem designed for partners to extend functionality.
    </p>
    <p class="pbody">
      It would be great for Grubable to pair with OpenTable to turn the decision
      or recommendation into a real reservation in a restaurant. It would be
      especially useful for the group feature; after the group decides and
      learns which restrictions they should take into account, OpenTable takes
      over and books the restaurant.
    </p>

    <p class="pheading">Discussion</p>
    <p class="pbody">
      The best word to describe our P3 process is collaborative, extremely
      collaborative. For some team members, the early stages were not the most
      fun or engaging, especially the initial requirement to sit down with pen
      and paper and generate ideas. It was a creative challenge to push past the
      first few obvious concepts and produce as many solutions as possible.
    </p>
    <p class="pbody">
      The process however became far more rewarding as we started to refine and
      combine ideas. Once we began polishing, praising, and giving constructive
      feedback, our discussions gained momentum. Ideas flowed more naturally,
      and our thinking became more concrete.
    </p>
    <p class="pbody">
      The structure and thoroughness of the assignment also helped us narrow our
      scope. It forced us to move from broad concepts to specific features.. At
      the same time, it made it obvious that this is only a first rough
      iteration. Our solution will need continued refinement, revision, and
      likely significant change before it becomes something we believe is
      useful.
    </p>
    <p class="pbody">
      Usability testing reinforced this iterative mindset. Much of the feedback
      pointed to issues we couldn't solve with small tweaks; many require
      returning to the drawing board and rethinking the design. Finally, our
      market research helped validate the problem space: we confirmed that
      people are actively searching for ways to address dietary restrictions
      when eating out. We also found that while parts of our solution overlap
      with existing tools, our core idea - especially the anonymous,
      group-oriented decision support - remains unique and novel. By analyzing
      competitors, we can borrow ideas and also learn from where they went wrong
      as our own idea evolves.
    </p>
  </div>
</div>
