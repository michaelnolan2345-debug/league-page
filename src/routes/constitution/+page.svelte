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
    
    <h3 class="noUnderscore clickable" onclick={() => goToSection(one)}>Section 1: Roster</h3>
        <h4 class="noUnderscore clickable" onclick={() => goToSection(oneOne)}>1.1 Positional Breakdown</h4>
            <h5 class="noUnderscore clickable" onclick={() => goToSection(oneOneOne)}>1.1.1 Position Maximums</h5>
        <h4 class="noUnderscore clickable" onclick={() => goToSection(oneTwo)}>1.2 Trading</h4>
            <h5 class="noUnderscore clickable" onclick={() => goToSection(oneTwoOne)}>1.2.1 Trade Collusion</h5>
            <h5 class="noUnderscore clickable" onclick={() => goToSection(oneTwoTwo)}>1.2.2 Lending Players Prohibition</h5>
            <h5 class="noUnderscore clickable" onclick={() => goToSection(oneTwoThree)}>1.2.3 Trade Deadline</h5>
            <h5 class="noUnderscore clickable" onclick={() => goToSection(oneTwoFour)}>1.2.4 Trade Restrictions</h5>
            <h5 class="noUnderscore clickable" onclick={() => goToSection(oneTwoFive)}>1.2.5 Veto/Trade Process</h5>
        <h4 class="noUnderscore clickable" onclick={() => goToSection(oneThree)}>1.3 Waiver Wire</h4>
    
    <h3 class="noUnderscore clickable" onclick={() => goToSection(two)}>Section 2: Drafting</h3>
    
        <h4 class="noUnderscore clickable" onclick={() => goToSection(twoOne)}>2.1 Draft Order</h4>
        <h4 class="noUnderscore clickable" onclick={() => goToSection(twoTwo)}>2.2 Rookie Drafts</h4>
        <h4 class="noUnderscore clickable" onclick={() => goToSection(twoThree)}>2.3 Rookie Pay Scale</h4>
    
    
    <h3 class="noUnderscore clickable" onclick={() => goToSection(four)}>Section 3: Postseason</h3>
    
        <h4 class="noUnderscore clickable" onclick={() => goToSection(fourOne)}>3.1 Playoffs</h4>
        <h4 class="noUnderscore clickable" onclick={() => goToSection(fourTwo)}>3.2 Playoff Tiebreakers</h4>

    <h3 class="noUnderscore clickable" onclick={() => goToSection(seven)}>Section 4: League Finances</h3>
    
        <h4 class="noUnderscore clickable" onclick={() => goToSection(sevenOne)}>4.1 League Dues</h4>
        <h4 class="noUnderscore clickable" onclick={() => goToSection(sixTwo)}>4.2 Payout</h4>
    
    
    <hr />
    
    <h2 class="sectionHeading" bind:this={one}>Section 1 Roster Breakdown</h2>
    
    <h3 class="subSectionHeading" bind:this={oneOne}>1.1 Positional Breakdown</h3>
    
    <p>28 Total Players</p>
    
    <p class="underscore">Starters</p>
    <ul>
        <li>QB</li>
        <li>RB</li>
        <li>RB</li>
        <li>WR</li>
        <li>WR</li>
        <li>TE</li>
        <li>FLEX (RB/WR/TE)</li>
        <li>FLEX (RB/WR)</li>
        <li>SUPERFLEX (QB/RB/WR/TE)</li>
    </ul>
    
    <p>13 Bench Spots</p>
    
        <h4 bind:this={oneOneOne}>1.1.1 Position Maximums</h4>
        
        <div class="subBlock">
            <table class="positionMaximums">
                <tbody>
                <tr><td>QB</td><td class="right">6 Players</td></tr>
                <tr><td>RB</td><td class="right">12 Players</td></tr>
                <tr><td>WR</td><td class="right">12 Players</td></tr>
                <tr><td>TE</td><td class="right">6 Players</td></tr>
                </tbody>
            </table>
        </div>


    <h3 class="subSectionHeading" bind:this={oneTwo}>1.2 Trading</h3>
    
    <p>Teams may trade players in any capacity they see fit. In an effort to incentivize trading and add a fun wrinkle to trades, all players acquired by a new team have their current salary set as Year 1 for salary calculations regardless of how many years they were with a previous team.</p>

    <p>An example: Team A drafts God Shammgod with the first pick in the third round (3.01). During week 5 of Team A’s third season with God Shammgod (3$), Team B offers 3 first round picks for him and team A accepts. Team B now has Shammgod’s contract on Year 1 at 3$, meaning it will not trigger the underpaid salary kicker in the offseason because that player will be calculated using the Year 2 calculation.</p>

    <p>Teams may trade draft picks up to two years in advance. Using the 2023 season as an example, this means that the 2023/2024/2025 draft picks are available as tradeable assets.</p>

    <p>If a player on a rookie contract is traded, it will be reverted to a veteran contract upon acquisition.</p>

    <h4 bind:this={oneTwoOne}>1.2.1 Trade Collusion</h4>
    <div class="subBlock">
        <p>If any owners are suspected of accepting bribes/offering bribes to enhance their/another owners team via trade, trading any assets other than fantasy players, draft picks, FAAB $, or otherwise found guilty of engaging in any form of collusion*, all parties involved in the trade will be susceptible to punishment. The punishments will go as followed:</p>
        
        <ul>
            <li>First Offense – Immediate reduction of FAAB budget by 80%</li>
            <li>Second Offense – Immediate freeze on all transaction types for the next 18 weeks of regular season and playoff fantasy football games, including trades and waiver wire bids</li>
            <li>Third Offense – A league meeting of all members not involved in any of the improper trades/activity in question will take place to discuss next steps.</li>
        </ul>

        <p>All trades that are found guilty of collusion, will be reversed/denied. If the trade had affected the outcome of previous games, the results of those games will be revised.  </p>

        <p>*Collusion includes the organizing of veto votes against an acceptable trade.</p>

        <p>The commissioner will err on the side of letting owners manage their teams the way they see fit. Any collusion will need to be clear. The commissioner reserves the right to step in and at the very least assess the thinking of any team involved in a heavily lop-sided trade. </p>
    </div>

    <h4 bind:this={oneTwoTwo}>1.2.2 Lending Players Prohibition</h4>
    <div class="subBlock">
        <p>Any player traded from a team may not be re-acquired via trade within 6 weeks of the original trade. Any teams involved in this behavior will be subject to the aforementioned collusion punishments.</p>
    </div>
    
    <h4 bind:this={oneTwoThree}>1.2.3 Trade Deadline</h4>
    <div class="subBlock">
        <p>The trade deadline will be set for the Saturday of the week 11 games of the NFL season.</p>
    </div>
    
    <h4 bind:this={oneTwoFour}>1.2.4 Trade Restrictions</h4>
    <div class="subBlock">
        <p>You will not be able to trade draft picks that are more than 3 drafts away. For example, during the 2021 season you cannot trade any picks in or after the 2025 draft. You may only trade FAAB $ from the current season.</p>
    </div>
    
    <h4 bind:this={oneTwoFive}>1.2.5 Veto/Trade Process</h4>
    <div class="subBlock">
        <p>A total of 7 veto votes are required to veto a trade. Vetoes are only appropriate in instances of collusion or an egregious mismatch of value (i.e. CMC for a backup kicker). Not liking a trade does not warrant a veto.</p>
    </div>
    
    
    
    <h3 bind:this={oneThree}>1.3 Waiver Wire</h3>
    
    <p>FAAB Waiver wire system. Each team will begin the season with $100. $0 bids are allowed. Bids will process Thursdays and Sundays at 9AM EST.</p>

    <p>FAAB budgets will reset each season in January.</p>
    
    
    <h2 class="sectionHeading" bind:this={two}>Section 2 Drafting</h2>
    
    <h3 bind:this={twoOne}>2.1 Draft Format</h3>
    <p>The Benny Bean Inaugural Draft will be an Auction format draft, including rookies. The winning bid will set the acquired player’s base salary for their team. Starting in Year 2 the league will split the offseason draft into two formats, the Annual Rookie Draft and the Free Agent Auction. The salary at the time of draft will be considered a waiver bid price for the remainder of the year if the player is dropped.</p>

    <h3 bind:this={twoTwo}>2.2 Rookie Drafts</h3>
    <p>The rookie draft will take place after the annual NFL draft and will be a three round traditional draft format. Draft selections will be determined by previous season records. The playoff teams will be reseeded for draft purposes based on results. Draft order will be determined by using the lowest scores based on Perfect lineups (which is calculated by sleeper) for the non-playoff teams and then playoff finish otherwise.</p>
        <ol>
        <li>1.01 - Lowest MAXpf</li>
        <li>1.02 - 2nd Lowest MAXpf</li>
        <li>1.03 - 3rd Lowest MAXpf</li>
        <li>1.04 - 4th lowest MAXpf</li>
        <li>1.05 - 5th lowest MAXpf</li>
        <li>1.06 - 6th lowest MAXpf</li>
        <li>1.07 - 6th place (playoff seeding determines tiebreaker with 5th place)</li>
        <li>1.08 - 5th place (playoff seeding determines tiebreaker with 6th place)</li>
        <li>1.09 - 4th place</li>
        <li>1.10 - 3rd place</li>
        <li>1.11 - 2nd place</li>
        <li>1.12 - 1st place</li>
    </ol>
    
    <h3 bind:this={twoThree}>2.3 Rookie Pay Scale</h3>
    <p>Rookies will be assigned a starting salary following the pay scale below:</p>
    <ol>
    <li>1.01 - 70$<li>
    <li>1.02 - 67$<li>
    <li>1.03 - 64$<li>
    <li>1.04 - 61$<li>
    <li>1.05 - 58$<li>
    <li>1.06 - 55$<li>
    <li>1.07 - 52$<li>
    <li>1.08 - 49$<li>
    <li>1.09 - 46$<li>
    <li>1.10 - 43$<li>
    <li>1.11 - 40$<li>
    <li>1.12 - 37$<li>
    <li>2.01 - 34$<li>
    <li>2.02 - 31$<li>
    <li>2.03 - 28$<li>
    <li>2.04 - 25$<li>
    <li>2.05 - 22$<li>
    <li>2.06 - 19$<li>
    <li>2.07 - 16$<li>
    <li>2.08 - 13$<li>
    <li>2.09 - 10$<li>
    <li>2.10 -  7$<li>
    <li>2.11 -  4$<li>
    <li>2.12 -  1$<li>
    <li>3.01 -  1$<li>
    <li>3.02 -  1$<li>
    <li>3.03 -  1$<li>
    <li>3.04 -  1$<li>
    <li>3.05 -  1$<li>
    <li>3.06 -  1$<li>
    <li>3.07 -  1$<li>
    <li>3.08 -  1$<li>
    <li>3.09 -  1$<li>
    <li>3.10 -  1$<li>
    <li>3.11 -  1$<li>
    <li>3.12 -  1$<li>
     </ol>
    <h2 class="sectionHeading" bind:this={four}>Section 3 Postseason</h2>
    
    <h3 bind:this={fourOne}>3.1 Playoffs</h3>
    <p>At the end of the season 6 teams will make the playoffs. The first round of playoffs will commence in week 15. The top two teams in each division by record and the 2 wild card teams that finish with the most points will receive a playoff berth. The 2 teams that win their division will receive a bye week in the first round of the playoffs. The highest seed in each round gets to choose their opponent from among the remaining teams. Each playoff matchup will only last one week and the winner will advance. Week 18 will not be used.</p>
    
    <h3 bind:this={fourTwo}>3.2 Seeding Tiebreakers</h3>
    <p>Record determines who wins their division and takes 2nd place in a division. From there seeds are determined as follows:</p>

    <ol>
        <li>1 - Conference Champion (higher total points)</li>
        <li>2 - Conference Champion (lower total points)</li>
        <li>3 - Conference Runner-up (higher total points)</li>
        <li>4 - Conference Runner-up (lower total points)</li>
        <li>5 - Wild Card (highest remaining total points)</li>
        <li>6 - Wild Card (highest remaining total points)</li>
    </ol>


    <h2 class="sectionHeading" bind:this={seven}>Section 4 League Finances</h2>
    
    <h3 bind:this={sevenOne}>4.1 League Dues</h3>
    <p>League dues are set at {dues}$.</p>
    
    <h3 bind:this={sevenTwo}>4.2 Payout</h3>
    <p>League payout is structured as follows:</p>
    <ul>
        <li>1st place: {dues * 7}$</li>
        <li>2nd place: {dues * 2.5}$</li>
        <li>3rd place: {dues * 1.5}$</li>
        <li>Regular Season Scoring Leader: {dues}$</li>
    </ul>

</div>
