# <a name="onedrive-file-storage-api-overview"></a><span data-ttu-id="85f47-101">Обзор API для хранилища файлов OneDrive</span><span class="sxs-lookup"><span data-stu-id="85f47-101">OneDrive file storage API overview</span></span>

<span data-ttu-id="85f47-102">OneDrive является центром файлов в Office 365.</span><span class="sxs-lookup"><span data-stu-id="85f47-102">OneDrive is the files hub in Office 365.</span></span>
<span data-ttu-id="85f47-103">Люди работают с файлами в различных контекстах, например Microsoft Teams, группах, SharePoint и т. д.</span><span class="sxs-lookup"><span data-stu-id="85f47-103">People work with files in a variety of contexts, like Microsoft Teams, groups, SharePoint, and more.</span></span>
<span data-ttu-id="85f47-104">С OneDrive пользователи открывать эти файлы независимо от того, где они хранятся, а с Microsoft Graph для работы с ними можно использовать один API.</span><span class="sxs-lookup"><span data-stu-id="85f47-104">With OneDrive, users can access these files no matter where they are stored, and with Microsoft Graph, you can use a single API to work with them.</span></span>

<span data-ttu-id="85f47-105">Файлы в Office 365 хранятся на [дисках][Drive API].</span><span class="sxs-lookup"><span data-stu-id="85f47-105">Files in Office 365 are stored in [drives][Drive API].</span></span>
<span data-ttu-id="85f47-106">Пользователи могут хранить файлы на личном (своем OneDrive) либо общем диске на базе библиотеки документов [SharePoint][].</span><span class="sxs-lookup"><span data-stu-id="85f47-106">Users can store files in a personal drive - their OneDrive - or in a shared drive powered by a [SharePoint][] document library.</span></span>
<span data-ttu-id="85f47-107">Гибкость OneDrive позволяет пользователям работать с коллегами так, как им удобно.</span><span class="sxs-lookup"><span data-stu-id="85f47-107">OneDrive's flexibility lets users collaborate however it works best for them.</span></span>
<span data-ttu-id="85f47-108">Пользователи могут делиться ссылками на файлы, копировать либо перемещать файлы на диски групп или даже прикреплять файлы OneDrive к почтовым сообщениям в Outlook.</span><span class="sxs-lookup"><span data-stu-id="85f47-108">Users can share links to files, copy or move files to team drives, or even attach OneDrive files to mail messages in Outlook.</span></span>

## <a name="why-integrate-with-onedrive-file-storage-in-the-cloud"></a><span data-ttu-id="85f47-109">Преимущества интеграции с облачным файловым хранилищем OneDrive?</span><span class="sxs-lookup"><span data-stu-id="85f47-109">Why integrate with OneDrive file storage in the cloud?</span></span>

### <a name="tap-into-an-ecosystem-with-billions-of-files"></a><span data-ttu-id="85f47-110">Использование экосистемы с миллиардами файлов</span><span class="sxs-lookup"><span data-stu-id="85f47-110">Tap into an ecosystem with billions of files</span></span>

<span data-ttu-id="85f47-111">Пользователи OneDrive могут получать доступ к своим файлам с любого устройства как подключением, так и без подключения к Интернету, и делиться ими с коллегами, так и с внешними пользователями.</span><span class="sxs-lookup"><span data-stu-id="85f47-111">OneDrive users can access their files from any device, online or offline, and share files with people inside or outside their organization.</span></span>
<span data-ttu-id="85f47-112">OneDrive позволяет совместно работать над документами в режиме реального времени в знакомых приложениях, таких как Word, Excel и PowerPoint.</span><span class="sxs-lookup"><span data-stu-id="85f47-112">OneDrive enables real-time coauthoring in familiar apps like Word, Excel, and PowerPoint.</span></span>
<span data-ttu-id="85f47-113">Платформа Microsoft Graph обеспечивает информативные эскизы для сотен форматов файлов, потоковой передачи видео, аналитики и многого другого.</span><span class="sxs-lookup"><span data-stu-id="85f47-113">Files light up with rich thumbnails for hundreds of formats, video streaming, analytics, and more, powered by Microsoft Graph.</span></span>
<span data-ttu-id="85f47-114">Данные в OneDrive защищены передовыми технологиями шифрования, соответствия требованиям и безопасности, которым доверяют клиенты.</span><span class="sxs-lookup"><span data-stu-id="85f47-114">Data in OneDrive is protected with advanced encryption, compliance, and security features that customers trust.</span></span>

<span data-ttu-id="85f47-115">Поскольку приложение OneDrive работает на более чем 500 миллионах устройств и более 85 % компаний из списка Fortune 500 используют OneDrive для бизнеса, интеграция вашего приложения с OneDrive позволит вам охватить миллионы потребителей, учащихся и бизнес-пользователей и взаимодействовать с клиентами там, где они уже работают каждый день.</span><span class="sxs-lookup"><span data-stu-id="85f47-115">With over 500 million devices running the OneDrive app and over 85% of the Fortune 500 using OneDrive for Business, by integrating your app with OneDrive, you can connect with millions of consumers, students, and business users and engage with customers where they already do their work every day.</span></span>

