---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: baseItem
ms.openlocfilehash: bbfebd734407259c391cdb1ce74beb96dc74d8bf
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="baseitem-resource-type"></a><span data-ttu-id="2841a-102">Тип ресурса baseItem</span><span class="sxs-lookup"><span data-stu-id="2841a-102">BaseItem resource type</span></span>

<span data-ttu-id="2841a-p101">**baseItem** — это абстрактный ресурс, который содержит стандартный набор свойств, также используемых несколькими другими типами ресурсов. Ниже перечислены ресурсы, производные от ресурса **baseItem**.</span><span class="sxs-lookup"><span data-stu-id="2841a-p101">The **baseItem** resource is an abstract resource that contains a common set of properties shared among several other resources types. Resources that derive from **baseItem** include:</span></span>

* [<span data-ttu-id="2841a-105">drive</span><span class="sxs-lookup"><span data-stu-id="2841a-105">drive</span></span>](drive.md)
* [<span data-ttu-id="2841a-106">driveItem</span><span class="sxs-lookup"><span data-stu-id="2841a-106">DriveItem</span></span>](driveitem.md)
* [<span data-ttu-id="2841a-107">site</span><span class="sxs-lookup"><span data-stu-id="2841a-107">site</span></span>](site.md)
* [<span data-ttu-id="2841a-108">sharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="2841a-108">sharedDriveItem</span></span>](shareddriveitem.md)

## <a name="json-representation"></a><span data-ttu-id="2841a-109">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2841a-109">JSON representation</span></span>

<span data-ttu-id="2841a-110">Ниже показано представление ресурса **baseItem** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2841a-110">Here is a JSON representation of a **baseItem** resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "createdBy", "lastModifiedBy", "description", "parentReference", "webUrl" ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.baseItem"
}-->

```json
{
  "id": "string (identifier)",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "datetime",
  "description": "string",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "datetime",
  "name": "string",
  "parentReference": { "@odata.type": "microsoft.graph.itemReference" },
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="2841a-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="2841a-111">Properties</span></span>

| <span data-ttu-id="2841a-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="2841a-112">Property</span></span>             | <span data-ttu-id="2841a-113">Тип</span><span class="sxs-lookup"><span data-stu-id="2841a-113">Type</span></span>              | <span data-ttu-id="2841a-114">Описание</span><span class="sxs-lookup"><span data-stu-id="2841a-114">Description</span></span>                                                                            |
| :------------------- | :---------------- | :------------------------------------------------------------------------------------- |
| <span data-ttu-id="2841a-115">id</span><span class="sxs-lookup"><span data-stu-id="2841a-115">id</span></span>                   | <span data-ttu-id="2841a-116">string</span><span class="sxs-lookup"><span data-stu-id="2841a-116">string</span></span>            | <span data-ttu-id="2841a-p102">Уникальный идентификатор диска. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2841a-p102">The unique identifier of the drive. Read-only.</span></span>                                         |
| <span data-ttu-id="2841a-119">createdBy</span><span class="sxs-lookup"><span data-stu-id="2841a-119">createdBy</span></span>            | <span data-ttu-id="2841a-120">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="2841a-120">[identitySet][]</span></span>   | <span data-ttu-id="2841a-p103">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2841a-p103">Identity of the user, device, or application which created the item. Read-only.</span></span>        |
| <span data-ttu-id="2841a-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2841a-123">createdDateTime</span></span>      | <span data-ttu-id="2841a-124">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2841a-124">dateTimeOffset</span></span>    | <span data-ttu-id="2841a-p104">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2841a-p104">Date and time of item creation. Read-only.</span></span>                                             |
| <span data-ttu-id="2841a-127">eTag</span><span class="sxs-lookup"><span data-stu-id="2841a-127">eTag</span></span>                 | <span data-ttu-id="2841a-128">string</span><span class="sxs-lookup"><span data-stu-id="2841a-128">string</span></span>            | <span data-ttu-id="2841a-p105">ETag для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2841a-p105">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="2841a-131">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="2841a-131">lastModifiedBy</span></span>       | <span data-ttu-id="2841a-132">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="2841a-132">[identitySet][]</span></span>   | <span data-ttu-id="2841a-p106">Идентификатор пользователя, устройства или приложения, внесшего последние изменения в элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2841a-p106">Identity of the user, device, and application which last modified the item. Read-only.</span></span> |
| <span data-ttu-id="2841a-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2841a-135">lastModifiedDateTime</span></span> | <span data-ttu-id="2841a-136">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2841a-136">dateTimeOffset</span></span>    | <span data-ttu-id="2841a-p107">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2841a-p107">Date and time the item was last modified. Read-only.</span></span>                                   |
| <span data-ttu-id="2841a-139">name</span><span class="sxs-lookup"><span data-stu-id="2841a-139">name</span></span>                 | <span data-ttu-id="2841a-140">string</span><span class="sxs-lookup"><span data-stu-id="2841a-140">string</span></span>            | <span data-ttu-id="2841a-p108">Имя элемента. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="2841a-p108">The name of the item. Read-write.</span></span>                                                      |
| <span data-ttu-id="2841a-143">parentReference</span><span class="sxs-lookup"><span data-stu-id="2841a-143">parentReference</span></span>      | <span data-ttu-id="2841a-144">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="2841a-144">[itemReference][]</span></span> | <span data-ttu-id="2841a-p109">Сведения о родительском элементе, если элемент выступает в роли родительского элемента. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="2841a-p109">Parent information, if the item has a parent. Read-write.</span></span>                              |
| <span data-ttu-id="2841a-147">webUrl</span><span class="sxs-lookup"><span data-stu-id="2841a-147">webUrl</span></span>               | <span data-ttu-id="2841a-148">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="2841a-148">string (url)</span></span>      | <span data-ttu-id="2841a-p110">URL-адрес для отображения ресурса в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2841a-p110">URL that displays the resource in the browser. Read-only.</span></span>                              |

[identitySet]: identityset.md
[itemReference]: itemreference.md

## <a name="remarks"></a><span data-ttu-id="2841a-153">Примечания</span><span class="sxs-lookup"><span data-stu-id="2841a-153">Remarks</span></span>

<span data-ttu-id="2841a-154">Тип `baseItem` не предназначен для непосредственного использования.</span><span class="sxs-lookup"><span data-stu-id="2841a-154">The `baseItem` type is not expected to be used directly.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/BaseItem"
} -->
