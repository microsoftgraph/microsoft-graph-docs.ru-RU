---
title: Обзор API для хранилища файлов OneDrive
description: OneDrive является центром файлов в Office 365.
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 9bbc5158140930081beb665580b3f8344f6a1738
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32560769"
---
# <a name="onedrive-file-storage-api-overview"></a><span data-ttu-id="8d784-103">Обзор API для хранилища файлов OneDrive</span><span class="sxs-lookup"><span data-stu-id="8d784-103">OneDrive file storage API overview</span></span>

<span data-ttu-id="8d784-104">OneDrive является центром файлов в Office 365.</span><span class="sxs-lookup"><span data-stu-id="8d784-104">OneDrive is the files hub in Office 365.</span></span>
<span data-ttu-id="8d784-105">Люди работают с файлами в различных контекстах, например Microsoft Teams, группах, SharePoint и т. д.</span><span class="sxs-lookup"><span data-stu-id="8d784-105">People work with files in a variety of contexts, like Microsoft Teams, groups, SharePoint, and more.</span></span>
<span data-ttu-id="8d784-106">С OneDrive пользователи открывать эти файлы независимо от того, где они хранятся, а с Microsoft Graph для работы с ними можно использовать один API.</span><span class="sxs-lookup"><span data-stu-id="8d784-106">With OneDrive, users can access these files no matter where they are stored, and with Microsoft Graph, you can use a single API to work with them.</span></span>

<span data-ttu-id="8d784-107">Файлы в Office 365 хранятся на [дисках][Drive API].</span><span class="sxs-lookup"><span data-stu-id="8d784-107">Files in Office 365 are stored in [drives][Drive API].</span></span>
<span data-ttu-id="8d784-108">Пользователи могут хранить файлы на личном (своем OneDrive) либо общем диске на базе библиотеки документов [SharePoint][].</span><span class="sxs-lookup"><span data-stu-id="8d784-108">Users can store files in a personal drive - their OneDrive - or in a shared drive powered by a [SharePoint][] document library.</span></span>
<span data-ttu-id="8d784-109">Гибкость OneDrive позволяет пользователям работать с коллегами так, как им удобно.</span><span class="sxs-lookup"><span data-stu-id="8d784-109">OneDrive's flexibility lets users collaborate however it works best for them.</span></span>
<span data-ttu-id="8d784-110">Пользователи могут делиться ссылками на файлы, копировать либо перемещать файлы на диски групп или даже прикреплять файлы OneDrive к почтовым сообщениям в Outlook.</span><span class="sxs-lookup"><span data-stu-id="8d784-110">Users can share links to files, copy or move files to team drives, or even attach OneDrive files to mail messages in Outlook.</span></span>

## <a name="why-integrate-with-onedrive-file-storage-in-the-cloud"></a><span data-ttu-id="8d784-111">Преимущества интеграции с облачным файловым хранилищем OneDrive?</span><span class="sxs-lookup"><span data-stu-id="8d784-111">Why integrate with OneDrive file storage in the cloud?</span></span>

### <a name="tap-into-an-ecosystem-with-billions-of-files"></a><span data-ttu-id="8d784-112">Использование экосистемы с миллиардами файлов</span><span class="sxs-lookup"><span data-stu-id="8d784-112">Tap into an ecosystem with billions of files</span></span>

