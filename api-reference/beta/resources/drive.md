---
author: JeremyKelley
ms.author: JeremyKelley
title: Тип ресурса drive
description: Ресурс drive представляет хранилище OneDrive пользователя или библиотеку документов в SharePoint
localization_priority: Priority
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 689c020a0c717fb395d13822c2c8de8f265988a3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012725"
---
# <a name="drive-resource-type"></a><span data-ttu-id="2ff6a-103">Тип ресурса drive</span><span class="sxs-lookup"><span data-stu-id="2ff6a-103">drive resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ff6a-104">Ресурс drive — объект верхнего уровня, представляющий хранилище OneDrive пользователя или библиотеку документов в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="2ff6a-104">The drive resource is the top level object representing a user's OneDrive or a document library in SharePoint.</span></span>

<span data-ttu-id="2ff6a-p101">Для пользователей OneDrive всегда будет доступен хотя бы один диск (диск по умолчанию). Для пользователей, у которых нет лицензии на OneDrive, такой диск может быть недоступен.</span><span class="sxs-lookup"><span data-stu-id="2ff6a-p101">OneDrive users will always have at least one drive available, their default drive. Users without a OneDrive license may not have a default drive available.</span></span>

## <a name="methods"></a><span data-ttu-id="2ff6a-107">Методы</span><span class="sxs-lookup"><span data-stu-id="2ff6a-107">Methods</span></span>

