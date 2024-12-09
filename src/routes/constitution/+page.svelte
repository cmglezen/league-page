<script>
    import { dues } from '$lib/utils/helper';
    let one, oneOne, oneOneOne, oneTwo, oneTwoOne, oneTwoTwo, oneTwoThree, oneTwoFour, oneTwoFive, oneThree;
    let two, twoOne, twoTwo, twoThree;
    let three, threeOne;
    let four, fourOne, fourTwo;
    let five, fiveOne;
    let six, sixOne, sixTwo, sixThree;
    let seven, sevenOne, sevenTwo, sevenThree;

    const goToSection = (section) => {
        const top = section.getBoundingClientRect().top + window.pageYOffset;
        window.scrollTo({left: 0, top, behavior: 'smooth'});
    }
</script>

<style>
    .constitution {
        position: relative;
        z-index: 1;
        width: 92%;
        max-width: 800px;
        margin: 8em auto 10em;
    }

    h1 {
        font-size: 2em;
        line-height: 1.2em;
        text-align: center;
        margin: 2em 0 1.5em;
    }

    h2 {
        font-size: 1.5em;
        line-height: 1.2em;
    }

    h3 {
        text-decoration: underline;
        font-size: 1.3em;
        line-height: 1.2em;
    }

    h4 {
        text-decoration: underline;
        margin-left: 2em;
        font-size: 1.2em;
        line-height: 1.2em;
    }

    h5 {
        margin-left: 6em;
        font-size: 0.8em;
        line-height: 1.1em;
    }

    .subBlock {
        margin-left: 2.4em;
    }

    .sectionHeading {
        margin: 4em 0 1.5em;
    }

    .subSectionHeading {
        margin: 1.5em 0 1.5em;
    }

    .underscore {
        text-decoration: underline;
    }

    .right {
        text-align: right;
    }

    .positionMaximums td {
        min-width: 3em;
    }

    .noUnderscore {
        text-decoration: none;
    }

    .clickable {
        cursor: pointer;
    }

    .clickable:hover {
        color: #00316b;
    }

    p {
        color: #777;
    }
</style>

