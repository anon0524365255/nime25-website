---
#
# By default, content added below the "---" mark will appear in the home page
# between the top bar and the list of recent posts.
# To change the home page layout, edit the _layouts/home.html file.
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
#
layout: post
title: "Designing Percussive Timbre Remappings: Negotiating Audio Representations and Evolving Parameter Spaces"
---

<style>
  .audio-switch-wrapper {
    padding-top: 10px;
    width: 100%;
  }
  .audio-switch-inner {
    display: flex;
    justify-content: center;
    align-items: center;
  }
</style>

Website accompanying the NIME 2025 submission.

## Annotated Portfolio

An annotated portfolio brings together a collection of individual
artefacts with annotations that help to illuminate design thinking and capture similarities
and differences amongst artefacts. They serve to present material that was
created in a particular design context while drawing out important features that may be
interesting in a broader research context. "Annotated portfolios are, perhaps, a way of
modestly reaching out beyond the particular without losing grounding" [(Gaver & Bowers, 2012)](#references).

Here, we present a set of eight patches that were created during an in-studio session.
Videos of short performance recordings are provided for each
patch, which are annotated with reflections on design thinking and motivations. 
We used the real-time timbre remapping system presented in the paper and each patch 
either exemplifies a feature of the system or presents an intervention applied to overcome
a limitation or achieve an aesthetic goal.

### Derailer

<div style="position: relative; padding-top: 10px%;">
  <video
    id="derailer-video"
    class="video-js"
    controls
    preload="auto"
    data-setup="{}"
  >
    <source src="https://customer-c3u274buzk2jtvrk.cloudflarestream.com/6335d39f2e7e0510f266f6104c1e19e7/manifest/video.m3u8" type="application/x-mpegURL" />
    <p class="vjs-no-js">
      To view this video please enable JavaScript, and consider upgrading to a
      web browser that
      <a href="https://videojs.com/html5-video-support/" target="_blank"
        >supports HTML5 video</a
      >
    </p>
  </video>

<div class="audio-switch-wrapper">
  <div class="audio-switch-inner">
    <div class="btn-group audio-switch" data-toggle="buttons" video-id="derailer-video">
        <label class="btn btn-outline-secondary">
            <input type="radio" class="btn-check" name="options" value="mixed" autocomplete="off" checked> Mixed
        </label>
        <label class="btn btn-outline-secondary">
            <input type="radio" class="btn-check" name="options" value="drum" autocomplete="off"> Drum Only
        </label>
        <label class="btn btn-outline-secondary">
            <input type="radio" class="btn-check" name="options" value="synth" autocomplete="off"> Synth Only
        </label>
    </div>
  </div>
</div>

</div>

#### Patch Notes
This patch varied the MIDI note being triggered on inference based on the spectral centroid of the real time audio analysis (256 sample window). The spectral centroid was scaled down to a smaller range of the available MIDI notes, then was split into two registers corresponding with the head of the drum and the cowbell, and each register was quantized to a fixed key and scale.

#### Reflections
The long resonance of Derailer and the somewhat polyphonic nature of playback worked well with separating the two playing surfaces out into different registers. The idea here was to have a kind of "bass line" underneath a flurry of melodic pitches somewhat inspired by handpan instruments.

### Modular Synthesizer

<div style="position: relative; padding-top: 10px%;">
  <video
    id="modular-video"
    class="video-js"
    controls
    preload="auto"
    width="750"
    height="300"
    data-setup="{}"
  >
    <source src="https://customer-c3u274buzk2jtvrk.cloudflarestream.com/2f3852ef48effbace9eddb7b0b618a4e/manifest/video.m3u8" type="application/x-mpegURL" />
    <p class="vjs-no-js">
      To view this video please enable JavaScript, and consider upgrading to a
      web browser that
      <a href="https://videojs.com/html5-video-support/" target="_blank"
        >supports HTML5 video</a
      >
    </p>
  </video>

