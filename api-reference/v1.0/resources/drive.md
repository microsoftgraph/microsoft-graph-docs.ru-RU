---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Drive
ms.openlocfilehash: 0b178967f7eb8da8bdf8584bb13a7d4f9950392b
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="drive-resource-type"></a><span data-ttu-id="855b0-102">Тип ресурса Drive</span><span class="sxs-lookup"><span data-stu-id="855b0-102">Drive resource type</span></span>

<span data-ttu-id="855b0-103">Ресурс Drive — объект верхнего уровня, представляющий хранилище OneDrive пользователя или библиотеку документов в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="855b0-103">The drive resource is the top level object representing a user's OneDrive or a document library in SharePoint.</span></span>

<span data-ttu-id="855b0-p101">Для пользователей OneDrive всегда будет доступен хотя бы один диск (диск по умолчанию). Для пользователей, у которых нет лицензии на OneDrive, такой диск может быть недоступен.</span><span class="sxs-lookup"><span data-stu-id="855b0-p101">OneDrive users will always have at least one drive available, their default drive. Users without a OneDrive license may not have a default drive available.</span></span>

## <a name="json-representation"></a><span data-ttu-id="855b0-106">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="855b0-106">JSON representation</span></span>

<span data-ttu-id="855b0-107">Ниже показано представление ресурса Drive в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="855b0-107">Here is a JSON representation of a Drive resource.</span></span>

<span data-ttu-id="855b0-108">Ресурс **drive** является производным от ресурса [**baseItem**](baseitem.md) и наследует его свойства.</span><span class="sxs-lookup"><span data-stu-id="855b0-108">The **drive** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

<!-- { "blockType": "resource", 
       "@odata.type": "microsoft.graph.drive",
       "keyProperty": "id", 
       "optionalProperties": [ "activities", "createdBy", "createdDateTime", "description", "lastModifiedBy", "lastModifiedDateTime", "name", "webUrl", "items", "root", "special", "system"] } -->

