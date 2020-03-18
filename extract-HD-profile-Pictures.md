# Extract HD profile Pictures

1. Find User-ID in one of the transmitted JSON (I am open for additions how to find this more easily than just going through the different JSON and trying to find the appropriate User with it's ID)
2. Request the image-Info (not sure if it's just the profile picture or all public pictures) from `https://i.instagram.com/api/v1/users/{user_id}/info/` using the Instagram App User-Agent-String `Mozilla/5.0 (Linux; Android 8.1.0; motorola one Build/OPKS28.63-18-3; wv) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/70.0.3538.80 Mobile Safari/537.36 Instagram 72.0.0.21.98 Android (27/8.1.0; 320dpi; 720x1362; motorola; motorola one; deen_sprout; qcom; pt_BR; 132081645)` 
3. Find `hd_profile_pic_url_info` in the received JSON and use the URL listed there to access the full-resolution Picture
