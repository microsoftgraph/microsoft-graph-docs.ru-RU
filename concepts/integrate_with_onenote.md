# <a name="use-microsoft-graph-to-integrate-with-onenote"></a>Интеграция с OneNote при помощи Microsoft Graph

Путем интеграции приложений с OneNote вы можете создавать функциональные интерфейсы на различных платформах, доступных миллионам пользователей по всему миру. С помощью Microsoft Graph вы можете получать доступ к записным книжкам, разделам и страницам в OneNote для создания решений, помогающих пользователям планировать и упорядочивать идеи и сведения.

## <a name="why-create-onenote-apps"></a>Зачем создавать приложения OneNote?

С помощью Microsoft Graph можно создавать заметки, списки, изображения, файлы и другие элементы записных книжек OneNote, а также управлять ими.

### <a name="collect-and-organize-notes-and-ideas"></a>Сбор и упорядочение заметок и идей  
OneNote можно использовать как холст, где пользователи будут добавлять и упорядочивать содержимое. Microsoft Graph упрощает создание приложений, с помощью которых можно делать учебные заметки и проводить исследования, делиться планами и идеями с родными и близкими, а также обмениваться фотографиями покупок. Приложение может собирать нужные пользователям сведения, отправлять их в OneNote и помогать упорядочивать их.

### <a name="capture-information-in-many-formats"></a>Запись данных во множестве форматов
Записывайте HTML-код, внедряйте изображения (с локального компьютера или общедоступного URL-адреса), видео, звуковые файлы, электронные сообщения и другие файлы распространенных типов. В OneNote даже могут отображаться веб-страницы и PDF-файлы в виде моментальных снимков. Microsoft Graph поддерживает набор стандартных тегов HTML и CSS для разметки страниц OneNote, позволяющий создавать нужное оформление с помощью таблиц, встроенных рисунков и базового форматирования. 

### <a name="use-the-onenote-ecosystem-to-enhance-your-core-scenarios"></a>Расширение основных сценариев с помощью экосистемы OneNote
Воспользуйтесь широкими возможностями OneNote. API OneNote в Microsoft Graph выполняют распознавание текста с изображений, поддерживают полнотекстовый поиск, автоматически синхронизируют клиенты, обрабатывают изображения, а также извлекают записанные визитные карточки, описания продукции и рецепты из Интернета. Вы можете использовать OneNote в качестве цифрового хранилища в облаке для заметок и небольших файлов мультимедиа, а также в качестве канала для данных, относящихся к определенным доменам. 

### <a name="reach-millions-of-onenote-users-on-all-major-platforms"></a>Доступ для миллионов пользователей OneNote на всех основных платформах
С помощью OneNote вы можете сделать свое приложение более популярным. Приложение OneNote предустановлено на новых устройствах с Windows и доступно на большинстве платформ, в Интернете и в составе Office 365. При публикации приложений, использующих многофункциональную среду OneNote, вам открывается доступ к обширному кроссплатформенному рынку.

<!-- Might be good to show a few examples of Microsoft Graph API calls here, similar to what we have in the featured scenarios topic: https://developer.microsoft.com/en-us/graph/docs/concepts/featured_scenarios. You could have an H2 section called "What can I do with OneNote APIs in Microsoft Graph?"-->

## <a name="what-can-i-do-with-onenote-apis-in-microsoft-graph"></a>Возможности API OneNote в Microsoft Graph

Ниже приводятся некоторые из наиболее популярных запросов для работы с ресурсами OneNote.

|Операция|URL-адрес|
|:--------|:--|
|GET мои записные книжки|[https://graph.microsoft.com/v1.0/me/onenote/notebooks](https://developer.microsoft.com/ru-RU/graph/graph-explorer?request=me/onenote/notebooks&version=1.0)|
|GET мои разделы|[https://graph.microsoft.com/v1.0/me/onenote/sections](https://developer.microsoft.com/ru-RU/graph/graph-explorer?request=me/onenote/sections&version=1.0)|
|GET мои страницы|[https://graph.microsoft.com/v1.0/me/onenote/pages](https://developer.microsoft.com/ru-RU/graph/graph-explorer?request=me/onenote/pages&version=1.0)|

## <a name="explore-the-onenote-apis"></a>Изучение API OneNote
Используйте [песочницу Microsoft Graph](https://developer.microsoft.com/ru-RU/graph/graph-explorer), чтобы опробовать API OneNote с собственными записными книжками OneNote.

Чтобы отправлять вызовы API OneNote из песочницы Graph, нажмите **Показать другие примеры** в столбце слева. **Включите** OneNote с помощью меню. Вам также потребуется включить соответствующие разрешения. В меню слева под именем учетной записи выберите **Изменить разрешения**. Дополнительные сведения о разрешениях OneNote см. в разделе [Разрешения для заметок](permissions_reference.md#notes-permissions).

Чтобы приступить к работе с API OneNote в Microsoft Graph, см. [справочник по OneNote](../api-reference/v1.0/resources/onenote.md).

## <a name="see-also"></a>См. также

* [Правила размещения фирменной символики](https://msdn.microsoft.com/ru-RU/office/office365/howto/onenote-branding)
* [Получение содержимого и структуры OneNote](https://msdn.microsoft.com/ru-RU/office/office365/howto/onenote-get-content)
* [Добавление изображений, видео и файлов](https://msdn.microsoft.com/ru-RU/office/office365/howto/onenote-images-files)
* [Создание элементов с абсолютным положением](https://msdn.microsoft.com/ru-RU/office/office365/howto/onenote-abs-pos)
* [Извлечение данных](https://msdn.microsoft.com/ru-RU/office/office365/howto/onenote-extract-data)
* [Использование тегов заметок](https://msdn.microsoft.com/ru-RU/office/office365/howto/onenote-note-tags)

