# Custom Dropdown Plugin

This custom dropdown plugin is a jQuery extension designed with flexibility in mind. You can use it to add a dynamic dropdown menu to your project with a user-friendly interface and various features.

Bu özel açılır menü eklentisi, esneklik düşünülerek tasarlanmış bir jQuery uzantısıdır. Kullanıcı dostu bir arayüz ve çeşitli özelliklerle projenize dinamik bir açılır menü eklemek için kullanabilirsiniz.

## Features

- **Search Functionality**: Easily filter options in the dropdown menu with the live search feature.
- **Multiple Selection Support**: Allows for selecting multiple options or a single option.
- **Actions Box**: The actions box enables quick actions like selecting all options or clearing selections.
- **Customizable Texts**: Customize the texts displayed in the dropdown menu as you see fit.

## Özellikler

- **Arama Fonksiyonu**: Canlı arama özelliği ile açılır menüdeki seçenekleri kolayca filtreleyin.
- **Çoklu Seçim Desteği**: Birden fazla seçeneği veya tek bir seçeneği seçmeye olanak tanır.
- **Eylem Kutusu**: Tüm seçenekleri seçme veya seçimleri temizleme gibi hızlı işlemler yapmanıza olanak tanır.
- **Özelleştirilebilir Metinler**: Açılır menüde gösterilen metinleri istediğiniz gibi özelleştirin.

## Usage

1. Add the jQuery library to the `<head>` section of your HTML file:

    ```html
    <script src="https://code.jquery.com/jquery-3.3.1.min.js"></script>
    ```

2. Include the dropdown menu in your project:

    ```html
    <select class="selectpicker" data-count-selected-text="5" data-live-search="true" data-actions-box="true"
            data-text-choose-options="Custom Choose Options"
            data-text-no-results="Custom No Results"
            data-text-deselect-all="Custom Deselect All"
            data-text-select-all="Custom Select All"
            data-text-search="Custom Search..."
            data-text-items-selected="Custom items Selected"
            data-show-selected-image="true"
            multiple>
        <option selected>Example</option>
        <option selected>Ketchup</option>
        <option selected>Relish</option>
        <option selected>Mayonnaise</option>
        <option data-img="https://upload.wikimedia.org/wikipedia/commons/a/ac/Approve_icon.svg" data-img-width="30px" data-img-height="30px">Hot Sauce</option>
        <option>BBQ Sauce</option>
        <option>Soy Sauce</option>
    </select>
    ```

3. Activate your jQuery plugin on the page:

    ```html
    <script>
        $(document).ready(function () {
            $('.selectpicker').customSelect();
        });
    </script>
    ```

4. You can now use your custom dropdown menu!

## Kullanım

1. jQuery kütüphanesini HTML dosyanızın `<head>` bölümüne ekleyin:

    ```html
    <script src="https://code.jquery.com/jquery-3.3.1.min.js"></script>
    ```

2. Projenize açılır menüyü dahil edin:

    ```html
    <select class="selectpicker" data-count-selected-text="5" data-live-search="true" data-actions-box="true"
            data-text-choose-options="Özel Seçenekleri Seçin"
            data-text-no-results="Özel Sonuç Yok"
            data-text-deselect-all="Özel Tümünü Kaldır"
            data-text-select-all="Özel Tümünü Seç"
            data-text-search="Özel Ara..."
            data-text-items-selected="Özel Seçilen Öğeler"
            data-show-selected-image="true"
            multiple>
        <option selected>Örnek</option>
        <option selected>Ketchup</option>
        <option selected>Relish</option>
        <option selected>Mayonez</option>
        <option data-img="https://upload.wikimedia.org/wikipedia/commons/a/ac/Approve_icon.svg" data-img-width="30px" data-img-height="30px">Acı Sos</option>
        <option>BBQ Sosu</option>
        <option>Soya Sosu</option>
    </select>
    ```

3. Sayfada jQuery eklentinizi aktif hale getirin:

    ```html
    <script>
        $(document).ready(function () {
            $('.selectpicker').customSelect();
        });
    </script>
    ```

4. Artık özel açılır menünüzü kullanabilirsiniz!

## Data Attributes

