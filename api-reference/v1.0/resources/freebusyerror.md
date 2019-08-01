---
title: Тип ресурса Фрибусеррор
description: Представляет сведения об ошибке при попытке получить доступ к пользователю, списку рассылки или ресурсу.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ca306ba5a40ffc08147c8e8449ab03bf51afd745
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030284"
---
# <a name="freebusyerror-resource-type"></a><span data-ttu-id="988a2-103">Тип ресурса Фрибусеррор</span><span class="sxs-lookup"><span data-stu-id="988a2-103">freeBusyError resource type</span></span>

<span data-ttu-id="988a2-104">Представляет сведения об ошибке при попытке получить доступ к пользователю, списку рассылки или ресурсу.</span><span class="sxs-lookup"><span data-stu-id="988a2-104">Represents error information from attempting to get the availability of a user, distribution list, or resource.</span></span>

## <a name="properties"></a><span data-ttu-id="988a2-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="988a2-105">Properties</span></span>
| <span data-ttu-id="988a2-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="988a2-106">Property</span></span>     | <span data-ttu-id="988a2-107">Тип</span><span class="sxs-lookup"><span data-stu-id="988a2-107">Type</span></span>   |<span data-ttu-id="988a2-108">Описание</span><span class="sxs-lookup"><span data-stu-id="988a2-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="988a2-109">message</span><span class="sxs-lookup"><span data-stu-id="988a2-109">message</span></span> |<span data-ttu-id="988a2-110">String</span><span class="sxs-lookup"><span data-stu-id="988a2-110">String</span></span> |<span data-ttu-id="988a2-111">Описание ошибки.</span><span class="sxs-lookup"><span data-stu-id="988a2-111">Describes the error.</span></span> |
|<span data-ttu-id="988a2-112">Респонсекоде</span><span class="sxs-lookup"><span data-stu-id="988a2-112">responseCode</span></span> |<span data-ttu-id="988a2-113">String</span><span class="sxs-lookup"><span data-stu-id="988a2-113">String</span></span> |<span data-ttu-id="988a2-114">Код ответа из запроса на доступность пользователя, списка рассылки или ресурса.</span><span class="sxs-lookup"><span data-stu-id="988a2-114">The response code from querying for the availability of the user, distribution list, or resource.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="988a2-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="988a2-115">JSON representation</span></span>

<span data-ttu-id="988a2-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="988a2-116">The following is a JSON representation of the resource.</span></span>

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
