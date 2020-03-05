---
author: JeremyKelley
description: Ресурс baseItem — это абстрактный ресурс, который содержит общий набор свойств, которые являются общими для нескольких других типов ресурсов.
ms.date: 09/10/2017
title: baseItem
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 5d72147602872478578b39617c77b227a27124b4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508033"
---
# <a name="baseitem-resource-type"></a><span data-ttu-id="db3ac-103">Тип ресурса baseItem</span><span class="sxs-lookup"><span data-stu-id="db3ac-103">BaseItem resource type</span></span>

<span data-ttu-id="db3ac-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="db3ac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db3ac-p101">**baseItem** — это абстрактный ресурс, который содержит стандартный набор свойств, также используемых несколькими другими типами ресурсов. Ниже перечислены ресурсы, производные от ресурса **baseItem**.</span><span class="sxs-lookup"><span data-stu-id="db3ac-p101">The **baseItem** resource is an abstract resource that contains a common set of properties shared among several other resources types. Resources that derive from **baseItem** include:</span></span>

* [<span data-ttu-id="db3ac-107">drive</span><span class="sxs-lookup"><span data-stu-id="db3ac-107">drive</span></span>](drive.md)
* [<span data-ttu-id="db3ac-108">driveItem</span><span class="sxs-lookup"><span data-stu-id="db3ac-108">driveItem</span></span>](driveitem.md)
* [<span data-ttu-id="db3ac-109">site</span><span class="sxs-lookup"><span data-stu-id="db3ac-109">site</span></span>](site.md)
* [<span data-ttu-id="db3ac-110">sharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="db3ac-110">sharedDriveItem</span></span>](shareddriveitem.md)

## <a name="json-representation"></a><span data-ttu-id="db3ac-111">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="db3ac-111">JSON representation</span></span>

<span data-ttu-id="db3ac-112">Ниже показано представление ресурса **baseItem** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="db3ac-112">Here is a JSON representation of a **baseItem** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="db3ac-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="db3ac-113">Properties</span></span>

| <span data-ttu-id="db3ac-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="db3ac-114">Property</span></span>             | <span data-ttu-id="db3ac-115">Тип</span><span class="sxs-lookup"><span data-stu-id="db3ac-115">Type</span></span>              | <span data-ttu-id="db3ac-116">Описание</span><span class="sxs-lookup"><span data-stu-id="db3ac-116">Description</span></span>                                                                            |
| :------------------- | :---------------- | :------------------------------------------------------------------------------------- |
| <span data-ttu-id="db3ac-117">id</span><span class="sxs-lookup"><span data-stu-id="db3ac-117">id</span></span>                   | <span data-ttu-id="db3ac-118">строка</span><span class="sxs-lookup"><span data-stu-id="db3ac-118">string</span></span>            | <span data-ttu-id="db3ac-p102">Уникальный идентификатор диска. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="db3ac-p102">The unique identifier of the drive. Read-only.</span></span>                                         |
| <span data-ttu-id="db3ac-121">createdBy</span><span class="sxs-lookup"><span data-stu-id="db3ac-121">createdBy</span></span>            | <span data-ttu-id="db3ac-122">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="db3ac-122">[identitySet][]</span></span>   | <span data-ttu-id="db3ac-p103">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="db3ac-p103">Identity of the user, device, or application which created the item. Read-only.</span></span>        |
| <span data-ttu-id="db3ac-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="db3ac-125">createdDateTime</span></span>      | <span data-ttu-id="db3ac-126">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db3ac-126">dateTimeOffset</span></span>    | <span data-ttu-id="db3ac-p104">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="db3ac-p104">Date and time of item creation. Read-only.</span></span>                                             |
| <span data-ttu-id="db3ac-129">eTag</span><span class="sxs-lookup"><span data-stu-id="db3ac-129">eTag</span></span>                 | <span data-ttu-id="db3ac-130">string</span><span class="sxs-lookup"><span data-stu-id="db3ac-130">string</span></span>            | <span data-ttu-id="db3ac-p105">ETag для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="db3ac-p105">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="db3ac-133">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="db3ac-133">lastModifiedBy</span></span>       | <span data-ttu-id="db3ac-134">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="db3ac-134">[identitySet][]</span></span>   | <span data-ttu-id="db3ac-p106">Идентификатор пользователя, устройства или приложения, внесшего последние изменения в элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="db3ac-p106">Identity of the user, device, and application which last modified the item. Read-only.</span></span> |
| <span data-ttu-id="db3ac-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="db3ac-137">lastModifiedDateTime</span></span> | <span data-ttu-id="db3ac-138">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db3ac-138">dateTimeOffset</span></span>    | <span data-ttu-id="db3ac-p107">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="db3ac-p107">Date and time the item was last modified. Read-only.</span></span>                                   |
| <span data-ttu-id="db3ac-141">name</span><span class="sxs-lookup"><span data-stu-id="db3ac-141">name</span></span>                 | <span data-ttu-id="db3ac-142">string</span><span class="sxs-lookup"><span data-stu-id="db3ac-142">string</span></span>            | <span data-ttu-id="db3ac-p108">Имя элемента. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="db3ac-p108">The name of the item. Read-write.</span></span>                                                      |
| <span data-ttu-id="db3ac-145">parentReference</span><span class="sxs-lookup"><span data-stu-id="db3ac-145">parentReference</span></span>      | <span data-ttu-id="db3ac-146">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="db3ac-146">[itemReference][]</span></span> | <span data-ttu-id="db3ac-p109">Сведения о родительском элементе, если элемент выступает в роли родительского элемента. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="db3ac-p109">Parent information, if the item has a parent. Read-write.</span></span>                              |
| <span data-ttu-id="db3ac-149">webUrl</span><span class="sxs-lookup"><span data-stu-id="db3ac-149">webUrl</span></span>               | <span data-ttu-id="db3ac-150">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="db3ac-150">string (url)</span></span>      | <span data-ttu-id="db3ac-p110">URL-адрес для отображения ресурса в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="db3ac-p110">URL that displays the resource in the browser. Read-only.</span></span>                              |

[identitySet]: identityset.md
[itemReference]: itemreference.md

## <a name="remarks"></a><span data-ttu-id="db3ac-155">Примечания</span><span class="sxs-lookup"><span data-stu-id="db3ac-155">Remarks</span></span>

<span data-ttu-id="db3ac-156">Тип `baseItem` не предназначен для непосредственного использования.</span><span class="sxs-lookup"><span data-stu-id="db3ac-156">The `baseItem` type is not expected to be used directly.</span></span>

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