The custom dropdown plugin uses several `data-*` attributes to customize its behavior and appearance. Here are the available attributes and their descriptions:

- **data-count-selected-text**: Displays a custom message when multiple options are selected. You can define how many items to show in the message (e.g., "5 items selected").

- **data-live-search**: Enables or disables the live search feature. Set this to `"true"` to allow users to filter options in real-time as they type in the search box.

- **data-actions-box**: Controls the visibility of the actions box that allows users to perform bulk actions like "Select All" or "Deselect All." Set this to `"true"` to display the actions box.

- **data-text-choose-options**: Custom text displayed in the dropdown when the user is prompted to choose options.

- **data-text-no-results**: Custom message shown in the dropdown when there are no matching results found during a search.

- **data-text-deselect-all**: Text displayed for the "Deselect All" action in the actions box.

- **data-text-select-all**: Text displayed for the "Select All" action in the actions box.

- **data-text-search**: Placeholder text for the search input box.

- **data-text-items-selected**: Custom message displayed when options are selected. You can customize it to reflect the number of selected items (e.g., "2 items selected").

- **data-show-selected-image**: When set to `"true"`, this attribute enables the display of images associated with selected options, if available.

- **data-img**: Specifies the URL of an image to be displayed next to the option in the dropdown.

- **data-img-width**: Defines the width of the image associated with the option (in CSS units, e.g., "30px").

- **data-img-height**: Defines the height of the image associated with the option (in CSS units, e.g., "30px").

## Veri Özellikleri

Özel açılır menü eklentisi, davranışını ve görünümünü özelleştirmek için birkaç `data-*` özniteliği kullanır. İşte mevcut öznitelikler ve açıklamaları:

- **data-count-selected-text**: Birden fazla seçenek seçildiğinde özel bir mesaj görüntüler. Mesajda gösterilecek öğe sayısını tanımlayabilirsiniz (örn. "5 öğe seçildi").

- **data-live-search**: Canlı arama özelliğini etkinleştirir veya devre dışı bırakır. Kullanıcıların arama kutusuna yazarken seçenekleri gerçek zamanlı olarak filtrelemesine izin vermek için `"true"` olarak ayarlayın.

- **data-actions-box**: Kullanıcıların "Tümünü Seç" veya "Tümünü Kaldır" gibi toplu işlemler yapmasını sağlayan eylem kutusunun görünürlüğünü kontrol eder. Eylem kutusunu görüntülemek için `"true"` olarak ayarlayın.

- **data-text-choose-options**: Kullanıcının seçenekleri seçmesi istendiğinde açılır menüde görüntülenen özel metin.

- **data-text-no-results**: Arama sırasında eşleşen sonuç bulunmadığında açılır menüde gösterilen özel mesaj.

- **data-text-deselect-all**: Eylem kutusundaki "Tümünü Kaldır" işlemi için görüntülenen metin.

- **data-text-select-all**: Eylem kutusundaki "Tümünü Seç" işlemi için görüntülenen metin.

- **data-text-search**: Arama giriş kutusu için yer tutucu metin.

- **data-text-items-selected**: Seçenekler seçildiğinde görüntülenen özel mesaj. Seçilen öğe sayısını yansıtacak şekilde özelleştirebilirsiniz (örn. "2 öğe seçildi").

- **data-show-selected-image**: `"true"` olarak ayarlandığında, bu öznitelik, mevcutsa seçili seçeneklerle ilişkili resimlerin görüntülenmesini sağlar.

- **data-img**: Açılır menüdeki seçeneğin yanında görüntülenecek resmin URL'sini belirtir.

- **data-img-width**: Seçenekle ilişkili resmin genişliğini tanımlar (CSS birimlerinde, örn. "30px").

- **data-img-height**: Seçenekle ilişkili resmin yüksekliğini tanımlar (CSS birimlerinde, örn. "30px").

## License

This dropdown menu extension is licensed under the [MIT License](LICENSE).

---

Bu güncellenmiş açıklama, hem İngilizce hem de Türkçe kısımlarda tutarlılığı sağlamak için gözden geçirildi. Başka bir isteğiniz olursa lütfen belirtin!
