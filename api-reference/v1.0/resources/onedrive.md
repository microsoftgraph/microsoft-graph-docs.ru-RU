# <a name="working-with-files-in-microsoft-graph"></a><span data-ttu-id="2ea90-101">Работа с файлами в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2ea90-101">Working with files in Microsoft Graph</span></span>

<span data-ttu-id="2ea90-p101">С помощью Microsoft Graph можно создать приложение, которое подключается к файлам в OneDrive, OneDrive для бизнеса и библиотеках документов SharePoint. Используя Microsoft Graph, вы можете создавать различные решения для работы с файлами в Office 365. Возможны варианты как для простого хранения документов пользователей, так и сложные сценарии совместного использования файлов.</span><span class="sxs-lookup"><span data-stu-id="2ea90-p101">You can use Microsoft Graph to create an app that connects with files across OneDrive, OneDrive for Business, and SharePoint document libraries. With Microsoft Graph, you can build a variety of experiences with files stored in Office 365, from simply storing user documents to complex file sharing scenarios.</span></span>

<span data-ttu-id="2ea90-104">В Microsoft Graph доступны два типа ресурсов для работы с файлами:</span><span class="sxs-lookup"><span data-stu-id="2ea90-104">Microsoft Graph exposes two resource types for working with files:</span></span>

* <span data-ttu-id="2ea90-105">[Drive](drive.md). Представляет логический контейнер для файлов, например библиотеку документов или пользовательское хранилище OneDrive.</span><span class="sxs-lookup"><span data-stu-id="2ea90-105">[Drive](drive.md) - Represents a logical container of files, like a document library or a user's OneDrive.</span></span>
* <span data-ttu-id="2ea90-106">[DriveItem](driveitem.md). Представляет элемент на диске, например документ, фотографию, видео или папку.</span><span class="sxs-lookup"><span data-stu-id="2ea90-106">[DriveItem](driveitem.md) - Represents an item within a drive, like a document, photo, video, or folder.</span></span>

<span data-ttu-id="2ea90-107">Большинство операций с файлами выполняется путем взаимодействия с ресурсами **DriveItem**.</span><span class="sxs-lookup"><span data-stu-id="2ea90-107">Most of the interaction with files occurs through interaction with **DriveItem** resources. The following is an example of a DriveItem resource:</span></span> <span data-ttu-id="2ea90-108">Ниже представлен пример ресурса DriveItem.</span><span class="sxs-lookup"><span data-stu-id="2ea90-108">The following is an example of a driveItem resource.</span></span>

```json
{
  "@content.downloadUrl":"http://public-sn3302.files.1drv.com/y2pcT7OaUEExF7EHOlpTjCE55mIUoiX7H3sx1ff6I-nP35XUTBqZlnkh9FJhWb_pf9sZ7LEpEchvDznIbQig0hWBeidpwFkOqSKCwQylisarN6T0ecAeMvantizBUzM2PA1",
  "createdDateTime": "2016-09-16T03:37:04.72Z",
  "cTag": "aYzpENDY0OEYwNkM5MUQ5RDNEITU0OTI3LjI1Ng",
  "eTag": "aRDQ2NDhGMDZDOTFEOUQzRCE1NDkyNy4w",
  "id":"D4648F06C91D9D3D!54927",
  "lastModifiedBy": {
    "user": {
      "displayName": "Daron Spektor",
      "id": "d4648f06c91d9d3d"
    }
  },
  "name":"BritishShorthair.jpg",
  "size":35212,
  "image":{
    "height":398,
    "width":273
  },
  "file": {
    "hashes":{
      "sha1Hash":"wmgPQ6jrSeMX7JP1XmstQEGM2fc="
    }
  }
}
```

<span data-ttu-id="2ea90-109">В ресурсах **Drive** и **DriveItem** данные доступны в трех вариантах.</span><span class="sxs-lookup"><span data-stu-id="2ea90-109">**Drive** and **DriveItem** resources expose data in three different ways:</span></span>

