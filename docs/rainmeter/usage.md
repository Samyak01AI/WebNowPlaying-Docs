[Rainmeter]
Update=1000
BackgroundMode=2
SolidColor=0,0,0,255

[MeasureTitle]
Measure=Plugin
Plugin=WebNowPlaying
PlayerType=Title

[MeasureArtist]
Measure=Plugin
Plugin=WebNowPlaying
PlayerType=Artist

[MeasureAlbum]
Measure=Plugin
Plugin=WebNowPlaying
PlayerType=Album

[MeterPrev]
Meter=String
X=5
Y=5
FontColor=FFFF00
Text="Prev"
# The measure to perform the Bang on does not matter,
# it can be any WebNowPlaying measure.
LeftMouseUpAction=[!CommandMeasure "MeasureTitle" "Previous"]

[MeterNext]
Meter=String
X=20R
Y=5
FontColor=FFFF00
Text="Next"
LeftMouseUpAction=[!CommandMeasure "MeasureTitle" "Next"]

[MeterTitle]
Meter=String
MeasureName=MeasureTitle
X=5
Y=35
W=400
H=20
FontColor=255,255,255,255
Text="Title: %1"

[MeterArtist]
Meter=String
MeasureName=MeasureArtist
X=5
Y=55
W=400
H=20
FontColor=255,255,255,255
Text="Artist: %1"

[MeterAlbum]
Meter=String
MeasureName=MeasureAlbum
X=5
Y=75
W=400
H=20
FontColor=255,255,255,255
Text="Album: %1"