<div class="audio-switch-wrapper">
  <div class="audio-switch-inner">
    <div class="btn-group audio-switch" data-toggle="buttons" video-id="modular-video">
        <label class="btn btn-outline-secondary">
            <input type="radio" class="btn-check" name="options" value="mixed" autocomplete="off" checked> Mixed
        </label>
        <label class="btn btn-outline-secondary">
            <input type="radio" class="btn-check" name="options" value="drum" autocomplete="off"> Drum Only
        </label>
        <label class="btn btn-outline-secondary">
            <input type="radio" class="btn-check" name="options" value="synth" autocomplete="off"> Synth Only
        </label>
    </div>
  </div>
</div>

</div>

#### Patch Notes
This patch uses the timbre remapping approach as presented in the paper applied to a Eurorack 
modular synthesizer patch. Six parameters are included for modulations and are controlled
via CV from an [Expert Sleepers ES-8](https://www.expert-sleepers.co.uk/es8.html).
Parameters include FM controls, wavetable position, envelope attack/deday time, filter resonance.

#### Reflections
There was a palpable fragility to the mapping here where tiny changes in dynamics led to very wide timbral changes on the synth. This led to a more subtle and subdued language that tried to navigate some subtle nuances in the notes. As a contrast, some faster passages were useful to show the melodic capabilities of this mapping and setup.

### 808 Snare

<div style="position: relative; padding-top: 10px%;">
  <video
    id="808snare-video"
    class="video-js"
    controls
    preload="auto"
    width="750"
    height="300"
    data-setup="{}"
  >
    <source src="https://customer-c3u274buzk2jtvrk.cloudflarestream.com/3c3f5e79c2a46f6ecceed811ab790f07/manifest/video.m3u8" type="application/x-mpegURL" />
    <p class="vjs-no-js">
      To view this video please enable JavaScript, and consider upgrading to a
      web browser that
      <a href="https://videojs.com/html5-video-support/" target="_blank"
        >supports HTML5 video</a
      >
    </p>
  </video>

<div class="audio-switch-wrapper">
  <div class="audio-switch-inner">
    <div class="btn-group audio-switch" data-toggle="buttons" video-id="808snare-video">
        <label class="btn btn-outline-secondary">
            <input type="radio" class="btn-check" name="options" value="mixed" autocomplete="off" checked> Mixed
        </label>
        <label class="btn btn-outline-secondary">
            <input type="radio" class="btn-check" name="options" value="drum" autocomplete="off"> Drum Only
        </label>
        <label class="btn btn-outline-secondary">
            <input type="radio" class="btn-check" name="options" value="synth" autocomplete="off"> Synth Only
        </label>
    </div>
  </div>
</div>

</div>

#### Patch Notes
This patch used mapping generated by the genetic algorithm crawl, but was then modified for playback by removing the modulation of one of the oscillators to limit the variability of the snare "tone", keeping it more in line with conventional uses of an 808 snare.

#### Reflections
Using the patch with the reduced pitch mapping felt much more like an 808 snare would in the context of a backbeat. To highlight this, a more conventional backbeat with "cowbell" accents demonstrates the nuance available in the core 808 hits based on the dynamic and timbral variation of the input sounds.

### Loudness Compensation

<div style="position: relative; padding-top: 10px%;">
  <video
    id="loudness-video"
    class="video-js"
    controls
    preload="auto"
    width="750"
    height="300"
    data-setup="{}"
  >
    <source src="https://customer-c3u274buzk2jtvrk.cloudflarestream.com/283f4f5728096cf913e3b2ef93b5e34e/manifest/video.m3u8" type="application/x-mpegURL" />
    <p class="vjs-no-js">
      To view this video please enable JavaScript, and consider upgrading to a
      web browser that
      <a href="https://videojs.com/html5-video-support/" target="_blank"
        >supports HTML5 video</a
      >
    </p>
  </video>

<div class="audio-switch-wrapper">
  <div class="audio-switch-inner">
    <div class="btn-group audio-switch" data-toggle="buttons" video-id="loudness-video">
        <label class="btn btn-outline-secondary">
            <input type="radio" class="btn-check" name="options" value="mixed" autocomplete="off" checked> Mixed
        </label>
        <label class="btn btn-outline-secondary">
            <input type="radio" class="btn-check" name="options" value="drum" autocomplete="off"> Drum Only
        </label>
        <label class="btn btn-outline-secondary">
            <input type="radio" class="btn-check" name="options" value="synth" autocomplete="off"> Synth Only
        </label>
    </div>
  </div>
</div>

</div>

#### Patch Notes
This patch used a noisier Quantussy mapping as the basis, and was chosen for it's acoustic snare-like qualities. To add additional variance the loudness of the matched preset was compensated for by computing the difference between the preset and the realtime audio, such that it closely followed the performance dynamic.

#### Reflections
Although this example is simply a demonstration of the impact of loudness compensation, the overall expressiveness enabled by loudness compensation is something that was applied to nearly every example. Even though loudness is directly encoded in some descriptor types (i.e. hybrid descriptors and melbands) and implicitely in the others via just variations in synthesis parameters, directly compensating for additional dynamic variance feels significantly more organic than with it being disabled.

### Classification + Parallel Timbre Remapping

<div style="position: relative; padding-top: 10px%;">
  <video
    id="classification-video"
    class="video-js"
    controls
    preload="auto"
    width="750"
    height="300"
    data-setup="{}"
  >
    <source src="https://customer-c3u274buzk2jtvrk.cloudflarestream.com/f3719e3657477017c34fc9f34852e281/manifest/video.m3u8" type="application/x-mpegURL" />
    <p class="vjs-no-js">
      To view this video please enable JavaScript, and consider upgrading to a
      web browser that
      <a href="https://videojs.com/html5-video-support/" target="_blank"
        >supports HTML5 video</a
      >
    </p>
  </video>

<div class="audio-switch-wrapper">
  <div class="audio-switch-inner">
    <div class="btn-group audio-switch" data-toggle="buttons" video-id="classification-video">
        <label class="btn btn-outline-secondary">
            <input type="radio" class="btn-check" name="options" value="mixed" autocomplete="off" checked> Mixed
        </label>
        <label class="btn btn-outline-secondary">
            <input type="radio" class="btn-check" name="options" value="drum" autocomplete="off"> Drum Only
        </label>
        <label class="btn btn-outline-secondary">
            <input type="radio" class="btn-check" name="options" value="synth" autocomplete="off"> Synth Only
        </label>
    </div>
  </div>
</div>

</div>

#### Patch Notes
This patch is built from two parallel mappings on the Quantussy synthesizer which are routed to at inference from a classifier trained on examples of hits on the head and on the rim of the drum. The loudness of the realtime audio input is additionally mapped to the duration of the low-pass gate that the genetic algorithm cralwed through. The additional layer of a one-to-one mapping (loudness->duration) adds morphological variety to the timbral range of the inference.

#### Reflections
Having two clear presets opened up some performance possibilities where inter and intra modulations were more distinct and "playable" in the instrument. The additional mapping of loudness to duration allowed for some very fast gestures and rolls while still retaining clear articulation with the quieter and shorter sounds.

### Multiple Timescale Morphing

<div style="position: relative; padding-top: 10px%;">
  <video
    id="adsr-video"
    class="video-js"
    controls
    preload="auto"
    width="750"
    height="300"
    data-setup="{}"
  >
    <source src="https://customer-c3u274buzk2jtvrk.cloudflarestream.com/b227a5c067c24e021dca80e506d96494/manifest/video.m3u8" type="application/x-mpegURL" />
    <p class="vjs-no-js">
      To view this video please enable JavaScript, and consider upgrading to a
      web browser that
      <a href="https://videojs.com/html5-video-support/" target="_blank"
        >supports HTML5 video</a
      >
    </p>
  </video>

<div class="audio-switch-wrapper">
  <div class="audio-switch-inner">
    <div class="btn-group audio-switch" data-toggle="buttons" video-id="adsr-video">
        <label class="btn btn-outline-secondary">
            <input type="radio" class="btn-check" name="options" value="mixed" autocomplete="off" checked> Mixed
        </label>
        <label class="btn btn-outline-secondary">
            <input type="radio" class="btn-check" name="options" value="drum" autocomplete="off"> Drum Only
        </label>
        <label class="btn btn-outline-secondary">
            <input type="radio" class="btn-check" name="options" value="synth" autocomplete="off"> Synth Only
        </label>
    </div>
  </div>
</div>

</div>

#### Patch Notes
This patch uses three different mappings, each generated from the same anchor preset on the Quantussy synthesizer, but focussing on a different timeframe for each (256, 4410, and 11025 samples respectively). The idea was to capture the morphology of the synthesizer and then map to that with the timescale regression. The presets are then morphed through at the time of inference based on the morphology of the original synthesizer sound. The interface also allowed for transforming and distorting the preset interpolation in a manner similar to an ADR envelope in conventional synthesis topologies. During inference loudness and spectral centroid were also mapped to the interpolation/timbral morphology duration (making it shorter or longer overall) as well as adjusting the attack and release of the ADSR being applied to the Quantussy output.

#### Reflections
This combination of processes, incorporating multiple timescales of feature mappings and realtime analysis, via timescale regression, and additional layers of morpholigical mappings based on realtime descriptor analysis felt the most expressive and dynamic of all the mappings. The nuance and variability afforded by the layers of mappings created a responsive and expressive instrument in terms of timbral, morphololgical, and dynamic playability. Much like in the classification example, the direct control of duration also enabled incredibly fast gestures without any loss in clarity.

### Latent Feature Control

<div style="position: relative; padding-top: 10px%;">
  <video
    id="latent-video"
    class="video-js"
    controls
    preload="auto"
    width="750"
    height="300"
    data-setup="{}"
  >
    <source src="https://customer-c3u274buzk2jtvrk.cloudflarestream.com/d09b602ef4f5b005b57c1c3d3ce5bd05/manifest/video.m3u8" type="application/x-mpegURL" />
    <p class="vjs-no-js">
      To view this video please enable JavaScript, and consider upgrading to a
      web browser that
      <a href="https://videojs.com/html5-video-support/" target="_blank"
        >supports HTML5 video</a
      >
    </p>
  </video>

<div class="audio-switch-wrapper">
  <div class="audio-switch-inner">
    <div class="btn-group audio-switch" data-toggle="buttons" video-id="latent-video">
        <label class="btn btn-outline-secondary">
            <input type="radio" class="btn-check" name="options" value="mixed" autocomplete="off" checked> Mixed
        </label>
        <label class="btn btn-outline-secondary">
            <input type="radio" class="btn-check" name="options" value="drum" autocomplete="off"> Drum Only
        </label>
        <label class="btn btn-outline-secondary">
            <input type="radio" class="btn-check" name="options" value="synth" autocomplete="off"> Synth Only
        </label>
    </div>
  </div>
</div>

</div>

#### Patch Notes
This patch uses the same set of mappings as the timescale morphing example, and on the same Quantussy synthesizer, but makes explicit use of the "latent" manipulation of the feature differences in the anchor used to compute the nearest matching preset. The top slider adjusts the range and offset of spectral centroid, spectral skewness, and rolloffpercent low. The second slider adjusts the range and offset of spectral spread.

#### Reflections
Although this example is simply a demonstration of the "latent" space scaling, this kind of adjustment and fine-tuning was profoundly helpful when evaluating the expressivity of any given mapping. There were many examples where the preset encoded the timbral difference well but the resultant mapping felt "too bright" or "too harsh". Being able to manipulate and scale the "latent" space this way made these kinds of presets still useful and expressive.

### Multiple Timescale + Multiple Feature Morphing

<div style="position: relative; padding-top: 10px%;">
  <video
    id="adsr-multi-video"
    class="video-js"
    controls
    preload="auto"
    width="750"
    height="300"
    data-setup="{}"
  >
    <source src="https://customer-c3u274buzk2jtvrk.cloudflarestream.com/14ad410701306621bea2c20d38295c23/manifest/video.m3u8" type="application/x-mpegURL" />
    <p class="vjs-no-js">
      To view this video please enable JavaScript, and consider upgrading to a
      web browser that
      <a href="https://videojs.com/html5-video-support/" target="_blank"
        >supports HTML5 video</a
      >
    </p>
  </video>

<div class="audio-switch-wrapper">
  <div class="audio-switch-inner">
    <div class="btn-group audio-switch" data-toggle="buttons" video-id="adsr-multi-video">
        <label class="btn btn-outline-secondary">
            <input type="radio" class="btn-check" name="options" value="mixed" autocomplete="off" checked> Mixed
        </label>
        <label class="btn btn-outline-secondary">
            <input type="radio" class="btn-check" name="options" value="drum" autocomplete="off"> Drum Only
        </label>
        <label class="btn btn-outline-secondary">
            <input type="radio" class="btn-check" name="options" value="synth" autocomplete="off"> Synth Only
        </label>
    </div>
  </div>
</div>

</div>

#### Patch Notes
This patch is similar to the timescale morphing example, using a Quantussy synthesizer, but uses different feature types for each temporal slice of the preset. This allowed using features that were more tailored to different areas of the sound, for example using MFCCs to capture the transient phase of the synthezied sound (256 samples), due to its ability to encode complex timbral variety. This patch also made use of the loudness and spectral centroid mappings tied to playback morphology and some "latent" feature manipulation to shift the overall voicing of the presets.

#### Reflections
Much like in the Timescale Morphing preset, this complex and multidimensional mapping schema creates an expressive instrument with clear detail and articulation for the different types of sounds coming from the muffled drum, rim, and cowbell.


## References

Gaver, B., & Bowers, J. (2012). Annotated portfolios. Interactions, 19(4), 40–49. [doi.org/10.1145/2212877.2212889](https://doi.org/10.1145/2212877.2212889)




<script>
    let selected = "btn-secondary";
    let deselected = "btn-outline-secondary";
    let audioTracks = {};

    jQuery("document").ready(function() {
        
        jQuery("video").each(function() {
          var  player = videojs(this);
          player.fluid(true);
          audioTracks[player.id()] = {};

          player.on("loadeddata", function() {
            const tracks = this.audioTracks();
            for (var i = 0; i < tracks.length; i++)
            {
              var track = tracks[i];
              if (track.label === "original") {
                track.enabled = true;
                track.label = "mixed";
                audioTracks[this.id()]["mixed"] = track;
              } else if (track.label === "synth") {
                track.enabled = false;
                audioTracks[this.id()]["synth"] = track;
              } else if (track.label === "drum") {
                track.enabled = false;
                audioTracks[this.id()]["drum"] = track;
              }
            }
          })
        });


        jQuery(".audio-switch").each(function() {
            var videoId = jQuery(this).attr("video-id");

            jQuery(this).find("input").each(function() {
                var button = jQuery(this);
                var checked = button.attr("checked");
                var label = button.parent();
                if (typeof checked !== 'undefined' && checked !== false) {
                    label.removeClass(deselected);
                    label.addClass(selected);
                } else {
                    label.removeClass(selected);
                    label.addClass(deselected);
                }
                button.click(function() {
                    let mix = button.attr("value");
                    switchAudio(videoId, mix);

                    jQuery(this).parent().siblings().removeClass(selected).addClass(deselected);
                    label.addClass(selected);
                    label.removeClass(deselected);
                });
            });
        });
    });


    function switchAudio(videoId, mix) {
        var player = videojs(videoId);
        var tracks = player.audioTracks();
        console.log(audioTracks);
        if (tracks.length > 1) {
          for (let i = 0; i < tracks.length; i++) {
            tracks[i].enabled = false;
          }
          audioTracks[videoId][mix].enabled = true;
          
          // audioTracks[videoId][mix].enabled = true;
            // if (mix === "mix") {
            //     tracks[0].enabled = true;
            // } else if (mix === "drum") {
            //     tracks[1].enabled = true;
            // } else if (mix === "synth") {
            //     tracks[2].enabled = true;
            // }
        } else {
            console.log("Only one video track");
        }
    };
</script>

<script src="https://vjs.zencdn.net/8.16.1/video.min.js"></script>