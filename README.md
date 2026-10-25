# Portfolio content

Published JSON and optimized images for the GitHub-backed Portfolio CMS. The application reads `content/site.json`, the category/technology registries, and one document per project in `content/projects/`. Images use repository-relative paths under `media/`.

## Migration — 25 October 2026

The previous complete `master` tree is preserved on [legacy](https://github.com/ervin-sungkono/web-assets/tree/legacy) at commit `3a62ce04163dfdc8d6e328df385ba538762555b9`. The old `data/` JSON has moved to that branch. Existing `images/` and `icons/` files remain unchanged on `master` as compatibility assets until the application has cut over; do not remove them before verifying all existing URLs.

The conversion preserved 17 public project slugs, centralized taxonomy, and generated 25 optimized raster images, including the Frontend Mentor gallery. Validation reported no missing metadata, invalid references, or errors. Project years use verified GitHub repository creation timestamps as proxies because the legacy JSON did not contain years. Legacy SVG icons remain available at their old URLs; the new technology registry keeps labels without importing those icons.

| Previous JSON | CMS slug |
| --- | --- |
| `744526407.json` | `wetrack-app` |
| `647812745.json` | `chatgpt-clone` |
| `583715585.json` | `next-pokedex` |
| `626356347.json` | `frontendmentor-io` |
| `548464131.json` | `easy-trip` |
| `526852146.json` | `kita-peduli` |
| `592381448.json` | `discord-music-bot` |
| `566667418.json` | `inventory-management-app` |
| `858016238.json` | `qr-code-gen` |
| `518750261.json` | `css-box-shadow-generator` |
| `541891916.json` | `todo-app` |
| `517544061.json` | `clock-app` |
| `518089178.json` | `weather-forecast-app` |
| `519540760.json` | `dnd-multiplication-game` |
| `620749427.json` | `simple-youtube-clone` |
| `522490482.json` | `javascript-2d-chess` |
| `558204741.json` | `android-calculator-app` |

`frontendmentor.json` was retained as challenge details in the migration report and eight gallery images under the established `frontendmentor-io` project. No additional public slugs were invented.

## Rollback and operations

Revert the migration commit to restore the old `master` tree, or use the preserved `legacy` branch as the previous reader source. Preserve `legacy` and the compatibility assets until application, routes, and hosted media have been verified. Keep this content repository separate from the application's deployment source; ordinary content commits should invalidate ISR rather than deploy the application.

All committed content, including unpublished projects and history, is public. CMS writes use `Portfolio CMS <cms@portfolio.local>` as both Git author and committer; keep that email unassociated with the owner's GitHub account.