<span data-ttu-id="8d784-113">Пользователи OneDrive могут получать доступ к своим файлам с любого устройства как подключением, так и без подключения к Интернету, и делиться ими с коллегами, так и с внешними пользователями.</span><span class="sxs-lookup"><span data-stu-id="8d784-113">OneDrive users can access their files from any device, online or offline, and share files with people inside or outside their organization.</span></span>
<span data-ttu-id="8d784-114">OneDrive позволяет совместно работать над документами в режиме реального времени в знакомых приложениях, таких как Word, Excel и PowerPoint.</span><span class="sxs-lookup"><span data-stu-id="8d784-114">OneDrive enables real-time coauthoring in familiar apps like Word, Excel, and PowerPoint.</span></span>
<span data-ttu-id="8d784-115">Платформа Microsoft Graph обеспечивает информативные эскизы для сотен форматов файлов, потоковой передачи видео, аналитики и многого другого.</span><span class="sxs-lookup"><span data-stu-id="8d784-115">Files light up with rich thumbnails for hundreds of formats, video streaming, analytics, and more, powered by Microsoft Graph.</span></span>
<span data-ttu-id="8d784-116">Данные в OneDrive защищены передовыми технологиями шифрования, соответствия требованиям и безопасности, которым доверяют клиенты.</span><span class="sxs-lookup"><span data-stu-id="8d784-116">Data in OneDrive is protected with advanced encryption, compliance, and security features that customers trust.</span></span>

<span data-ttu-id="8d784-117">Поскольку приложение OneDrive работает на более чем 500 миллионах устройств и более 85 % компаний из списка Fortune 500 используют OneDrive для бизнеса, интеграция вашего приложения с OneDrive позволит вам охватить миллионы потребителей, учащихся и бизнес-пользователей и взаимодействовать с клиентами там, где они уже работают каждый день.</span><span class="sxs-lookup"><span data-stu-id="8d784-117">With over 500 million devices running the OneDrive app and over 85% of the Fortune 500 using OneDrive for Business, by integrating your app with OneDrive, you can connect with millions of consumers, students, and business users and engage with customers where they already do their work every day.</span></span>

### <a name="store-your-apps-files-in-a-powerful-cloud"></a><span data-ttu-id="8d784-118">Хранение файлов вашего приложения в мощном облаке</span><span class="sxs-lookup"><span data-stu-id="8d784-118">Store your app's files in a powerful cloud</span></span>

<span data-ttu-id="8d784-119">Когда вы храните файлы в OneDrive, ваше приложение может использовать возможности облака Майкрософт, а ваши пользователи могут получать доступ к своим файлам, где бы они ни находились.</span><span class="sxs-lookup"><span data-stu-id="8d784-119">When you store your files in OneDrive, your app can take advantage of the features of the Microsoft cloud and your users can access their files anywhere.</span></span>
<span data-ttu-id="8d784-120">Используйте пакет SDK для [средства выбора файлов][], чтобы быстро открывать, скачивать и сохранять файлы, хранимые в OneDrive, а также делиться ими из вашего приложения через знакомый интерфейс OneDrive.</span><span class="sxs-lookup"><span data-stu-id="8d784-120">Use the [file picker][] SDK to quickly open, download, save, or share files stored in OneDrive from within your own app, using the same experience OneDrive users are familiar with.</span></span>
<span data-ttu-id="8d784-121">Получайте информацию о выбранных файлах прямо из пакета SDK или используйте API Microsoft Graph для более глубокого взаимодействия с файлами.</span><span class="sxs-lookup"><span data-stu-id="8d784-121">Get information about selected files directly from the picker SDK, or use Microsoft Graph APIs directly to interact more deeply with files.</span></span>
<span data-ttu-id="8d784-122">Используйте [специальные папки][], чтобы хранить файлы в известных папках OneDrive, например `Documents` и `Camera Roll`, или предоставьте своему приложению собственную папку.</span><span class="sxs-lookup"><span data-stu-id="8d784-122">Use [special folders][] to store files in well-known locations on OneDrive, like `Documents` and `Camera Roll`, or give your app its own personal folder.</span></span>

### <a name="bring-your-app-straight-to-users-within-onedrive"></a><span data-ttu-id="8d784-123">Подача вашего приложения напрямую пользователям в OneDrive</span><span class="sxs-lookup"><span data-stu-id="8d784-123">Bring your app straight to users within OneDrive</span></span>

