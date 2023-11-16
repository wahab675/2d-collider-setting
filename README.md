# 2d-collider-setting
void SetScreenColliders()
 {
     float aspect = (float)Screen.width / Screen.height;
     float worldHeight = MainCam.orthographicSize * 2;
     float worldWidth = worldHeight * aspect;
     LeftScreenCollider.transform.position = new Vector3((-worldWidth-1f) / 2f, 0, 0);
     RightScreenCollider.transform.position = new Vector3((worldWidth+1f)/ 2f, 0, 0);
 }
