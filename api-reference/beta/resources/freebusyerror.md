---
title: Тип ресурса Фрибусеррор
description: Представляет сведения об ошибке при попытке получить доступ к пользователю, списку рассылки или ресурсу.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 82350bc8cfeece76e0cd5c6873810988194cfb01
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971965"
---
# <a name="freebusyerror-resource-type"></a><span data-ttu-id="1507f-103">Тип ресурса Фрибусеррор</span><span class="sxs-lookup"><span data-stu-id="1507f-103">freeBusyError resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="1507f-104">Представляет сведения об ошибке при попытке получить доступ к пользователю, списку рассылки или ресурсу.</span><span class="sxs-lookup"><span data-stu-id="1507f-104">Represents error information from attempting to get the availability of a user, distribution list, or resource.</span></span>

## <a name="properties"></a><span data-ttu-id="1507f-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="1507f-105">Properties</span></span>
| <span data-ttu-id="1507f-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="1507f-106">Property</span></span>     | <span data-ttu-id="1507f-107">Тип</span><span class="sxs-lookup"><span data-stu-id="1507f-107">Type</span></span>   |<span data-ttu-id="1507f-108">Описание</span><span class="sxs-lookup"><span data-stu-id="1507f-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1507f-109">message</span><span class="sxs-lookup"><span data-stu-id="1507f-109">message</span></span> |<span data-ttu-id="1507f-110">String</span><span class="sxs-lookup"><span data-stu-id="1507f-110">String</span></span> |<span data-ttu-id="1507f-111">Описание ошибки.</span><span class="sxs-lookup"><span data-stu-id="1507f-111">Describes the error.</span></span> |
|<span data-ttu-id="1507f-112">Респонсекоде</span><span class="sxs-lookup"><span data-stu-id="1507f-112">responseCode</span></span> |<span data-ttu-id="1507f-113">String</span><span class="sxs-lookup"><span data-stu-id="1507f-113">String</span></span> |<span data-ttu-id="1507f-114">Код ответа из запроса на доступность пользователя, списка рассылки или ресурса.</span><span class="sxs-lookup"><span data-stu-id="1507f-114">The response code from querying for the availability of the user, distribution list, or resource.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="1507f-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1507f-115">JSON representation</span></span>

<span data-ttu-id="1507f-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1507f-116">The following is a JSON representation of the resource.</span></span>

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
  "tocPath": "",
  "suppressions": []
}
-->
