---
author: JeremyKelley
description: Ресурс baseItem — это абстрактный ресурс, который содержит общий набор свойств, которые являются общими для нескольких других типов ресурсов.
ms.date: 09/10/2017
title: baseItem
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 38e697e4a991871bd592cc891dcd131e845572fe
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013145"
---
# <a name="baseitem-resource-type"></a><span data-ttu-id="6b470-103">Тип ресурса baseItem</span><span class="sxs-lookup"><span data-stu-id="6b470-103">BaseItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b470-p101">**baseItem** — это абстрактный ресурс, который содержит стандартный набор свойств, также используемых несколькими другими типами ресурсов. Ниже перечислены ресурсы, производные от ресурса **baseItem**.</span><span class="sxs-lookup"><span data-stu-id="6b470-p101">The **baseItem** resource is an abstract resource that contains a common set of properties shared among several other resources types. Resources that derive from **baseItem** include:</span></span>

* [<span data-ttu-id="6b470-106">drive</span><span class="sxs-lookup"><span data-stu-id="6b470-106">drive</span></span>](drive.md)
* [<span data-ttu-id="6b470-107">driveItem</span><span class="sxs-lookup"><span data-stu-id="6b470-107">driveItem</span></span>](driveitem.md)
* [<span data-ttu-id="6b470-108">site</span><span class="sxs-lookup"><span data-stu-id="6b470-108">site</span></span>](site.md)
* [<span data-ttu-id="6b470-109">sharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="6b470-109">sharedDriveItem</span></span>](shareddriveitem.md)

## <a name="json-representation"></a><span data-ttu-id="6b470-110">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="6b470-110">JSON representation</span></span>

<span data-ttu-id="6b470-111">Ниже показано представление ресурса **baseItem** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6b470-111">Here is a JSON representation of a **baseItem** resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "createdBy", "lastModifiedBy", "description", "parentReference", "webUrl" ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.baseItem",
  "abstract": true
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

## <a name="properties"></a><span data-ttu-id="6b470-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="6b470-112">Properties</span></span>

| <span data-ttu-id="6b470-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="6b470-113">Property</span></span>             | <span data-ttu-id="6b470-114">Тип</span><span class="sxs-lookup"><span data-stu-id="6b470-114">Type</span></span>              | <span data-ttu-id="6b470-115">Описание</span><span class="sxs-lookup"><span data-stu-id="6b470-115">Description</span></span>                                                                            |
| :------------------- | :---------------- | :------------------------------------------------------------------------------------- |
| <span data-ttu-id="6b470-116">id</span><span class="sxs-lookup"><span data-stu-id="6b470-116">id</span></span>                   | <span data-ttu-id="6b470-117">строка</span><span class="sxs-lookup"><span data-stu-id="6b470-117">string</span></span>            | <span data-ttu-id="6b470-p102">Уникальный идентификатор диска. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6b470-p102">The unique identifier of the drive. Read-only.</span></span>                                         |
| <span data-ttu-id="6b470-120">createdBy</span><span class="sxs-lookup"><span data-stu-id="6b470-120">createdBy</span></span>            | <span data-ttu-id="6b470-121">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="6b470-121">[identitySet][]</span></span>   | <span data-ttu-id="6b470-p103">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6b470-p103">Identity of the user, device, or application which created the item. Read-only.</span></span>        |
| <span data-ttu-id="6b470-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6b470-124">createdDateTime</span></span>      | <span data-ttu-id="6b470-125">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b470-125">dateTimeOffset</span></span>    | <span data-ttu-id="6b470-p104">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6b470-p104">Date and time of item creation. Read-only.</span></span>                                             |
| <span data-ttu-id="6b470-128">eTag</span><span class="sxs-lookup"><span data-stu-id="6b470-128">eTag</span></span>                 | <span data-ttu-id="6b470-129">string</span><span class="sxs-lookup"><span data-stu-id="6b470-129">string</span></span>            | <span data-ttu-id="6b470-p105">ETag для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6b470-p105">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="6b470-132">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="6b470-132">lastModifiedBy</span></span>       | <span data-ttu-id="6b470-133">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="6b470-133">[identitySet][]</span></span>   | <span data-ttu-id="6b470-p106">Идентификатор пользователя, устройства или приложения, внесшего последние изменения в элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6b470-p106">Identity of the user, device, and application which last modified the item. Read-only.</span></span> |
| <span data-ttu-id="6b470-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6b470-136">lastModifiedDateTime</span></span> | <span data-ttu-id="6b470-137">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b470-137">dateTimeOffset</span></span>    | <span data-ttu-id="6b470-p107">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6b470-p107">Date and time the item was last modified. Read-only.</span></span>                                   |
| <span data-ttu-id="6b470-140">name</span><span class="sxs-lookup"><span data-stu-id="6b470-140">name</span></span>                 | <span data-ttu-id="6b470-141">string</span><span class="sxs-lookup"><span data-stu-id="6b470-141">string</span></span>            | <span data-ttu-id="6b470-p108">Имя элемента. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="6b470-p108">The name of the item. Read-write.</span></span>                                                      |
| <span data-ttu-id="6b470-144">parentReference</span><span class="sxs-lookup"><span data-stu-id="6b470-144">parentReference</span></span>      | <span data-ttu-id="6b470-145">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="6b470-145">[itemReference][]</span></span> | <span data-ttu-id="6b470-p109">Сведения о родительском элементе, если элемент выступает в роли родительского элемента. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="6b470-p109">Parent information, if the item has a parent. Read-write.</span></span>                              |
| <span data-ttu-id="6b470-148">webUrl</span><span class="sxs-lookup"><span data-stu-id="6b470-148">webUrl</span></span>               | <span data-ttu-id="6b470-149">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="6b470-149">string (url)</span></span>      | <span data-ttu-id="6b470-p110">URL-адрес для отображения ресурса в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6b470-p110">URL that displays the resource in the browser. Read-only.</span></span>                              |

[identitySet]: identityset.md
[itemReference]: itemreference.md

## <a name="remarks"></a><span data-ttu-id="6b470-154">Примечания</span><span class="sxs-lookup"><span data-stu-id="6b470-154">Remarks</span></span>

<span data-ttu-id="6b470-155">Тип `baseItem` не предназначен для непосредственного использования.</span><span class="sxs-lookup"><span data-stu-id="6b470-155">The `baseItem` type is not expected to be used directly.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/BaseItem",
  "suppressions": []
}
-->
