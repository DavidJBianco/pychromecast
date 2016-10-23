This is a fork of https://github.com/balloob/pychromecast.
It is a POC of a working YouTube controller that uses the Youtube Queue.
**This is still work in progress**

How to use
----------

.. code:: python

    import pychromecast           
    from pychromecast.controllers.youtube import YouTubeController 
    cast = pychromecast.get_chromecast('ChtromeCast_name')
    yt = YouTubeController()
    cast.register_handler(yt)
    yt.play_video('video_id')
    
    # After video loads
    
    # Controll player
    yt.pause()
    yt.play()
    
    # Manage the playlist
    yt.add_to_queue('video_id')
    yt.clear_playlist()
    
    # Check media status
    yt.status.player_is_playing
    yt.status
    

    
