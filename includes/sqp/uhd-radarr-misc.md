??? abstract "Misc - [CLICK TO EXPAND]"
    | Custom Format                                                                                            | Score                                              | Trash ID                                        |
    | -------------------------------------------------------------------------------------------------------- | -------------------------------------------------: | ----------------------------------------------- |
    | [{{ radarr['cf']['repack-proper']['name'] }}](/Radarr/Radarr-collection-of-custom-formats/#repackproper) | {{ radarr['cf']['repack-proper']['trash_score'] }} | {{ radarr['cf']['repack-proper']['trash_id'] }} |
    | [{{ radarr['cf']['repack2']['name'] }}](/Radarr/Radarr-collection-of-custom-formats/#repack2)            | {{ radarr['cf']['repack2']['trash_score'] }}       | {{ radarr['cf']['repack2']['trash_id'] }}       |
    | [{{ radarr['cf']['x264']['name'] }}](/Radarr/Radarr-collection-of-custom-formats/#x264)                  | :warning: -10000 :warning:                         | {{ radarr['cf']['x264']['trash_id'] }}          |

    !!! warning "Scores marked with a :warning: warning :warning: are different to those used in the main guide"

    ------
    Breakdown and Why

    - `x264` has a score of `-10000` because we only want the HDR/DV versions of the `WEBDL-1080p`
    - if you're only running 1 Radarr, You might want to remove the `x264`CF so you will also get the HD release if there is no UHD version.

    ??? tip "Proper and Repacks - [CLICK TO EXPAND]"

        I also suggest to change the Propers and Repacks settings in Radarr

        `Media Management` => `File Management` to `Do Not Prefer` and use the [Repack/Proper](/Radarr/Radarr-collection-of-custom-formats/#repackproper) Custom Format.

        ![!cf-mm-propers-repacks-disable](/Radarr/images/cf-mm-propers-repacks-disable.png)

        This way you make sure the Custom Formats preferences will be used and not ignored.
