---
title: Тип ресурса oneNoteIdentitySet
description: '**Поддержка готовится к выпуску**'
localization_priority: Normal
ms.openlocfilehash: d2969d073503a9fd586641abeb3d82f719db8545
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874090"
---
# <a name="onenoteidentityset-resource-type"></a><span data-ttu-id="225f4-103">Тип ресурса oneNoteIdentitySet</span><span class="sxs-lookup"><span data-stu-id="225f4-103">oneNoteIdentitySet resource type</span></span>

> <span data-ttu-id="225f4-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="225f4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="225f4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="225f4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="225f4-106">**Поддержка готовится к выпуску**</span><span class="sxs-lookup"><span data-stu-id="225f4-106">**Support coming soon**</span></span>

<span data-ttu-id="225f4-107">Тип OneNoteIdentitySet — с ключом коллекцию объектов [OneNoteIdentity](onenoteidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="225f4-107">The OneNoteIdentitySet type is a keyed collection of [OneNoteIdentity](onenoteidentity.md) objects.</span></span>
<span data-ttu-id="225f4-108">Он используется для представления набора удостоверения, связанные с различные события для _записной книжки_, _раздел_ или _страницы_, например, _созданные_ или _Кем изменено_.</span><span class="sxs-lookup"><span data-stu-id="225f4-108">It is used to represent a set of identities associated with various events for a _Notebook_, _Section_ or _Page_, such as _created by_ or _last modified by_.</span></span> 
 
<span data-ttu-id="225f4-109">В настоящее время в нем ключей и одного _**пользователя**_.</span><span class="sxs-lookup"><span data-stu-id="225f4-109">Currently it contains a single key, _**user**_.</span></span>  <span data-ttu-id="225f4-110">В будущем могут быть добавлены разделы, такие как устройство или приложение для изменения элемента.</span><span class="sxs-lookup"><span data-stu-id="225f4-110">In future, keys such as the device or application to change the item may be added.</span></span>

<span data-ttu-id="225f4-111">В будущем этого типа будут объединены с [IdentitySet](identityset.md)</span><span class="sxs-lookup"><span data-stu-id="225f4-111">In future, this type will be merged with [IdentitySet](identityset.md)</span></span>

## <a name="json-representation"></a><span data-ttu-id="225f4-112">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="225f4-112">JSON representation</span></span>

<span data-ttu-id="225f4-113">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="225f4-113">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="225f4-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="225f4-114">Properties</span></span>
| <span data-ttu-id="225f4-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="225f4-115">Property</span></span>     | <span data-ttu-id="225f4-116">Тип</span><span class="sxs-lookup"><span data-stu-id="225f4-116">Type</span></span>   |<span data-ttu-id="225f4-117">Описание</span><span class="sxs-lookup"><span data-stu-id="225f4-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="225f4-118">user</span><span class="sxs-lookup"><span data-stu-id="225f4-118">user</span></span>|[<span data-ttu-id="225f4-119">oneNoteIdentity</span><span class="sxs-lookup"><span data-stu-id="225f4-119">oneNoteIdentity</span></span>](onenoteidentity.md)|<span data-ttu-id="225f4-120">Ресурс OneNoteIdentity, представляющий пользователя.</span><span class="sxs-lookup"><span data-stu-id="225f4-120">A OneNoteIdentity resource that represents a user.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "oneNoteIdentitySet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
