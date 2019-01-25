---
title: Тип ресурса oneNoteIdentitySet
description: '**Поддержка готовится к выпуску**'
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: e149d5548ce3585bbcda1f0a199fa97d7543af77
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516716"
---
# <a name="onenoteidentityset-resource-type"></a><span data-ttu-id="f83b5-103">Тип ресурса oneNoteIdentitySet</span><span class="sxs-lookup"><span data-stu-id="f83b5-103">oneNoteIdentitySet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f83b5-104">**Поддержка готовится к выпуску**</span><span class="sxs-lookup"><span data-stu-id="f83b5-104">**Support coming soon**</span></span>

<span data-ttu-id="f83b5-105">Тип OneNoteIdentitySet — с ключом коллекцию объектов [OneNoteIdentity](onenoteidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="f83b5-105">The OneNoteIdentitySet type is a keyed collection of [OneNoteIdentity](onenoteidentity.md) objects.</span></span>
<span data-ttu-id="f83b5-106">Он используется для представления набора удостоверения, связанные с различные события для _записной книжки_, _раздел_ или _страницы_, например, _созданные_ или _Кем изменено_.</span><span class="sxs-lookup"><span data-stu-id="f83b5-106">It is used to represent a set of identities associated with various events for a _Notebook_, _Section_ or _Page_, such as _created by_ or _last modified by_.</span></span> 
 
<span data-ttu-id="f83b5-107">В настоящее время в нем ключей и одного _**пользователя**_.</span><span class="sxs-lookup"><span data-stu-id="f83b5-107">Currently it contains a single key, _**user**_.</span></span>  <span data-ttu-id="f83b5-108">В будущем могут быть добавлены разделы, такие как устройство или приложение для изменения элемента.</span><span class="sxs-lookup"><span data-stu-id="f83b5-108">In future, keys such as the device or application to change the item may be added.</span></span>

<span data-ttu-id="f83b5-109">В будущем этого типа будут объединены с [IdentitySet](identityset.md)</span><span class="sxs-lookup"><span data-stu-id="f83b5-109">In future, this type will be merged with [IdentitySet](identityset.md)</span></span>

## <a name="json-representation"></a><span data-ttu-id="f83b5-110">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f83b5-110">JSON representation</span></span>

<span data-ttu-id="f83b5-111">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f83b5-111">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteidentityset"
}-->

```json
{
  "user": {"@odata.type": "microsoft.graph.oneNoteIdentity"}
}

```
## <a name="properties"></a><span data-ttu-id="f83b5-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="f83b5-112">Properties</span></span>
| <span data-ttu-id="f83b5-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="f83b5-113">Property</span></span>     | <span data-ttu-id="f83b5-114">Тип</span><span class="sxs-lookup"><span data-stu-id="f83b5-114">Type</span></span>   |<span data-ttu-id="f83b5-115">Описание</span><span class="sxs-lookup"><span data-stu-id="f83b5-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f83b5-116">user</span><span class="sxs-lookup"><span data-stu-id="f83b5-116">user</span></span>|[<span data-ttu-id="f83b5-117">oneNoteIdentity</span><span class="sxs-lookup"><span data-stu-id="f83b5-117">oneNoteIdentity</span></span>](onenoteidentity.md)|<span data-ttu-id="f83b5-118">Ресурс OneNoteIdentity, представляющий пользователя.</span><span class="sxs-lookup"><span data-stu-id="f83b5-118">A OneNoteIdentity resource that represents a user.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oneNoteIdentitySet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onenoteidentityset.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