|                        <span data-ttu-id="2ff6a-108">Метод</span><span class="sxs-lookup"><span data-stu-id="2ff6a-108">Method</span></span>                              |         <span data-ttu-id="2ff6a-109">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="2ff6a-109">Return type</span></span>         | <span data-ttu-id="2ff6a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2ff6a-110">Description</span></span> |
| :--------------------------------------------------------- | :-------------------------- |-------------|
| <span data-ttu-id="2ff6a-111">[Получение объекта drive][drive-get]</span><span class="sxs-lookup"><span data-stu-id="2ff6a-111">[Get drive][drive-get]</span></span>                                     | <span data-ttu-id="2ff6a-112">drive</span><span class="sxs-lookup"><span data-stu-id="2ff6a-112">drive</span></span>                       | <span data-ttu-id="2ff6a-113">Получение метаданных о диске</span><span class="sxs-lookup"><span data-stu-id="2ff6a-113">Get metadata about a user's default drive on OneDrive.</span></span> |
| <span data-ttu-id="2ff6a-114">[Получение корня диска][item-get]</span><span class="sxs-lookup"><span data-stu-id="2ff6a-114">[Get drive root][item-get]</span></span>                                 | <span data-ttu-id="2ff6a-115">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="2ff6a-115">[driveItem][]</span></span>               | <span data-ttu-id="2ff6a-116">Получение корневой папки диска</span><span class="sxs-lookup"><span data-stu-id="2ff6a-116">Get root folder for a drive</span></span> |
| <span data-ttu-id="2ff6a-117">[Список действий][drive-activities]</span><span class="sxs-lookup"><span data-stu-id="2ff6a-117">[List activities][drive-activities]</span></span>                        | <span data-ttu-id="2ff6a-118">Коллекция [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="2ff6a-118">[itemActivity][] collection</span></span> | <span data-ttu-id="2ff6a-119">Получение списка действий, выполненных на диске</span><span class="sxs-lookup"><span data-stu-id="2ff6a-119">List activities that occurred under the drive</span></span> |
| <span data-ttu-id="2ff6a-120">[Список отслеживаемых элементов][drive-following]</span><span class="sxs-lookup"><span data-stu-id="2ff6a-120">[List followed Items][drive-following]</span></span>                     | <span data-ttu-id="2ff6a-121">Коллекция [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="2ff6a-121">[driveItem][] collection</span></span>    | <span data-ttu-id="2ff6a-122">Получение списка отслеживаемых объектов driveItems пользователя</span><span class="sxs-lookup"><span data-stu-id="2ff6a-122">List the user's followed driveItems</span></span> |
| <span data-ttu-id="2ff6a-123">[Список дочерних элементов][item-children]</span><span class="sxs-lookup"><span data-stu-id="2ff6a-123">[List children][item-children]</span></span>                             | <span data-ttu-id="2ff6a-124">Коллекция [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="2ff6a-124">[driveItem][] collection</span></span>    | <span data-ttu-id="2ff6a-125">Получение списка дочерних элементов корневой папки диска</span><span class="sxs-lookup"><span data-stu-id="2ff6a-125">List children of the root folder of a drive</span></span> |
| <span data-ttu-id="2ff6a-126">[Список изменений][item-changes]</span><span class="sxs-lookup"><span data-stu-id="2ff6a-126">[List changes][item-changes]</span></span>                               | <span data-ttu-id="2ff6a-127">Коллекция [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="2ff6a-127">[driveItem][] collection</span></span>    | <span data-ttu-id="2ff6a-128">Получение списка изменений для всех объектов driveItems в ресурсе Drive</span><span class="sxs-lookup"><span data-stu-id="2ff6a-128">List changes for all Items in the Drive</span></span> |
| <span data-ttu-id="2ff6a-129">[Search][item-search]</span><span class="sxs-lookup"><span data-stu-id="2ff6a-129">[Search][item-search]</span></span>                                      | <span data-ttu-id="2ff6a-130">Коллекция [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="2ff6a-130">[driveItem][] collection</span></span>    | <span data-ttu-id="2ff6a-131">Поиск объектов driveItems на диске</span><span class="sxs-lookup"><span data-stu-id="2ff6a-131">Search for driveItems in a drive</span></span> |
| [<span data-ttu-id="2ff6a-132">Получение специальной папки</span><span class="sxs-lookup"><span data-stu-id="2ff6a-132">Get special folder</span></span>](../api/drive-get-specialfolder.md)    | <span data-ttu-id="2ff6a-133">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="2ff6a-133">[driveItem][]</span></span>               | <span data-ttu-id="2ff6a-134">Доступ к специальной папке по ее каноническому имени</span><span class="sxs-lookup"><span data-stu-id="2ff6a-134">Access a special (named) folder in the user's OneDrive by its known name.</span></span> |


## <a name="properties"></a><span data-ttu-id="2ff6a-135">Свойства</span><span class="sxs-lookup"><span data-stu-id="2ff6a-135">Properties</span></span>

| <span data-ttu-id="2ff6a-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="2ff6a-136">Property</span></span>             | <span data-ttu-id="2ff6a-137">Тип</span><span class="sxs-lookup"><span data-stu-id="2ff6a-137">Type</span></span>                          | <span data-ttu-id="2ff6a-138">Описание</span><span class="sxs-lookup"><span data-stu-id="2ff6a-138">Description</span></span>                                                                                                                                                                                                                      |
| :------------------- | :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="2ff6a-139">createdBy</span><span class="sxs-lookup"><span data-stu-id="2ff6a-139">createdBy</span></span>            | <span data-ttu-id="2ff6a-140">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="2ff6a-140">[identitySet][]</span></span>               | <span data-ttu-id="2ff6a-p102">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2ff6a-p102">Identity of the user, device, or application which created the item. Read-only.</span></span>                                                                                                                                                  |
| <span data-ttu-id="2ff6a-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2ff6a-143">createdDateTime</span></span>      | <span data-ttu-id="2ff6a-144">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ff6a-144">dateTimeOffset</span></span>                | <span data-ttu-id="2ff6a-p103">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2ff6a-p103">Date and time of item creation. Read-only.</span></span>                                                                                                                                                                                       |
| <span data-ttu-id="2ff6a-147">description</span><span class="sxs-lookup"><span data-stu-id="2ff6a-147">description</span></span>          | <span data-ttu-id="2ff6a-148">String</span><span class="sxs-lookup"><span data-stu-id="2ff6a-148">String</span></span>                        | <span data-ttu-id="2ff6a-149">Предоставляет отображаемое для пользователя описание диска.</span><span class="sxs-lookup"><span data-stu-id="2ff6a-149">Provide a user-visible description of the drive.</span></span> <span data-ttu-id="2ff6a-150">Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="2ff6a-150">Read-write.</span></span>
| <span data-ttu-id="2ff6a-151">driveType</span><span class="sxs-lookup"><span data-stu-id="2ff6a-151">driveType</span></span>            | <span data-ttu-id="2ff6a-152">Строка</span><span class="sxs-lookup"><span data-stu-id="2ff6a-152">String</span></span>                        | <span data-ttu-id="2ff6a-p105">Описывает тип диска, представленного данным ресурсом. Для личных дисков OneDrive возвращается `personal`. В случае дисков OneDrive для бизнеса возвращается `business`. В случае библиотек документов SharePoint возвращается `documentLibrary`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2ff6a-p105">Describes the type of drive represented by this resource. OneDrive personal drives will return `personal`. OneDrive for Business will return `business`. SharePoint document libraries will return `documentLibrary`. Read-only.</span></span> |
| <span data-ttu-id="2ff6a-158">id</span><span class="sxs-lookup"><span data-stu-id="2ff6a-158">id</span></span>                   | <span data-ttu-id="2ff6a-159">String</span><span class="sxs-lookup"><span data-stu-id="2ff6a-159">String</span></span>                        | <span data-ttu-id="2ff6a-p106">Уникальный идентификатор диска. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2ff6a-p106">The unique identifier of the drive. Read-only.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="2ff6a-162">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="2ff6a-162">lastModifiedBy</span></span>       | <span data-ttu-id="2ff6a-163">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="2ff6a-163">[identitySet][]</span></span>               | <span data-ttu-id="2ff6a-p107">Идентификатор пользователя, устройства или приложения, внесшего последние изменения в элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2ff6a-p107">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                                                                                           |
| <span data-ttu-id="2ff6a-166">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2ff6a-166">lastModifiedDateTime</span></span> | <span data-ttu-id="2ff6a-167">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ff6a-167">dateTimeOffset</span></span>                | <span data-ttu-id="2ff6a-p108">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2ff6a-p108">Date and time the item was last modified. Read-only.</span></span>                                                                                                                                                                             |
| <span data-ttu-id="2ff6a-170">name</span><span class="sxs-lookup"><span data-stu-id="2ff6a-170">name</span></span>                 | <span data-ttu-id="2ff6a-171">string</span><span class="sxs-lookup"><span data-stu-id="2ff6a-171">string</span></span>                        | <span data-ttu-id="2ff6a-p109">Имя элемента. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="2ff6a-p109">The name of the item. Read-write.</span></span>                                                                                                                                                                                                |
| <span data-ttu-id="2ff6a-174">owner</span><span class="sxs-lookup"><span data-stu-id="2ff6a-174">owner</span></span>                | [<span data-ttu-id="2ff6a-175">identitySet</span><span class="sxs-lookup"><span data-stu-id="2ff6a-175">identitySet</span></span>](identityset.md) | <span data-ttu-id="2ff6a-p110">Необязательный параметр. Учетная запись пользователя, которому принадлежит диск. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2ff6a-p110">Optional. The user account that owns the drive. Read-only.</span></span>                                                                                                                                                                       |
| <span data-ttu-id="2ff6a-179">quota</span><span class="sxs-lookup"><span data-stu-id="2ff6a-179">quota</span></span>                | [<span data-ttu-id="2ff6a-180">quota</span><span class="sxs-lookup"><span data-stu-id="2ff6a-180">quota</span></span>](quota.md)             | <span data-ttu-id="2ff6a-p111">Необязательный параметр. Сведения о квоте на дисковое пространство. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2ff6a-p111">Optional. Information about the drive's storage space quota. Read-only.</span></span>                                                                                                                                                          |
| <span data-ttu-id="2ff6a-184">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="2ff6a-184">sharepointIds</span></span>        | <span data-ttu-id="2ff6a-185">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="2ff6a-185">[sharepointIds][]</span></span>             | <span data-ttu-id="2ff6a-p112">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2ff6a-p112">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                                                                                                                                                         |
| <span data-ttu-id="2ff6a-188">system</span><span class="sxs-lookup"><span data-stu-id="2ff6a-188">system</span></span>               | <span data-ttu-id="2ff6a-189">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="2ff6a-189">[systemFacet][]</span></span>               | <span data-ttu-id="2ff6a-190">Если имеется это свойство, оно указывает, что данным диском управляет система.</span><span class="sxs-lookup"><span data-stu-id="2ff6a-190">If present, indicates that this is a system-managed drive.</span></span> <span data-ttu-id="2ff6a-191">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2ff6a-191">Read-only.</span></span>
| <span data-ttu-id="2ff6a-192">webUrl</span><span class="sxs-lookup"><span data-stu-id="2ff6a-192">webUrl</span></span>               | <span data-ttu-id="2ff6a-193">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="2ff6a-193">string (url)</span></span>                  | <span data-ttu-id="2ff6a-p114">URL-адрес для отображения ресурса в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2ff6a-p114">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                                                                                        |

[identitySet]: identityset.md
[sharepointIds]: sharepointids.md
[systemFacet]: systemfacet.md

## <a name="relationships"></a><span data-ttu-id="2ff6a-199">Связи</span><span class="sxs-lookup"><span data-stu-id="2ff6a-199">Relationships</span></span>

| <span data-ttu-id="2ff6a-200">Отношение</span><span class="sxs-lookup"><span data-stu-id="2ff6a-200">Relationship</span></span> | <span data-ttu-id="2ff6a-201">Тип</span><span class="sxs-lookup"><span data-stu-id="2ff6a-201">Type</span></span>                                 | <span data-ttu-id="2ff6a-202">Описание</span><span class="sxs-lookup"><span data-stu-id="2ff6a-202">Description</span></span>
|:-------------|:-------------------------------------|:-----------------------
| <span data-ttu-id="2ff6a-203">activities</span><span class="sxs-lookup"><span data-stu-id="2ff6a-203">activities</span></span>   | <span data-ttu-id="2ff6a-204">Коллекция [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="2ff6a-204">[itemActivity][] collection</span></span>          | <span data-ttu-id="2ff6a-205">Список последних действий, выполненных для этого объекта drive.</span><span class="sxs-lookup"><span data-stu-id="2ff6a-205">The list of recent activities that took place under this drive.</span></span>
| <span data-ttu-id="2ff6a-206">bundles</span><span class="sxs-lookup"><span data-stu-id="2ff6a-206">Multiple bundles</span></span>      | <span data-ttu-id="2ff6a-207">Коллекция [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="2ff6a-207">[driveItem][] collection</span></span>             | <span data-ttu-id="2ff6a-208">Коллекция объектов [bundles][bundle] (альбомы и наборы общих элементов с множественным выбором).</span><span class="sxs-lookup"><span data-stu-id="2ff6a-208">Collection of [bundles][bundle] (albums and multi-select-shared sets of items).</span></span> <span data-ttu-id="2ff6a-209">Только в OneDrive для личного пользования.</span><span class="sxs-lookup"><span data-stu-id="2ff6a-209">Only in personal OneDrive.</span></span>
| <span data-ttu-id="2ff6a-210">following</span><span class="sxs-lookup"><span data-stu-id="2ff6a-210">following</span></span>    | <span data-ttu-id="2ff6a-211">Коллекция [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="2ff6a-211">[driveItem][] collection</span></span>             | <span data-ttu-id="2ff6a-212">Список элементов, которые отслеживает пользователь.</span><span class="sxs-lookup"><span data-stu-id="2ff6a-212">The list of items the user is following.</span></span> <span data-ttu-id="2ff6a-213">Только в OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="2ff6a-213">Only in OneDrive for Business.</span></span>
| <span data-ttu-id="2ff6a-214">items</span><span class="sxs-lookup"><span data-stu-id="2ff6a-214">items</span></span>        | <span data-ttu-id="2ff6a-215">Коллекция [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="2ff6a-215">[driveItem][] collection</span></span>             | <span data-ttu-id="2ff6a-p117">Все элементы, содержащиеся на диске. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="2ff6a-p117">All items contained in the drive. Read-only. Nullable.</span></span>
| <span data-ttu-id="2ff6a-219">root</span><span class="sxs-lookup"><span data-stu-id="2ff6a-219">root</span></span>         | <span data-ttu-id="2ff6a-220">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="2ff6a-220">[driveItem][]</span></span>                        | <span data-ttu-id="2ff6a-p118">Корневая папка на диске. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2ff6a-p118">The root folder of the drive. Read-only.</span></span>
| <span data-ttu-id="2ff6a-223">special</span><span class="sxs-lookup"><span data-stu-id="2ff6a-223">special</span></span>      | <span data-ttu-id="2ff6a-224">Коллекция [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="2ff6a-224">[driveItem][] collection</span></span>             | <span data-ttu-id="2ff6a-p119">Коллекция общих папок, доступных в OneDrive. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="2ff6a-p119">Collection of common folders available in OneDrive. Read-only. Nullable.</span></span>


## <a name="json-representation"></a><span data-ttu-id="2ff6a-228">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2ff6a-228">JSON representation</span></span>

<span data-ttu-id="2ff6a-229">Ниже показано представление ресурса Drive в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2ff6a-229">Here is a JSON representation of a Drive resource.</span></span>

<span data-ttu-id="2ff6a-230">Ресурс **drive** является производным от ресурса [**baseItem**](baseitem.md) и наследует его свойства.</span><span class="sxs-lookup"><span data-stu-id="2ff6a-230">The **drive** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "activities",
    "createdBy",
    "createdDateTime",
    "description",
    "lastModifiedBy",
    "lastModifiedDateTime",
    "name",
    "webUrl",
    "items",
    "root",
    "special",
    "system"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.drive"
}-->

```json
{
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "id": "string",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "string (timestamp)",
  "description": "string",
  "driveType": "personal | business | documentLibrary",
  "following": [{"@odata.type": "microsoft.graph.driveItem"}],
  "items": [{"@odata.type": "microsoft.graph.driveItem"}],
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "string (timestamp)",
  "name": "string",
  "owner": {"@odata.type": "microsoft.graph.identitySet"},
  "quota": {"@odata.type": "microsoft.graph.quota"},
  "root": {"@odata.type": "microsoft.graph.driveItem"},
  "special": [{"@odata.type": "microsoft.graph.driveItem"}],
  "system": {"@odata.type": "microsoft.graph.systemFacet"},
  "webUrl": "string",
  "sharepointIds": {"@odata.type": "microsoft.graph.sharepointIds"}
}
```


[bundle]: bundle.md
[driveItem]: driveItem.md
[itemActivity]: itemactivity.md
[item-resource]: driveitem.md
[identity-set]: identityset.md
[quota-facet]: quota.md
[drive-resource]: drive.md
[drive-activities]: ../api/activities-list.md
[drive-following]: ../api/drive-list-following.md
[drive-get]: ../api/drive-get.md
[item-get]: ../api/driveitem-get.md
[item-changes]: ../api/driveitem-delta.md
[item-search]: ../api/driveitem-search.md
[item-children]: ../api/driveitem-list-children.md


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Drive is a top level object for OneDrive API that provides access to the contents of a drive. ",
  "keywords": "drive,objects,resources",
  "section": "documentation",
  "tocPath": "Drives",
  "tocBookmarks": {
    "Resources/Drive": "#"
  },
  "suppressions": []
}
-->