<div class="constitution">
    <h1 class="noUnderscore">LEGENDS LEAGUE CONSTITUTION</h1>
    
    <h2 class="noUnderscore">TABLE OF CONTENTS</h2>
    
    <h3 class="noUnderscore clickable" on:click={() => goToSection(one)}>Section 1: League Structure</h3>
      
    <h3 class="noUnderscore clickable" on:click={() => goToSection(two)}>Section 2: Payouts</h3>
    
  
    <h3 class="noUnderscore clickable" on:click={() => goToSection(three)}>Section 3: Scoring and Roster</h3>
    
    <h3 class="noUnderscore clickable" on:click={() => goToSection(four)}>Section 4: Trades and Waivers</h3>
    
    <h3 class="noUnderscore clickable" on:click={() => goToSection(five)}>Section 5: League Deadlines</h3>
    
        <h4 class="noUnderscore clickable" on:click={() => goToSection(fiveOne)}>5.1 League Tanking Policy</h4>

    <h3 class="noUnderscore clickable" on:click={() => goToSection(six)}>Section 6: Rookie Draft</h3>
    
    <h3 class="noUnderscore clickable" on:click={() => goToSection(seven)}>Section 7: Playoffs</h3>
        
    <hr />
    
    <h2 class="sectionHeading" bind:this={one}>Section 1 League Structure</h2>
    <p>12 Teams</p>
    <p> 26 Roster spots and 2 Injured Reserve Slots</p>
    <p>Starters</p>
    <ul>
        <li>QB</li>
        <li>RB</li>
        <li>RB</li>
        <li>WR</li>
        <li>WR</li>
        <li>WR</li>
        <li>TE</li>
        <li>FLEX (RB/WR/TE)</li>
        <li>FLEX (RB/WR/TE)</li>
        <li>SUPERFLEX (QB/RB/WR/TE)</li>
    </ul>
    
    <p>2 IR Spots (Player must be labeled as IR in the Sleeper App)</p>
 
    <h2 class="sectionHeading" bind:this={two}>Section 2 Payouts</h2>
    
    <p>Entry: $55 per year</p>
    <p>1st Place: $395</p>
    <p>2nd Place: $110</p>
    <p>3rd Place: $55</p>
    <p>Progressive Pot: $100 per year</p>
    <p></p>
    <p>The progressive pot will go to the first team to win back to back championships.  Once that is paid out the pot will start over again. If, for any reason, the league ceases to exist and the progressive pot has not been won the pot will be split between the owners.</p>
    <p>If an owner abandons a team they will not receive any portion of the progressive pot upon their exit and all efforts will be made to replace the abandoned team with a new owner.</p>
    <p></p>
    <p>League Dues will be collected and distributed through leaguesafe.com</p>
       
    <h2 class="sectionHeading" bind:this={three}>Section 3 Scoring and Roster</h2>

    <p>We will be using Sleeper.com/APP and their .5 PPR scoring and roster requirements.  4 points per QB touchdown and -2 per interception.  This is NOT a Tight End premium league. Please refer to the Sleeper website for any details on scoring, tiebreakers, and roster cuts etc.</p>
    <p>You only have control of the players on your roster. If a player retires and you think he might come back a year or two later you have to keep him on your roster to maintain control of that player.</p>
    
    <h2 class="sectionHeading" bind:this={four}>Section 4 Trades and Waivers</h2>
    
    <p>Trade deadline is week 13 and you can trade draft picks up to 2 years in advance. There will be no votes on trades and no trade vetoed unless collusion is obvious.  A perceived unbalanced trade is not evidence of “collusion”. If you feel collusion is obvious, contact the commissioner or co-commissioner.  
        Waivers:  Waivers will be handled by a blind bid FAAB (Free Agency Acquisition Budget) style system.  The budget will be $100 from the opening of the year (May or June) until the end of the fantasy season (Week 17 of the NFL season). There is no minimum to bid, you can bid $0 and after you’ve exhausted your budget all bids will be $0.  The budget will reset to $100 for the next season, no roll over.  Waivers will clear very early Wednesday morning. If you have any questions just ask.  
    </p>

    <h2 class="sectionHeading" bind:this={five}>Section 5 League Deadlines</h2>
    
    <p>League will be shut down from the end of the fantasy playoffs until April 1</p>
    <p>League Dues will be due by April 1</p>
    <p>Assuming all teams are paid and accounted for there will be a rookie draft (4 rounds) in late April, early May following the NFL draft, date to be determined.</p>
    <p>Rosters are allowed to go over the 26 man roster positions to accommodate the players from the rookie draft but must be cut down to 26 before the rookie draft and then before the beginning of the NFL season.</p>
    <h2 class="sectionHeading" bind:this={six}>Section 6 Rookie Draft</h2>
        
    <p>Draft Position:  The rookie draft position of the 6 playoff teams is determined by the results of the playoffs (Champ gets pick 12, runner-up gets pick 11 etc.)  The rookie draft position of the non-playoff teams is determined by the standings at the end of the regular season. The consolation bracket ‘The Toilet Bowl’ will not change your draft position.</p>
    <p>Eligible Players:  All incoming rookies and all available free agents are available to be drafted in the rookie draft.</p>
    <p>Draft Date:  The rookie draft will be held annually approximately one week after the NFL draft.  </p>
    
    <h2 class="sectionHeading" bind:this={seven}>Section 7 Playoffs</h2>
    
    <p>There are no divisions.  The top 6 teams by record make the playoffs with the top two teams earning a first round bye.  The playoffs start on week 15 of the NFL season.  Tiebreakers are pretty standard. Determined by overall points, head to head record and scoring.
    The bottom 6 teams will compete in a Toilet Bowl where each team is trying to avoid losing and being flushed to the next round.  There will be some incentive to not be the Toilet Bowl Turd. For example the last place team gets to be re-named for the next season by the 7th place team or some other form of ridiculous embarrassment… to be determined :)   
    </p>
    
    
</div>