* <span data-ttu-id="2ea90-110">Как _свойства_ (например, **id** и **name**), которые представляют простые значения (строки, числа, логические значения).</span><span class="sxs-lookup"><span data-stu-id="2ea90-110">_Properties_ (like **id** and **name**) expose simple values (strings, numbers, Booleans).</span></span>
* <span data-ttu-id="2ea90-111">_Аспекты_ (например, **file** и **photo**) содержат сложные значения.</span><span class="sxs-lookup"><span data-stu-id="2ea90-111">_Facets_ (like **file** and **photo**) expose complex values.</span></span> <span data-ttu-id="2ea90-112">Наличие аспекта **file** или **folder** указывает поведение и свойства ресурса **DriveItem**.</span><span class="sxs-lookup"><span data-stu-id="2ea90-112">Facets (like file and photo) expose complex values. The presence of **file** or **folder** facets indicates behaviors and properties of a **DriveItem**.</span></span>
* <span data-ttu-id="2ea90-113">_Ссылки_ (например, **children** и **thumbnails**) указывают на коллекции других ресурсов.</span><span class="sxs-lookup"><span data-stu-id="2ea90-113">_References_ (like **children** and **thumbnails**) point to collections of other resources.</span></span>

## <a name="commonly-accessed-resources"></a><span data-ttu-id="2ea90-114">Часто используемые ресурсы</span><span class="sxs-lookup"><span data-stu-id="2ea90-114">Commonly accessed resources</span></span>

<span data-ttu-id="2ea90-115">В большинстве запросов API для работы с файлами используется один из указанных ниже базовых ресурсов, позволяющих получить доступ к ресурсу **Drive** или **DriveItem**.</span><span class="sxs-lookup"><span data-stu-id="2ea90-115">Most API requests for file interactions will use one of these base resources to access a **Drive** or **DriveItem**.</span></span>

| <span data-ttu-id="2ea90-116">Путь</span><span class="sxs-lookup"><span data-stu-id="2ea90-116">Path</span></span>    | <span data-ttu-id="2ea90-117">Ресурс</span><span class="sxs-lookup"><span data-stu-id="2ea90-117">Resource</span></span>    |
|---------|-------------|
| `/me/drive` | <span data-ttu-id="2ea90-118">Хранилище OneDrive пользователя</span><span class="sxs-lookup"><span data-stu-id="2ea90-118">User's OneDrive</span></span> |
| `/me/drives` | <span data-ttu-id="2ea90-119">Перечисление ресурсов OneDrive, доступных пользователю.</span><span class="sxs-lookup"><span data-stu-id="2ea90-119">Enumerate OneDrive resources available to the user.</span></span> |
| `/drives/{drive-id}` | <span data-ttu-id="2ea90-120">Доступ к определенному ресурсу **Drive** по идентификатору диска.</span><span class="sxs-lookup"><span data-stu-id="2ea90-120">Access a specific **Drive** by the drive's ID.</span></span> |
| `/drives/{drive-id}/root/children` | <span data-ttu-id="2ea90-121">Перечисление ресурсов **DriveItem** в корне определенного ресурса **Drive**.</span><span class="sxs-lookup"><span data-stu-id="2ea90-121">Enumerate the **DriveItem** resources in the root of a specific **Drive**.</span></span> |
| `/me/drive/items/{item-id}` | <span data-ttu-id="2ea90-122">Доступ к ресурсу **DriveItem** в пользовательском хранилище OneDrive по его уникальному идентификатору.</span><span class="sxs-lookup"><span data-stu-id="2ea90-122">Access a **DriveItem** in the user's OneDrive by its unique ID.</span></span> |
| `/me/drive/special/{special-id}` | <span data-ttu-id="2ea90-123">Доступ к специальной (именованной) папке в пользовательском хранилище OneDrive по ее известному имени.</span><span class="sxs-lookup"><span data-stu-id="2ea90-123">Access a special (named) folder in the user's OneDrive by its known name.</span></span> |
| `/users/{user-id}/drive` | <span data-ttu-id="2ea90-124">Доступ к хранилищу OneDrive другого пользователя по уникальному идентификатору этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="2ea90-124">Access another user's OneDrive by using the user's unique ID.</span></span> |
| `/groups/{group-id}/drive` | <span data-ttu-id="2ea90-125">Доступ к стандартной библиотеке документов группы по уникальному идентификатору этой группы.</span><span class="sxs-lookup"><span data-stu-id="2ea90-125">Access the default document library for a group by the group's unique ID.</span></span> |
| `/shares/{share-id}` | <span data-ttu-id="2ea90-126">Доступ к ресурсу **DriveItem** по свойству **sharedId** или URL-адресу для совместного доступа.</span><span class="sxs-lookup"><span data-stu-id="2ea90-126">Access a **DriveItem** by its **sharedId** or sharing URL.</span></span> |

