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
3. In the Stylus extension page that opens, click the Install Style button (near the top-left corner.)
4. Visit your Jira Kanban board, and enjoy the improvements!

### Notes

This add-on is dependant on what are evidently machine-generated CSS class names used by Atlassian on Jira Kanban board pages. Therefore, styles may break from time to time when Atlassian pushes a UI update.

(Historically, this does appear to be a fairly infrequent occurrence; on the order of once every few months, as of April 2024.)

When this happens, ideally, someone will push an update to this repository with fixes in reasonably short order! 

After that's been done, your Stylus extension should automatically obtain and apply the updates from the [userstyles.world mirror](https://userstyles.world/style/15633/ae-jira-kanban).

### Specific Improvements (as of v1.0.1)

- No longer truncates card titles
- Removes on-hover card title tool tips. (No longer needed now that titles aren't truncated!)
- Use full card with when displaying card titles
- Move the card "..." on-hover button to the bottom-left corner (to avoid obscuring card titles)
- Slightly increases card and column width
- Reduces unneeded vertical whitespace in the top header portion of the board
- Increases the column header font size
- Slightly reduces whitespace used by the column header row
- Replaces the default green "Task" card type icon (which looks very similar to the green "Story" card type icon) with an orange square icon
- Displays due dates in red

### Uninstallation Instructions

1. Browse to your Jira Kanban board. 
2. In the Stylus extensions settings, uncheck the `ae_jira_kanban` style.

Alternatively (if you aren't using it for anything else): Just disable or uninstall the Stylus extension from your browser.