<span data-ttu-id="8d784-124">Клиенты OneDrive могут запускать ваше приложение прямо из OneDrive, чтобы открывать, редактировать или просматривать файлы.</span><span class="sxs-lookup"><span data-stu-id="8d784-124">OneDrive customers can use or launch your app directly from within OneDrive to open, edit, or preview files.</span></span>
<span data-ttu-id="8d784-125">Используйте расширения [обработчика файлов][] OneDrive, чтобы предоставить значки и эскизы для своих расширений файлов; добавьте свое приложение в кнопку **Создать** или даже действия в строку меню для запуска своего приложения.</span><span class="sxs-lookup"><span data-stu-id="8d784-125">Use OneDrive's [file handler][] extensions to provide icons and previews for your own custom file extensions, add your app to the **New** button or even add your own custom actions to the menu bar to launch your app.</span></span>

### <a name="work-with-content-in-formats-your-app-understands"></a><span data-ttu-id="8d784-126">Работа с содержимым в форматах, которые понимает ваше приложение</span><span class="sxs-lookup"><span data-stu-id="8d784-126">Work with content in formats your app understands</span></span>

<span data-ttu-id="8d784-127">Ваше приложение может получить содержимое в наиболее удобном для вас формате.</span><span class="sxs-lookup"><span data-stu-id="8d784-127">Your app can get file content in the format that is most convenient for you.</span></span>
<span data-ttu-id="8d784-128">Приложение может отображать [эскизы][] нестандартного размера для сотен различных форматов файлов.</span><span class="sxs-lookup"><span data-stu-id="8d784-128">Your app can display custom-sized [thumbnails][] for hundreds of different file formats.</span></span>
<span data-ttu-id="8d784-129">Вы можете скачивать файлы в различных альтернативных [форматах][], например PDF.</span><span class="sxs-lookup"><span data-stu-id="8d784-129">You can download files in a variety of alternative [formats][], like PDF.</span></span>
<span data-ttu-id="8d784-130">Вы даже можете внедрить предварительный просмотр файлов OneDrive в свое приложение, воспользовавшись API [предварительного просмотра][] (бета-версия).</span><span class="sxs-lookup"><span data-stu-id="8d784-130">You can even embed the OneDrive file previewers within your app by using the [preview][] API (beta).</span></span>

### <a name="work-with-file-content-and-metadata-without-downloading-the-binary"></a><span data-ttu-id="8d784-131">Работа с содержимым и метаданными файла без скачивания двоичных данных</span><span class="sxs-lookup"><span data-stu-id="8d784-131">Work with file content and metadata without downloading the binary</span></span>

<span data-ttu-id="8d784-132">Microsoft Graph открывает доступ к различному содержимому через REST API без необходимости скачивания двоичных данных.</span><span class="sxs-lookup"><span data-stu-id="8d784-132">With Microsoft Graph, you can access rich content through REST APIs without having to download the binary.</span></span>
<span data-ttu-id="8d784-133">Изучайте извлеченные метаданные из [фотографий][], [аудиофайлов][] и [видеофайлов][].</span><span class="sxs-lookup"><span data-stu-id="8d784-133">Explore extracted metadata from [photo][], [audio][], and [video][] files.</span></span>
<span data-ttu-id="8d784-134">Используйте [API Excel][] для работы с необработанными данными, хранящимися в книге Excel.</span><span class="sxs-lookup"><span data-stu-id="8d784-134">Use the [Excel API][] to work directly with the raw data stored in an Excel workbook.</span></span>
<span data-ttu-id="8d784-135">Используйте [API заметок][] для доступа к содержимому записных книжек OneNote.</span><span class="sxs-lookup"><span data-stu-id="8d784-135">Use the [Notes API][] to access the contents of OneNote notebooks.</span></span>

### <a name="react-to-file-changes"></a><span data-ttu-id="8d784-136">Реагирование на изменения файлов</span><span class="sxs-lookup"><span data-stu-id="8d784-136">React to file changes</span></span>

