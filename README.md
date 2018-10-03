youtube-video
========

Youtube Video Vue Component
## Installation

  `npm install @spacebartech/youtube-video`

## Usage

  ```
  import YoutubeVideo from '@spacebartech/youtube-video'

  props : {
		videoId : {
			type : String
		},
		height : {
			default : 300
		},
		width : {
			default : 500
		}
	}

  youtube-video(
    :height='281',
    :width='500',
    :video-id=youtubeId
  )

  ```

## Tests

  `npm test`