<span data-ttu-id="2ea90-127">Ваше приложение может обращаться к элементу **DriveItem** в ресурсе **Drive** не только по уникальному идентификатору, но и по относительному пути от известного ресурса.</span><span class="sxs-lookup"><span data-stu-id="2ea90-127">In addition to addressing a **DriveItem** within a **Drive** by unique ID, your app can also address a **DriveItem** by relative path from a known resource. To address using a path, the colon () character is used to escape the relative path. This table provides an example of different ways to use the colon character to address an item by path.</span></span>
<span data-ttu-id="2ea90-128">Чтобы путь не был относительным, используйте двоеточие (`:`).</span><span class="sxs-lookup"><span data-stu-id="2ea90-128">To address using a path, the colon (`:`) character is used to escape the relative path.</span></span>
<span data-ttu-id="2ea90-129">В этой таблице представлены примеры различных способов использования двоеточия для обращения к элементу по пути.</span><span class="sxs-lookup"><span data-stu-id="2ea90-129">This table provides an example of different ways to use the colon character to address an item by path.</span></span>

| <span data-ttu-id="2ea90-130">Путь</span><span class="sxs-lookup"><span data-stu-id="2ea90-130">Path</span></span> | <span data-ttu-id="2ea90-131">Ресурс</span><span class="sxs-lookup"><span data-stu-id="2ea90-131">Resource</span></span> |
|---|---|
| `/me/drive/root:/path/to/file` | <span data-ttu-id="2ea90-132">Доступ к ресурсу **DriveItem** по относительному пути для корневой папки OneDrive пользователя.</span><span class="sxs-lookup"><span data-stu-id="2ea90-132">Access a **DriveItem** by path relative to the user's OneDrive root folder.</span></span> |
| `/me/drive/items/{item-id}:/path/to/file` | <span data-ttu-id="2ea90-133">Доступ к ресурсу **DriveItem** по относительному пути для другого элемента (экземпляра **DriveItem** с аспектом **folder**).</span><span class="sxs-lookup"><span data-stu-id="2ea90-133">Access a **DriveItem** by path relative to another item (a **DriveItem** with a **folder** facet).</span></span> |
| `/me/drive/root:/path/to/folder:/children` | <span data-ttu-id="2ea90-134">Получение списка дочерних экземпляров ресурса **DriveItem** по относительному пути для корневого каталога OneDrive пользователя.</span><span class="sxs-lookup"><span data-stu-id="2ea90-134">List the children of a **DriveItem** by path relative to the root of the user's OneDrive.</span></span> |
| `/me/drive/items/{item-id}:/path/to/folder:/children` | <span data-ttu-id="2ea90-135">Получение списка дочерних экземпляров ресурса **DriveItem** по относительному пути для другого элемента.</span><span class="sxs-lookup"><span data-stu-id="2ea90-135">List the children of a **DriveItem** by path relative to another item.</span></span> |

## <a name="drive-resource"></a><span data-ttu-id="2ea90-136">Ресурс Drive</span><span class="sxs-lookup"><span data-stu-id="2ea90-136">Drive resource</span></span>

<span data-ttu-id="2ea90-137">[Ресурс Drive](drive.md) — это объект верхнего уровня в хранилище OneDrive или библиотеке документов SharePoint пользователя.</span><span class="sxs-lookup"><span data-stu-id="2ea90-137">The [Drive resource](drive.md) is the top-level object within a user's OneDrive or a SharePoint document library. Nearly all files operations will start by addressing a specific drive resource.</span></span>
<span data-ttu-id="2ea90-138">Почти все операции с файлами начинаются с обращения к определенному ресурсу диска.</span><span class="sxs-lookup"><span data-stu-id="2ea90-138">The Drive resource is the top-level object within a user's OneDrive or a SharePoint document library. Nearly all files operations will start by addressing a specific drive resource.</span></span>

<span data-ttu-id="2ea90-139">К ресурсу диска можно обратиться по уникальному идентификатору диска или с помощью диска по умолчанию для [User](user.md), [Group](group.md) или организации.</span><span class="sxs-lookup"><span data-stu-id="2ea90-139">A drive resource can be addressed either by the drive's unique ID or by the default drive for a [User](user.md), [Group](group.md), or organization.</span></span> 

## <a name="driveitem-resource"></a><span data-ttu-id="2ea90-140">Ресурс DriveItem</span><span class="sxs-lookup"><span data-stu-id="2ea90-140">DriveItem resource</span></span>

