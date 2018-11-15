# ImageCropper
Multiple image cropper. This project uses https://github.com/fengyuanchen/cropperjs library.
You can add multiple rendition for images. Rendition examples:
```javascript
var renditions = [{ 'ID': 1, 'Title': 'Ana Sayfa Slider,Popup', 'Width': 1000, 'Height': 300 }, { 'ID': 2, 'Title': 'Ana Sayfa Slider Küçük Resim Url', 'Width': 99, 'Height': 65 }, { 'ID': 3, 'Title': 'Detay Sayfası Küçük Resimler', 'Width': 142, 'Height': 82 }, { 'ID': 4, 'Title': 'Tüm Haberler', 'Width': 290, 'Height': 165 }, { 'ID': 5, 'Title': 'Detay Sayfası Ana Resim', 'Width': 750, 'Height': 422 }, { 'ID': 6, 'Title': 'Sağ Menü Haberler', 'Width': 112, 'Height': 64 }, { 'ID': 7, 'Title': 'Kişi Listesi', 'Width': 150, 'Height': 100 }, { 'ID': 8, 'Title': 'Küçük Slider', 'Width': 195, 'Height': 268 }];
```
You can also change template for design it uses bootstrap 3.0 collapse
```javascript
var template = '<div data-toggle="collapse" href="#collapse_{0}" aria-expanded="false" aria-controls="_{0}"><h4>{1}</h4></div><div class="collapse" id="collapse_{0}"><img id="croppedImage_{0}"/><br><input type="button" value="Düzenle" id="edit_{0}" onclick="SetForCropping(\'{3}\',{2})" /><br><input type="button" value="Seçimi Kaydet" id="save_{0}"  onclick="SetCropImage(\'{3}\',{2})"  /><br><input type="button" id="reset_{0}"  value="Seçimi İptal Et" onclick="RestoreCropImage(\'{3}\',{2})"  "/></div><hr>';
```
