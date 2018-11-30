---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: baseItem
ms.openlocfilehash: d70a75be0be4d7ecbd010288cb313b8394736932
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082748"
---
# <a name="baseitem-resource-type"></a><span data-ttu-id="278fd-102">Тип ресурса baseItem</span><span class="sxs-lookup"><span data-stu-id="278fd-102">BaseItem resource type</span></span>

> <span data-ttu-id="278fd-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="278fd-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="278fd-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="278fd-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="278fd-p102">**baseItem** — это абстрактный ресурс, который содержит стандартный набор свойств, также используемых несколькими другими типами ресурсов. Ниже перечислены ресурсы, производные от ресурса **baseItem**.</span><span class="sxs-lookup"><span data-stu-id="278fd-p102">The **baseItem** resource is an abstract resource that contains a common set of properties shared among several other resources types. Resources that derive from **baseItem** include:</span></span>

* [<span data-ttu-id="278fd-107">drive</span><span class="sxs-lookup"><span data-stu-id="278fd-107">drive</span></span>](drive.md)
* [<span data-ttu-id="278fd-108">driveItem</span><span class="sxs-lookup"><span data-stu-id="278fd-108">driveItem</span></span>](driveitem.md)
* [<span data-ttu-id="278fd-109">site</span><span class="sxs-lookup"><span data-stu-id="278fd-109">site</span></span>](site.md)
* [<span data-ttu-id="278fd-110">sharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="278fd-110">sharedDriveItem</span></span>](shareddriveitem.md)

## <a name="json-representation"></a><span data-ttu-id="278fd-111">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="278fd-111">JSON representation</span></span>

<span data-ttu-id="278fd-112">Ниже показано представление ресурса **baseItem** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="278fd-112">Here is a JSON representation of a **baseItem** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="278fd-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="278fd-113">Properties</span></span>

| <span data-ttu-id="278fd-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="278fd-114">Property</span></span>             | <span data-ttu-id="278fd-115">Тип</span><span class="sxs-lookup"><span data-stu-id="278fd-115">Type</span></span>              | <span data-ttu-id="278fd-116">Описание</span><span class="sxs-lookup"><span data-stu-id="278fd-116">Description</span></span>                                                                            |
| :------------------- | :---------------- | :------------------------------------------------------------------------------------- |
| <span data-ttu-id="278fd-117">id</span><span class="sxs-lookup"><span data-stu-id="278fd-117">id</span></span>                   | <span data-ttu-id="278fd-118">строка</span><span class="sxs-lookup"><span data-stu-id="278fd-118">string</span></span>            | <span data-ttu-id="278fd-p103">Уникальный идентификатор диска. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="278fd-p103">The unique identifier of the drive. Read-only.</span></span>                                         |
| <span data-ttu-id="278fd-121">createdBy</span><span class="sxs-lookup"><span data-stu-id="278fd-121">createdBy</span></span>            | <span data-ttu-id="278fd-122">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="278fd-122">[identitySet][]</span></span>   | <span data-ttu-id="278fd-p104">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="278fd-p104">Identity of the user, device, or application which created the item. Read-only.</span></span>        |
| <span data-ttu-id="278fd-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="278fd-125">createdDateTime</span></span>      | <span data-ttu-id="278fd-126">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="278fd-126">dateTimeOffset</span></span>    | <span data-ttu-id="278fd-p105">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="278fd-p105">Date and time of item creation. Read-only.</span></span>                                             |
| <span data-ttu-id="278fd-129">eTag</span><span class="sxs-lookup"><span data-stu-id="278fd-129">eTag</span></span>                 | <span data-ttu-id="278fd-130">string</span><span class="sxs-lookup"><span data-stu-id="278fd-130">string</span></span>            | <span data-ttu-id="278fd-p106">ETag для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="278fd-p106">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="278fd-133">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="278fd-133">lastModifiedBy</span></span>       | <span data-ttu-id="278fd-134">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="278fd-134">[identitySet][]</span></span>   | <span data-ttu-id="278fd-p107">Идентификатор пользователя, устройства или приложения, внесшего последние изменения в элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="278fd-p107">Identity of the user, device, and application which last modified the item. Read-only.</span></span> |
| <span data-ttu-id="278fd-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="278fd-137">lastModifiedDateTime</span></span> | <span data-ttu-id="278fd-138">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="278fd-138">dateTimeOffset</span></span>    | <span data-ttu-id="278fd-p108">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="278fd-p108">Date and time the item was last modified. Read-only.</span></span>                                   |
| <span data-ttu-id="278fd-141">name</span><span class="sxs-lookup"><span data-stu-id="278fd-141">name</span></span>                 | <span data-ttu-id="278fd-142">строка</span><span class="sxs-lookup"><span data-stu-id="278fd-142">string</span></span>            | <span data-ttu-id="278fd-p109">Имя элемента. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="278fd-p109">The name of the item. Read-write.</span></span>                                                      |
| <span data-ttu-id="278fd-145">parentReference</span><span class="sxs-lookup"><span data-stu-id="278fd-145">parentReference</span></span>      | <span data-ttu-id="278fd-146">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="278fd-146">[itemReference][]</span></span> | <span data-ttu-id="278fd-p110">Сведения о родительском элементе, если элемент выступает в роли родительского элемента. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="278fd-p110">Parent information, if the item has a parent. Read-write.</span></span>                              |
| <span data-ttu-id="278fd-149">webUrl</span><span class="sxs-lookup"><span data-stu-id="278fd-149">webUrl</span></span>               | <span data-ttu-id="278fd-150">строка (url-адрес)</span><span class="sxs-lookup"><span data-stu-id="278fd-150">string (url)</span></span>      | <span data-ttu-id="278fd-p111">URL-адрес для отображения ресурса в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="278fd-p111">URL that displays the resource in the browser. Read-only.</span></span>                              |

[identitySet]: identityset.md
[itemReference]: itemreference.md

## <a name="remarks"></a><span data-ttu-id="278fd-155">Примечания</span><span class="sxs-lookup"><span data-stu-id="278fd-155">Remarks</span></span>

<span data-ttu-id="278fd-156">Тип `baseItem` не предназначен для непосредственного использования.</span><span class="sxs-lookup"><span data-stu-id="278fd-156">The `baseItem` type is not expected to be used directly.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/BaseItem"
} -->