<span data-ttu-id="2ea90-141">Ресурсы [DriveItem](driveitem.md) представляют собой объекты в файловой системе диска.</span><span class="sxs-lookup"><span data-stu-id="2ea90-141">[DriveItems](driveitem.md) are the objects inside a drive's file system.</span></span>
<span data-ttu-id="2ea90-142">Доступ к ним можно получить по свойству **id** с использованием синтаксиса `/items/{item-id}` или по пути в файловой системе с использованием синтаксиса `/root:/path/to/item/`.</span><span class="sxs-lookup"><span data-stu-id="2ea90-142">DriveItems can be accessed by their id using the  syntax, or by their file system path using the  syntax.</span></span>

<span data-ttu-id="2ea90-143">У ресурсов DriveItem есть _аспекты_, предоставляющие данные об удостоверении и возможностях элемента.</span><span class="sxs-lookup"><span data-stu-id="2ea90-143">DriveItems have _facets_ that provide data about the item's identity and capabilities.</span></span>

<span data-ttu-id="2ea90-144">Ресурсы DriveItem с аспектом **folder** действуют как контейнеры элементов и содержат ссылку **children**, указывающую на коллекцию элементов в папке.</span><span class="sxs-lookup"><span data-stu-id="2ea90-144">DriveItems with a **folder** facet act as containers of items, and have a **children** reference, which points to a collection of items under the folder.</span></span>

## <a name="shared-folders-and-remote-items"></a><span data-ttu-id="2ea90-145">Общие папки и удаленные элементы</span><span class="sxs-lookup"><span data-stu-id="2ea90-145">Shared folders and remote items</span></span>

<span data-ttu-id="2ea90-146">Пользователь, у которого есть личная (не рабочая или учебная) учетная запись OneDrive, может добавить один или несколько общих элементов с другого диска в свое хранилище OneDrive.</span><span class="sxs-lookup"><span data-stu-id="2ea90-146">OneDrive personal users can add one or more shared items from another drive to their own OneDrive. These shared items appear as a DriveItem in the children collection with a remoteItem facet.</span></span>
<span data-ttu-id="2ea90-147">Эти общие элементы отображаются в коллекции **children** как экземпляры **DriveItem** с аспектом [remoteItem](remoteitem.md).</span><span class="sxs-lookup"><span data-stu-id="2ea90-147">OneDrive personal users can add one or more shared items from another drive to their own OneDrive. These shared items appear as a **DriveItem** in the **children** collection with a [remoteItem](remoteitem.md) facet.</span></span>

<span data-ttu-id="2ea90-148">Дополнительные сведения о работе с общими папками и удаленными элементами см. в [статье, посвященной общим папкам и удаленным элементам](remoteitem.md).</span><span class="sxs-lookup"><span data-stu-id="2ea90-148">For more information about working with shared folders and remote items, see [Remote items and shared folders](remoteitem.md).</span></span>   

## <a name="sharing-and-permissions"></a><span data-ttu-id="2ea90-149">Совместный доступ и разрешения</span><span class="sxs-lookup"><span data-stu-id="2ea90-149">Sharing and permissions</span></span>

<span data-ttu-id="2ea90-150">Одно из самых распространенных действий для OneDrive и библиотек документов SharePoint — предоставление общего доступа к содержимому.</span><span class="sxs-lookup"><span data-stu-id="2ea90-150">One of the most common actions for OneDrive and SharePoint document libraries is sharing content with other people. Microsoft Graph allows your app to create sharing links, add permissions and send invitations to items in a drive.</span></span>
<span data-ttu-id="2ea90-151">С помощью Microsoft Graph ваше приложение может создавать [ссылки для общего доступа](../api/driveitem_createlink.md), [добавлять разрешения и отправлять приглашения](../api/driveitem_invite.md) для доступа к элементам на диске.</span><span class="sxs-lookup"><span data-stu-id="2ea90-151">One of the most common actions for OneDrive and SharePoint document libraries is sharing content with other people. Microsoft Graph allows your app to create [sharing links](../api/driveitem_createlink.md), [add permissions and send invitations](../api/driveitem_invite.md) to items in a drive.</span></span>

<span data-ttu-id="2ea90-152">Кроме того, с помощью Microsoft Graph ваше приложение может [получать доступ к общему содержимому](../api/shares_get.md) непосредственно по ссылке для совместного доступа.</span><span class="sxs-lookup"><span data-stu-id="2ea90-152">Microsoft Graph also provides a way for your app to [access shared content](../api/shares_get.md) directly from a sharing link.</span></span>

 