<span data-ttu-id="8d784-137">С помощью [веб-перехватчиков][] ваше приложение может получать уведомления при изменении файлов, чтобы вы могли быстро отреагировать.</span><span class="sxs-lookup"><span data-stu-id="8d784-137">With [webhooks][], your app can get notified when files change so you can quickly react.</span></span>
<span data-ttu-id="8d784-138">Используйте [API изменений][], чтобы посмотреть, что изменилось с момента последней синхронизации вашего приложения с облаком.</span><span class="sxs-lookup"><span data-stu-id="8d784-138">Use the [delta API][] to see what changed since the last time your app synchronized with the cloud.</span></span>

## <a name="api-reference"></a><span data-ttu-id="8d784-139">Справочные материалы по API</span><span class="sxs-lookup"><span data-stu-id="8d784-139">API reference</span></span>
<span data-ttu-id="8d784-140">Ищете справочные материалы по API для этой службы?</span><span class="sxs-lookup"><span data-stu-id="8d784-140">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="8d784-141">API для хранилища файлов OneDrive в Microsoft Graph 1.0</span><span class="sxs-lookup"><span data-stu-id="8d784-141">OneDrive file storage API in Microsoft Graph v1.0</span></span>](/graph/api/resources/onedrive?view=graph-rest-1.0)
- [<span data-ttu-id="8d784-142">API для хранилища файлов OneDrive в бета-версии Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8d784-142">OneDrive file storage API in Microsoft Graph beta</span></span>](/graph/api/resources/onedrive?view=graph-rest-beta)

## <a name="next-steps"></a><span data-ttu-id="8d784-143">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="8d784-143">Next steps</span></span>

<span data-ttu-id="8d784-144">Узнайте больше об [использовании API OneDrive][Drive API] в Microsoft Graph версии 1.0.</span><span class="sxs-lookup"><span data-stu-id="8d784-144">Find out more about [using the OneDrive API][Drive API] in Microsoft Graph v1.0.</span></span>

[SharePoint]: sharepoint-concept-overview.md
[средство выбора файлов]: https://dev.onedrive.com/sdk/js-v72/js-picker-overview.htm
[file picker]: https://dev.onedrive.com/sdk/js-v72/js-picker-overview.htm
[обработчик файлов]: https://docs.microsoft.com/onedrive/developer/file-handlers
[file handler]: https://docs.microsoft.com/onedrive/developer/file-handlers
[специальные папки]: /graph/api/drive-get-specialfolder?view=graph-rest-1.0
[special folders]: /graph/api/drive-get-specialfolder?view=graph-rest-1.0
[API заметок]: integrate-with-onenote.md
[Notes API]: integrate-with-onenote.md
[API Excel]: /graph/api/resources/excel?view=graph-rest-1.0
[Excel API]: /graph/api/resources/excel?view=graph-rest-1.0
[REST API]: /graph/api/resources/onedrive?view=graph-rest-1.0
[API изменений]: /graph/api/driveitem-delta?view=graph-rest-1.0
[delta API]: /graph/api/driveitem-delta?view=graph-rest-1.0
[видео]: /graph/api/resources/video?view=graph-rest-1.0
[video]: /graph/api/resources/video?view=graph-rest-1.0
[фото]: /graph/api/resources/photo?view=graph-rest-1.0
[photo]: /graph/api/resources/photo?view=graph-rest-1.0
[аудио]: /graph/api/resources/audio?view=graph-rest-1.0
[audio]: /graph/api/resources/audio?view=graph-rest-1.0
[форматы]: /graph/api/driveitem-get-content-format?view=graph-rest-1.0
[formats]: /graph/api/driveitem-get-content-format?view=graph-rest-1.0
[эскизы]: /graph/api/driveitem-list-thumbnails?view=graph-rest-1.0
[thumbnails]: /graph/api/driveitem-list-thumbnails?view=graph-rest-1.0
[предварительный просмотр]: /graph/api/driveitem-preview?view=graph-rest-beta
[preview]: /graph/api/driveitem-preview?view=graph-rest-beta
[веб-перехватчики]: /graph/api/resources/webhooks?view=graph-rest-1.0
[webhooks]: /graph/api/resources/webhooks?view=graph-rest-1.0
[Drive API]: /graph/api/resources/onedrive?view=graph-rest-1.0