### <a name="store-your-apps-files-in-a-powerful-cloud"></a><span data-ttu-id="85f47-116">Хранение файлов вашего приложения в мощном облаке</span><span class="sxs-lookup"><span data-stu-id="85f47-116">Store your app's files in a powerful cloud</span></span>

<span data-ttu-id="85f47-117">Когда вы храните файлы в OneDrive, ваше приложение может использовать возможности облака Майкрософт, а ваши пользователи могут получать доступ к своим файлам, где бы они ни находились.</span><span class="sxs-lookup"><span data-stu-id="85f47-117">When you store your files in OneDrive, your app can take advantage of the features of the Microsoft cloud and your users can access their files anywhere.</span></span>
<span data-ttu-id="85f47-118">Используйте пакет SDK для [средства выбора файлов][], чтобы быстро открывать, скачивать и сохранять файлы, хранимые в OneDrive, а также делиться ими из вашего приложения через знакомый интерфейс OneDrive.</span><span class="sxs-lookup"><span data-stu-id="85f47-118">Use the [file picker][] SDK to quickly open, download, save, or share files stored in OneDrive from within your own app, using the same experience OneDrive users are familiar with.</span></span>
<span data-ttu-id="85f47-119">Получайте информацию о выбранных файлах прямо из пакета SDK или используйте API Microsoft Graph для более глубокого взаимодействия с файлами.</span><span class="sxs-lookup"><span data-stu-id="85f47-119">Get information about selected files directly from the picker SDK, or use Microsoft Graph APIs directly to interact more deeply with files.</span></span>
<span data-ttu-id="85f47-120">Используйте [специальные папки][], чтобы хранить файлы в известных папках OneDrive, например `Documents` и `Camera Roll`, или предоставьте своему приложению собственную папку.</span><span class="sxs-lookup"><span data-stu-id="85f47-120">Use [special folders][] to store files in well-known locations on OneDrive, like `Documents` and `Camera Roll`, or give your app its own personal folder.</span></span>

### <a name="bring-your-app-straight-to-users-within-onedrive"></a><span data-ttu-id="85f47-121">Подача вашего приложения напрямую пользователям в OneDrive</span><span class="sxs-lookup"><span data-stu-id="85f47-121">Bring your app straight to users within OneDrive</span></span>

<span data-ttu-id="85f47-122">Клиенты OneDrive могут запускать ваше приложение прямо из OneDrive, чтобы открывать, редактировать или просматривать файлы.</span><span class="sxs-lookup"><span data-stu-id="85f47-122">OneDrive customers can use or launch your app directly from within OneDrive to open, edit, or preview files.</span></span>
<span data-ttu-id="85f47-123">Используйте расширения [обработчика файлов][] OneDrive, чтобы предоставить значки и эскизы для своих расширений файлов; добавьте свое приложение в кнопку **Создать** или даже действия в строку меню для запуска своего приложения.</span><span class="sxs-lookup"><span data-stu-id="85f47-123">Use OneDrive's [file handler][] extensions to provide icons and previews for your own custom file extensions, add your app to the **New** button or even add your own custom actions to the menu bar to launch your app.</span></span>

### <a name="work-with-content-in-formats-your-app-understands"></a><span data-ttu-id="85f47-124">Работа с содержимым в форматах, которые понимает ваше приложение</span><span class="sxs-lookup"><span data-stu-id="85f47-124">Work with content in formats your app understands</span></span>

<span data-ttu-id="85f47-125">Ваше приложение может получить содержимое в наиболее удобном для вас формате.</span><span class="sxs-lookup"><span data-stu-id="85f47-125">Your app can get file content in the format that is most convenient for you.</span></span>
<span data-ttu-id="85f47-126">Приложение может отображать [эскизы][] нестандартного размера для сотен различных форматов файлов.</span><span class="sxs-lookup"><span data-stu-id="85f47-126">Your app can display custom-sized [thumbnails][] for hundreds of different file formats.</span></span>
<span data-ttu-id="85f47-127">Вы можете скачивать файлы в различных альтернативных [форматах][], например PDF.</span><span class="sxs-lookup"><span data-stu-id="85f47-127">You can download files in a variety of alternative [formats][], like PDF.</span></span>
<span data-ttu-id="85f47-128">Вы даже можете внедрить предварительный просмотр файлов OneDrive в свое приложение, воспользовавшись API [предварительного просмотра][] (бета-версия).</span><span class="sxs-lookup"><span data-stu-id="85f47-128">You can even embed the OneDrive file previewers within your app by using the [preview][] API (beta).</span></span>

### <a name="work-with-file-content-and-metadata-without-downloading-the-binary"></a><span data-ttu-id="85f47-129">Работа с содержимым и метаданными файла без скачивания двоичных данных</span><span class="sxs-lookup"><span data-stu-id="85f47-129">Work with file content and metadata without downloading the binary</span></span>

