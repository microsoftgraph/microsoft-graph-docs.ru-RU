---
title: Тип ресурса Оненотеидентитисет
description: '**Поддержка скоро**'
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 9ffbc20a73aaed885d118094a7d1946459eb7efc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009365"
---
# <a name="onenoteidentityset-resource-type"></a><span data-ttu-id="5ae7f-103">Тип ресурса Оненотеидентитисет</span><span class="sxs-lookup"><span data-stu-id="5ae7f-103">oneNoteIdentitySet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ae7f-104">**Поддержка скоро**</span><span class="sxs-lookup"><span data-stu-id="5ae7f-104">**Support coming soon**</span></span>

<span data-ttu-id="5ae7f-105">Тип Оненотеидентитисет является коллекцией с ключами объектов [оненотеидентити](onenoteidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="5ae7f-105">The OneNoteIdentitySet type is a keyed collection of [OneNoteIdentity](onenoteidentity.md) objects.</span></span>
<span data-ttu-id="5ae7f-106">Он используется для представления набора удостоверений, связанных с различными событиями для _записной книжки_, _раздела_ или _страницы_, например _созданных автором_ или автором _последнего изменения_.</span><span class="sxs-lookup"><span data-stu-id="5ae7f-106">It is used to represent a set of identities associated with various events for a _Notebook_, _Section_ or _Page_, such as _created by_ or _last modified by_.</span></span> 
 
<span data-ttu-id="5ae7f-107">В настоящее время он содержит один ключ, _**User**_.</span><span class="sxs-lookup"><span data-stu-id="5ae7f-107">Currently it contains a single key, _**user**_.</span></span>  <span data-ttu-id="5ae7f-108">В дальнейшем можно добавить такие ключи, как устройство или приложение для изменения элемента.</span><span class="sxs-lookup"><span data-stu-id="5ae7f-108">In future, keys such as the device or application to change the item may be added.</span></span>

<span data-ttu-id="5ae7f-109">В дальнейшем этот тип будет объединен с [Identity](identityset.md)</span><span class="sxs-lookup"><span data-stu-id="5ae7f-109">In future, this type will be merged with [IdentitySet](identityset.md)</span></span>

## <a name="json-representation"></a><span data-ttu-id="5ae7f-110">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5ae7f-110">JSON representation</span></span>

<span data-ttu-id="5ae7f-111">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5ae7f-111">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteIdentityset"
}-->

```json
{
  "user": {"@odata.type": "microsoft.graph.onenoteIdentity"}
}

```
## <a name="properties"></a><span data-ttu-id="5ae7f-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="5ae7f-112">Properties</span></span>
| <span data-ttu-id="5ae7f-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="5ae7f-113">Property</span></span>     | <span data-ttu-id="5ae7f-114">Тип</span><span class="sxs-lookup"><span data-stu-id="5ae7f-114">Type</span></span>   |<span data-ttu-id="5ae7f-115">Описание</span><span class="sxs-lookup"><span data-stu-id="5ae7f-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5ae7f-116">user</span><span class="sxs-lookup"><span data-stu-id="5ae7f-116">user</span></span>|[<span data-ttu-id="5ae7f-117">Оненотеидентити</span><span class="sxs-lookup"><span data-stu-id="5ae7f-117">oneNoteIdentity</span></span>](onenoteidentity.md)|<span data-ttu-id="5ae7f-118">Ресурс Оненотеидентити, представляющий пользователя.</span><span class="sxs-lookup"><span data-stu-id="5ae7f-118">A OneNoteIdentity resource that represents a user.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oneNoteIdentitySet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
