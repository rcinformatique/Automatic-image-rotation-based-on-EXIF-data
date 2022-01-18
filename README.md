# Automatic-image-rotation-based-on-EXIF-data
La bibliothèque fait pivoter automatiquement l'image fournie en fonction des données EXIF ​​intégrées.  

Exemple d'utilisation:

$imageinfo = $this->upload->data();  
$full_path = $imageinfo['full_path'];

// vérification des données EXIF et fait une rotation automatique si nécessaire  
$this->load->library('image_autorotate', array('filepath' => $full_path));