<span data-ttu-id="85f47-130">Microsoft Graph открывает доступ к различному содержимому через REST API без необходимости скачивания двоичных данных.</span><span class="sxs-lookup"><span data-stu-id="85f47-130">With Microsoft Graph, you can access rich content through REST APIs without having to download the binary.</span></span>
<span data-ttu-id="85f47-131">Изучайте извлеченные метаданные из [фотографий][], [аудиофайлов][] и [видеофайлов][].</span><span class="sxs-lookup"><span data-stu-id="85f47-131">Explore extracted metadata from [photo][], [audio][], and [video][] files.</span></span>
<span data-ttu-id="85f47-132">Используйте [API Excel][] для работы с необработанными данными, хранящимися в книге Excel.</span><span class="sxs-lookup"><span data-stu-id="85f47-132">Use the [Excel API][] to work directly with the raw data stored in an Excel workbook.</span></span>
<span data-ttu-id="85f47-133">Используйте [API заметок][] для доступа к содержимому записных книжек OneNote.</span><span class="sxs-lookup"><span data-stu-id="85f47-133">Use the [Notes API][] to access the contents of OneNote notebooks.</span></span>

### <a name="react-to-file-changes"></a><span data-ttu-id="85f47-134">Реагирование на изменения файлов</span><span class="sxs-lookup"><span data-stu-id="85f47-134">React to file changes</span></span>

<span data-ttu-id="85f47-135">С помощью [веб-перехватчиков][] ваше приложение может получать уведомления при изменении файлов, чтобы вы могли быстро отреагировать.</span><span class="sxs-lookup"><span data-stu-id="85f47-135">With [webhooks][], your app can get notified when files change so you can quickly react.</span></span>
<span data-ttu-id="85f47-136">Используйте [API изменений][], чтобы посмотреть, что изменилось с момента последней синхронизации вашего приложения с облаком.</span><span class="sxs-lookup"><span data-stu-id="85f47-136">Use the [delta API][] to see what changed since the last time your app synchronized with the cloud.</span></span>

## <a name="next-steps"></a><span data-ttu-id="85f47-137">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="85f47-137">Next steps</span></span>

<span data-ttu-id="85f47-138">Узнайте больше об [использовании API OneDrive][Drive API] в Microsoft Graph версии 1.0.</span><span class="sxs-lookup"><span data-stu-id="85f47-138">Find out more about [using the OneDrive API][Drive API] in Microsoft Graph v1.0.</span></span>

[SharePoint]: sharepoint-concept-overview.md
[средство выбора файлов]: https://dev.onedrive.com/sdk/js-v72/js-picker-overview.htm
[File picker]: https://dev.onedrive.com/sdk/js-v72/js-picker-overview.htm
[обработчик файлов]: https://docs.microsoft.com/onedrive/developer/file-handlers
[file handler]: https://docs.microsoft.com/onedrive/developer/file-handlers
<span data-ttu-id="85f47-142">
  [специальные папки]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/drive_get_specialfolder</span><span class="sxs-lookup"><span data-stu-id="85f47-142">[Special folders]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/drive_get_specialfolder</span></span>
<span data-ttu-id="85f47-143">
  [API заметок]: https://developer.microsoft.com/en-us/graph/docs/concepts/integrate_with_onenote</span><span class="sxs-lookup"><span data-stu-id="85f47-143">[Notes API]: https://developer.microsoft.com/en-us/graph/docs/concepts/integrate_with_onenote</span></span>
<span data-ttu-id="85f47-144">
  [API Excel]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/excel</span><span class="sxs-lookup"><span data-stu-id="85f47-144">[Excel API]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/excel</span></span>
[REST API]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/onedrive
<span data-ttu-id="85f47-145">
  [API изменений]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/driveitem_delta</span><span class="sxs-lookup"><span data-stu-id="85f47-145">[delta API]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/driveitem_delta</span></span>
<span data-ttu-id="85f47-146">
  [видео]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/video</span><span class="sxs-lookup"><span data-stu-id="85f47-146">[video]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/video</span></span>
<span data-ttu-id="85f47-147">
  [фото]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/photo</span><span class="sxs-lookup"><span data-stu-id="85f47-147">[photo]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/photo</span></span>
<span data-ttu-id="85f47-148">
  [аудио]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/audio</span><span class="sxs-lookup"><span data-stu-id="85f47-148">[audio]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/audio</span></span>
<span data-ttu-id="85f47-149">
  [форматы]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/driveitem_get_content_format</span><span class="sxs-lookup"><span data-stu-id="85f47-149">[Formats]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/driveitem_get_content_format</span></span>
<span data-ttu-id="85f47-150">
  [эскизы]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/driveitem_list_thumbnails</span><span class="sxs-lookup"><span data-stu-id="85f47-150">[thumbnails]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/driveitem_list_thumbnails</span></span>
<span data-ttu-id="85f47-151">
  [предварительный просмотр]: https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/driveitem_preview</span><span class="sxs-lookup"><span data-stu-id="85f47-151">[preview]: https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/driveitem_preview</span></span>
<span data-ttu-id="85f47-152">
  [веб-перехватчики]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/webhooks</span><span class="sxs-lookup"><span data-stu-id="85f47-152">[Webhooks]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/webhooks</span></span>
[Drive API]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/onedrive
