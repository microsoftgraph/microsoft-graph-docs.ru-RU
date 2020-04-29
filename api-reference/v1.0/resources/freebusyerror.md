---
title: Тип ресурса Фрибусеррор
description: Представляет сведения об ошибке при попытке получить доступ к пользователю, списку рассылки или ресурсу.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 8e069aef1d26a409e9ebe29a516136a952604ee6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531387"
---
# <a name="freebusyerror-resource-type"></a><span data-ttu-id="e0622-103">Тип ресурса Фрибусеррор</span><span class="sxs-lookup"><span data-stu-id="e0622-103">freeBusyError resource type</span></span>

<span data-ttu-id="e0622-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0622-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e0622-105">Представляет сведения об ошибке при попытке получить доступ к пользователю, списку рассылки или ресурсу.</span><span class="sxs-lookup"><span data-stu-id="e0622-105">Represents error information from attempting to get the availability of a user, distribution list, or resource.</span></span>

## <a name="properties"></a><span data-ttu-id="e0622-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e0622-106">Properties</span></span>
| <span data-ttu-id="e0622-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e0622-107">Property</span></span>     | <span data-ttu-id="e0622-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e0622-108">Type</span></span>   |<span data-ttu-id="e0622-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e0622-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e0622-110">message</span><span class="sxs-lookup"><span data-stu-id="e0622-110">message</span></span> |<span data-ttu-id="e0622-111">String</span><span class="sxs-lookup"><span data-stu-id="e0622-111">String</span></span> |<span data-ttu-id="e0622-112">Описание ошибки.</span><span class="sxs-lookup"><span data-stu-id="e0622-112">Describes the error.</span></span> |
|<span data-ttu-id="e0622-113">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="e0622-113">responseCode</span></span> |<span data-ttu-id="e0622-114">String</span><span class="sxs-lookup"><span data-stu-id="e0622-114">String</span></span> |<span data-ttu-id="e0622-115">Код ответа из запроса на доступность пользователя, списка рассылки или ресурса.</span><span class="sxs-lookup"><span data-stu-id="e0622-115">The response code from querying for the availability of the user, distribution list, or resource.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="e0622-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e0622-116">JSON representation</span></span>

<span data-ttu-id="e0622-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e0622-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.freeBusyError"
}-->

```json
{
  "message": "String",
  "responseCode": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "freeBusyError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->
