# ae_userstyles

This repository contains visual styling improvement for websites (in the form of CSS overrides in a [UserCSS](https://github.com/openstyles/stylus/wiki/UserCSS) file). 

Currently, there's just one improved styling included: `ae_jira_kanban`, with improvements for Jira Kanban board pages. 

## ae_jira_kanban

Makes the Jira Kanban view more pleasant to use: Increases screen real estate dedicated to displaying cards; does not truncate card titles; and more.

### Installation Instructions

#### 1. Install the Stylus browser extension 

- Firefox: https://addons.mozilla.org/en-US/firefox/addon/styl-us/
- Google Chrome: https://chromewebstore.google.com/detail/stylus/clngdbkpkpeebahjckkjfobafhncgmne 

#### 2. Install the `ae_jira_kanban` style

1. Visit https://userstyles.world/style/15633/ae-jira-kanban 
2. Scroll down on that page a bit, and click the blue Install button. 
3. In the Stylus extension page that opens, click the Install Style button (near the top-left corner).

Now, browse to your Jira Kanban board, and enjoy the improvements!

### Notes

This add-on is dependent on what are evidently machine-generated CSS class names used by Atlassian on Jira Kanban board pages. Therefore, styles may break from time to time when Atlassian pushes a UI update.

(Historically, this does appear to be a fairly infrequent occurrence; on the order of once every few months, as of April 2024.)

When this happens, ideally, someone will push an update to this repository with fixes in reasonably short order! 

After that's been done, your Stylus extension should automatically obtain and apply the updates from the [userstyles.world mirror](https://userstyles.world/style/15633/ae-jira-kanban) -- no need for you to take any manual action!

### Specific Improvements (as of v1.0.8)

- Card titles are no longer truncated!
- Removes on-hover card title tool tips. (No longer needed now that titles aren't truncated!)
- Also removes on-hover tool tips for card Epic labels, and card IDs. 
- Uses the full card width when displaying card titles.
- Moves each card's `...` on-hover button to the bottom-center (to reduce obscuring of other card elements).
- Hides the drag-drop column overlays (introduced ~June 2025) that obscure the ordering position in the destination column.
- Slightly increases card and column width.
- Reduces unneeded vertical whitespace in the top header portion of the board.
- Increases the column header font size.
- Slightly reduces vertical whitespace in the column header row.
- Replaces the default green "Task" card type icon (which looks very similar to the green "Story" card type icon) with an orange square icon.
- Displays due dates in red.

### How To Contribute

_Note: At the current time, contributions are only accepted from AppFolio employees._

To publish a new version of the `ae_jira_kanban` styles:

1. As you would normally when doing development, clone this repository (if you haven't already), and create a new git branch
2. Make your changes (including appropriate comments, please!) to `ae_jira_kanban.user.css`, commit, and push.
    - Be sure to increment the `@version` number in the `UserStyle` headers at the top of the file (using typical [semantic versioning](https://semver.org/) practices); otherwise, the changes won't be automatically picked up by the [userstyles.world mirror](https://userstyles.world/style/15633/ae-jira-kanban), and automatically distributed to users.
3. Create a pull request for your branch, and have it reviewed and QA'ed by someone on your team, in the usual fashion.
4. Merge the pull request.

The updates will automatically be picked up by the userstyles.world mirror. (userstyles.world checks for changes every 4 hours, starting daily at 00:04 UTC. [See details](https://userstyles.world/docs/faq#how-does-mirroring-source-code-work).)

The Stylus browser extension periodically checks for, and applies, updates from the userstyles.world mirror (for users who originally installed from there). 

### Uninstallation Instructions

1. Browse to your Jira Kanban board. 
2. In the Stylus extensions settings, uncheck the `ae_jira_kanban` style.

(Tip: You can also uncheck and re-check `ae_jira_kanban` repeatedly, to observe the changes that the updated styles are making to your Jira Kanban board!)

Alternatively (if you aren't using it for anything else): Just disable or uninstall the Stylus extension from your browser.

### Special Thanks

- Julie DeMello, for contributing some of the original CSS!
- Seth VanBrocklin and Dean Johnson, for contributing to the project launch!
- AppFolio leadership, for continuing to sponsor Hack Days and Impact Fridays, without which this project would not exist!