```json
{
  "id": "string",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "string (timestamp)",
  "description": "string",
  "driveType": "personal | business | documentLibrary",
  "items": [ { "@odata.type": "microsoft.graph.driveItem" } ],
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "string (timestamp)",
  "name": "string",
  "owner": { "@odata.type": "microsoft.graph.identitySet" },
  "quota": { "@odata.type": "microsoft.graph.quota" },
  "root": { "@odata.type": "microsoft.graph.driveItem" },
  "special": [ { "@odata.type": "microsoft.graph.driveItem" }],
  "system": { "@odata.type": "microsoft.graph.systemFacet" },
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="855b0-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="855b0-109">Properties</span></span>

| <span data-ttu-id="855b0-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="855b0-110">Property</span></span>             | <span data-ttu-id="855b0-111">Тип</span><span class="sxs-lookup"><span data-stu-id="855b0-111">Type</span></span>                          | <span data-ttu-id="855b0-112">Описание</span><span class="sxs-lookup"><span data-stu-id="855b0-112">Description</span></span>                                                                                                                                                                                                                      |
| :------------------- | :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="855b0-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="855b0-113">createdBy</span></span>            | <span data-ttu-id="855b0-114">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="855b0-114">[identitySet][]</span></span>               | <span data-ttu-id="855b0-p102">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="855b0-p102">Identity of the user, device, or application which created the item. Read-only.</span></span>                                                                                                                                                  |
| <span data-ttu-id="855b0-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="855b0-117">createdDateTime</span></span>      | <span data-ttu-id="855b0-118">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="855b0-118">dateTimeOffset</span></span>                | <span data-ttu-id="855b0-p103">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="855b0-p103">Date and time of item creation. Read-only.</span></span>                                                                                                                                                                                       |
| <span data-ttu-id="855b0-121">description</span><span class="sxs-lookup"><span data-stu-id="855b0-121">description</span></span>          | <span data-ttu-id="855b0-122">String</span><span class="sxs-lookup"><span data-stu-id="855b0-122">String</span></span>                        | <span data-ttu-id="855b0-123">Предоставляет отображаемое для пользователя описание диска.</span><span class="sxs-lookup"><span data-stu-id="855b0-123">Provide a user-visible description of the drive.</span></span> <span data-ttu-id="855b0-124">Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="855b0-124">Read-write.</span></span>
| <span data-ttu-id="855b0-125">driveType</span><span class="sxs-lookup"><span data-stu-id="855b0-125">driveType</span></span>            | <span data-ttu-id="855b0-126">Строка</span><span class="sxs-lookup"><span data-stu-id="855b0-126">String</span></span>                        | <span data-ttu-id="855b0-p105">Описывает тип диска, представленного данным ресурсом. Для личных дисков OneDrive возвращается `personal`. В случае дисков OneDrive для бизнеса возвращается `business`. В случае библиотек документов SharePoint возвращается `documentLibrary`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="855b0-p105">Describes the type of drive represented by this resource. OneDrive personal drives will return `personal`. OneDrive for Business will return `business`. SharePoint document libraries will return `documentLibrary`. Read-only.</span></span> |
| <span data-ttu-id="855b0-132">id</span><span class="sxs-lookup"><span data-stu-id="855b0-132">id</span></span>                   | <span data-ttu-id="855b0-133">String</span><span class="sxs-lookup"><span data-stu-id="855b0-133">String</span></span>                        | <span data-ttu-id="855b0-p106">Уникальный идентификатор диска. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="855b0-p106">The unique identifier of the drive. Read-only.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="855b0-136">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="855b0-136">lastModifiedBy</span></span>       | <span data-ttu-id="855b0-137">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="855b0-137">[identitySet][]</span></span>               | <span data-ttu-id="855b0-p107">Идентификатор пользователя, устройства или приложения, внесшего последние изменения в элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="855b0-p107">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                                                                                           |
| <span data-ttu-id="855b0-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="855b0-140">lastModifiedDateTime</span></span> | <span data-ttu-id="855b0-141">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="855b0-141">dateTimeOffset</span></span>                | <span data-ttu-id="855b0-p108">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="855b0-p108">Date and time the item was last modified. Read-only.</span></span>                                                                                                                                                                             |
| <span data-ttu-id="855b0-144">name</span><span class="sxs-lookup"><span data-stu-id="855b0-144">name</span></span>                 | <span data-ttu-id="855b0-145">string</span><span class="sxs-lookup"><span data-stu-id="855b0-145">string</span></span>                        | <span data-ttu-id="855b0-p109">Имя элемента. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="855b0-p109">The name of the item. Read-write.</span></span>                                                                                                                                                                                                |
| <span data-ttu-id="855b0-148">owner</span><span class="sxs-lookup"><span data-stu-id="855b0-148">owner</span></span>                | [<span data-ttu-id="855b0-149">identitySet</span><span class="sxs-lookup"><span data-stu-id="855b0-149">identitySet</span></span>](identityset.md) | <span data-ttu-id="855b0-p110">Необязательный параметр. Учетная запись пользователя, которому принадлежит диск. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="855b0-p110">Optional. The user account that owns the drive. Read-only.</span></span>                                                                                                                                                                       |
| <span data-ttu-id="855b0-153">quota</span><span class="sxs-lookup"><span data-stu-id="855b0-153">quota</span></span>                | [<span data-ttu-id="855b0-154">quota</span><span class="sxs-lookup"><span data-stu-id="855b0-154">quota</span></span>](quota.md)             | <span data-ttu-id="855b0-p111">Необязательный параметр. Сведения о квоте на дисковое пространство. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="855b0-p111">Optional. Information about the drive's storage space quota. Read-only.</span></span>                                                                                                                                                          |
| <span data-ttu-id="855b0-158">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="855b0-158">sharepointIds</span></span>        | <span data-ttu-id="855b0-159">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="855b0-159">[sharepointIds][]</span></span>             | <span data-ttu-id="855b0-p112">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="855b0-p112">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                                                                                                                                                         |
| <span data-ttu-id="855b0-162">system</span><span class="sxs-lookup"><span data-stu-id="855b0-162">System</span></span>               | <span data-ttu-id="855b0-163">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="855b0-163">[systemFacet][]</span></span>               | <span data-ttu-id="855b0-164">Если имеется это свойство, оно указывает, что данным диском управляет система.</span><span class="sxs-lookup"><span data-stu-id="855b0-164">If present, indicates that this is a system-managed drive.</span></span> <span data-ttu-id="855b0-165">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="855b0-165">Read-only.</span></span>
| <span data-ttu-id="855b0-166">webUrl</span><span class="sxs-lookup"><span data-stu-id="855b0-166">webUrl</span></span>               | <span data-ttu-id="855b0-167">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="855b0-167">string (url)</span></span>                  | <span data-ttu-id="855b0-p114">URL-адрес для отображения ресурса в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="855b0-p114">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                                                                                        |

[identitySet]: identityset.md
[sharepointIds]: sharepointids.md
[systemFacet]: systemfacet.md

## <a name="relationships"></a><span data-ttu-id="855b0-173">Связи</span><span class="sxs-lookup"><span data-stu-id="855b0-173">Relationships</span></span>

| <span data-ttu-id="855b0-174">Связь</span><span class="sxs-lookup"><span data-stu-id="855b0-174">Relationship</span></span> | <span data-ttu-id="855b0-175">Тип</span><span class="sxs-lookup"><span data-stu-id="855b0-175">Type</span></span>                                 | <span data-ttu-id="855b0-176">Описание</span><span class="sxs-lookup"><span data-stu-id="855b0-176">Description</span></span>
|:-------------|:-------------------------------------|:-----------------------
| <span data-ttu-id="855b0-177">items</span><span class="sxs-lookup"><span data-stu-id="855b0-177">items</span></span>        | <span data-ttu-id="855b0-178">Коллекция [driveitem](driveitem.md)</span><span class="sxs-lookup"><span data-stu-id="855b0-178">[driveitem](driveitem.md) collection</span></span> | <span data-ttu-id="855b0-p115">Все элементы, содержащиеся на диске. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="855b0-p115">All items contained in the drive. Read-only. Nullable.</span></span>
| <span data-ttu-id="855b0-182">root</span><span class="sxs-lookup"><span data-stu-id="855b0-182">root</span></span>         | [<span data-ttu-id="855b0-183">driveitem</span><span class="sxs-lookup"><span data-stu-id="855b0-183">driveitem</span></span>](driveitem.md)            | <span data-ttu-id="855b0-p116">Корневая папка на диске. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="855b0-p116">The root folder of the drive. Read-only.</span></span>
| <span data-ttu-id="855b0-186">special</span><span class="sxs-lookup"><span data-stu-id="855b0-186">special</span></span>      | <span data-ttu-id="855b0-187">Коллекция [driveitem](driveitem.md)</span><span class="sxs-lookup"><span data-stu-id="855b0-187">[driveitem](driveitem.md) collection</span></span> | <span data-ttu-id="855b0-p117">Коллекция общих папок, доступных в OneDrive. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="855b0-p117">Collection of common folders available in OneDrive. Read-only. Nullable.</span></span>

## <a name="methods"></a><span data-ttu-id="855b0-191">Методы</span><span class="sxs-lookup"><span data-stu-id="855b0-191">Methods</span></span>

|                        <span data-ttu-id="855b0-192">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="855b0-192">Common task</span></span>                         |         <span data-ttu-id="855b0-193">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="855b0-193">HTTP method</span></span>         |
| :--------------------------------------------------------- | :-------------------------- |
| <span data-ttu-id="855b0-194">[Получение метаданных другого ресурса Drive][drive-get]</span><span class="sxs-lookup"><span data-stu-id="855b0-194">[Get Drive metadata of another Drive][drive-get]</span></span>           | `GET /drives/{drive-id}`    |
| <span data-ttu-id="855b0-195">[Получение корневой папки для ресурса Drive, используемого по умолчанию, пользователя][item-get]</span><span class="sxs-lookup"><span data-stu-id="855b0-195">[Get root folder for user's default Drive][item-get]</span></span>       | `GET /drive/root`           |
| <span data-ttu-id="855b0-196">[Получение списка дочерних элементов ресурса Drive][item-children]</span><span class="sxs-lookup"><span data-stu-id="855b0-196">[List children under the Drive][item-children]</span></span>             | `GET /drive/root/children`  |
| <span data-ttu-id="855b0-197">[Получение списка изменений для всех элементов в ресурсе Drive][item-changes]</span><span class="sxs-lookup"><span data-stu-id="855b0-197">[List changes for all Items in the Drive][item-changes]</span></span>    | `GET /drive/root/delta`     |
| <span data-ttu-id="855b0-198">[Поиск элементов в ресурсе Drive][item-search]</span><span class="sxs-lookup"><span data-stu-id="855b0-198">[Search for Items in the Drive][item-search]</span></span>               | `GET /drive/root/search`    |
| [<span data-ttu-id="855b0-199">Доступ к специальной папке</span><span class="sxs-lookup"><span data-stu-id="855b0-199">Access special folder</span></span>](../api/drive_get_specialfolder.md) | `GET /drive/special/{name}` |

<span data-ttu-id="855b0-200">В примерах в предыдущей таблице используется каталог `/drive`, но можно использовать и другие пути.</span><span class="sxs-lookup"><span data-stu-id="855b0-200">In the previous table, the examples use , but  is valid too.</span></span>

[item-resource]: driveitem.md
[identity-set]: identityset.md
[quota-facet]: quota.md
[drive-resource]: drive.md
[drive-get]: ../api/drive_get.md
[item-get]: ../api/driveitem_get.md
[item-changes]: ../api/driveitem_delta.md
[item-search]: ../api/driveitem_search.md
[item-children]: ../api/driveitem_list_children.md


<!-- {
  "type": "#page.annotation",
  "description": "Drive is a top level object for OneDrive API that provides access to the contents of a drive. ",
  "keywords": "drive,objects,resources",
  "section": "documentation",
  "tocPath": "Drives",
  "tocBookmarks": { "Resources/Drive": "#" }
} -->
