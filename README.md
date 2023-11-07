# BerryTube Emote System mk. 3

Backend MySQL/PHP?
(Do we want to store images in the SQL Database as well or in the flat file system?)

* Uses BerryTube login API to share credentials

  * Upon first login to database, creates user entry in local system that refers if user is banned.

    * If not banned then allow login
    * Maybe add a tier to allow only specific users or trusted users ability to submit emotes and/or add emotes without review at will?
  * If user is moderator/admin
    * Allow viewing and modification of all emotes
* User has the ability to submit emotes for review and view a reference sheet of emotes
    * User can submit new emotes, with aliases
    * Users can update emotes they submitted but it has to be re-reviewed before changes will take effect
    * User can delete emotes they have submitted in queue or have already submitted.
    * User may flag emotes for moderation review if it’s suggestive (with an reason specified)
* Mods and admins
    * Can Add Emotes
    * Can update emote aliases (but not change OG names)
    * Can delete emotes

## Impetus:
* Reddit is cracking down on emote subreddits and inactive ones, this behavior can only be more troubling
* This will allow us to bring the emote under first party system instead of relying on third parties.
* Adding emotes to the system is a pain in the ass.
