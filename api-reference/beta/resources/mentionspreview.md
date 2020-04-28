---
title: Тип ресурса Ментионспревиев
description: Представляет сведения об упоминании объектов в экземпляре ресурса.
localization_priority: Normal
author: simonhult
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 4658f152d478e4df0a0e492bdd9272f0cd9170ca
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522689"
---
# <a name="mentionspreview-resource-type"></a><span data-ttu-id="a783d-103">Тип ресурса Ментионспревиев</span><span class="sxs-lookup"><span data-stu-id="a783d-103">mentionsPreview resource type</span></span>

<span data-ttu-id="a783d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a783d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a783d-105">Представляет сведения об [упоминании](../resources/mention.md) объектов в экземпляре ресурса.</span><span class="sxs-lookup"><span data-stu-id="a783d-105">Represents information about [mention](../resources/mention.md) objects in a resource instance.</span></span>

## <a name="properties"></a><span data-ttu-id="a783d-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a783d-106">Properties</span></span>
| <span data-ttu-id="a783d-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a783d-107">Property</span></span>     | <span data-ttu-id="a783d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a783d-108">Type</span></span>   |<span data-ttu-id="a783d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a783d-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a783d-110">Упомянутые</span><span class="sxs-lookup"><span data-stu-id="a783d-110">isMentioned</span></span> | <span data-ttu-id="a783d-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="a783d-111">Boolean</span></span> | <span data-ttu-id="a783d-112">Имеет значение true, если пользователь, вошедшего в систему, упоминается в родительском экземпляре ресурса.</span><span class="sxs-lookup"><span data-stu-id="a783d-112">True if the signed-in user is mentioned in the parent resource instance.</span></span> <span data-ttu-id="a783d-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a783d-113">Read-only.</span></span> <span data-ttu-id="a783d-114">Поддерживает фильтр.</span><span class="sxs-lookup"><span data-stu-id="a783d-114">Supports filter.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a783d-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a783d-115">JSON representation</span></span>

<span data-ttu-id="a783d-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a783d-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mentionsPreview"
}-->

```json
{
  "isMentioned": "Boolean"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mentionsPreview resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
