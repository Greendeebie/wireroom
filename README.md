# Wire Room site

Three static pages. No build step, no dependencies, nothing to install.

    index.html      the landing page
    feeds.html      how to add your first feeds
    privacy.html    the privacy policy
    img/            screenshots

## Putting it online, free

1. Make a **public** repository on GitHub. Any name; `wireroom` is fine.
2. Upload everything in this folder to the root of it.
3. Repository **Settings → Pages**, set Source to *Deploy from a branch*, branch
   `main`, folder `/ (root)`, save.

A minute or two later it is live at `https://<your-username>.github.io/<repo>/`.

That URL is what goes in the Microsoft Store listing's **Support info**, and it is
what the privacy policy page is for - Partner Center currently holds that text pasted
in by hand, which means it can only be changed by resubmitting the listing.

A custom domain is optional and costs about £10 a year. The github.io address works
and ranks perfectly well for a phrase as specific as "split flap display windows".

## The board on the landing page

It is not a video or a GIF. It is the real mechanism in about sixty lines of
JavaScript: the app's own forty-nine position drum, in the app's own order, turning
forwards only at 55ms a flap with 18ms added per cell. A letter is reached by stepping
through every letter between it and the current one, exactly as the app does and
exactly as the mechanical boards do.

That is the reason it is worth having rather than a recording: a visitor who drags
their eye along it watches the wave cross, which is the thing being sold.

It settles, rests for 2.2 seconds, then turns to the next message. Under
`prefers-reduced-motion` it arrives already settled and changes without animating.
