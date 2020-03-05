---
title: Тип ресурса Оненотеидентити
description: '**Поддержка скоро**'
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: ad578dcfa54f51484aa7e29ad5c3ade8a9195b61
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522360"
---
# <a name="onenoteidentity-resource-type"></a><span data-ttu-id="f68d8-103">Тип ресурса Оненотеидентити</span><span class="sxs-lookup"><span data-stu-id="f68d8-103">oneNoteIdentity resource type</span></span>

<span data-ttu-id="f68d8-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f68d8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f68d8-105">**Поддержка скоро**</span><span class="sxs-lookup"><span data-stu-id="f68d8-105">**Support coming soon**</span></span>

<span data-ttu-id="f68d8-106">Тип Оненотеидентити представляет идентификатор _пользователя_.</span><span class="sxs-lookup"><span data-stu-id="f68d8-106">The OneNoteIdentity type represents an identity of a _user_.</span></span>

<span data-ttu-id="f68d8-107">В дальнейшем этот тип будет объединен с [удостоверением](identity.md)</span><span class="sxs-lookup"><span data-stu-id="f68d8-107">In future, this type will be merged with [identity](identity.md)</span></span>


## <a name="json-representation"></a><span data-ttu-id="f68d8-108">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f68d8-108">JSON representation</span></span>

<span data-ttu-id="f68d8-109">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f68d8-109">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteIdentity"
}-->

```json
{
  "displayName": "string",
  "id": "string"
}

```
## <a name="properties"></a><span data-ttu-id="f68d8-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="f68d8-110">Properties</span></span>
| <span data-ttu-id="f68d8-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="f68d8-111">Property</span></span>     | <span data-ttu-id="f68d8-112">Тип</span><span class="sxs-lookup"><span data-stu-id="f68d8-112">Type</span></span>   |<span data-ttu-id="f68d8-113">Описание</span><span class="sxs-lookup"><span data-stu-id="f68d8-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f68d8-114">displayName</span><span class="sxs-lookup"><span data-stu-id="f68d8-114">displayName</span></span>|<span data-ttu-id="f68d8-115">string</span><span class="sxs-lookup"><span data-stu-id="f68d8-115">string</span></span>|<span data-ttu-id="f68d8-116">Отображаемое имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="f68d8-116">The identity's display name.</span></span>|
|<span data-ttu-id="f68d8-117">id</span><span class="sxs-lookup"><span data-stu-id="f68d8-117">id</span></span>|<span data-ttu-id="f68d8-118">строка</span><span class="sxs-lookup"><span data-stu-id="f68d8-118">string</span></span>|<span data-ttu-id="f68d8-119">Уникальный идентификатор удостоверения.</span><span class="sxs-lookup"><span data-stu-id="f68d8-119">Unique identifier for the identity.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oneNoteIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
