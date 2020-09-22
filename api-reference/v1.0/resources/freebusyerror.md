---
title: Тип ресурса Фрибусеррор
description: Представляет сведения об ошибке при попытке получить доступ к пользователю, списку рассылки или ресурсу.
localization_priority: Normal
author: harini84
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: b161d47ff7a89c79a04e9400ff0d4756692f49c9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018234"
---
# <a name="freebusyerror-resource-type"></a><span data-ttu-id="1493b-103">Тип ресурса Фрибусеррор</span><span class="sxs-lookup"><span data-stu-id="1493b-103">freeBusyError resource type</span></span>

<span data-ttu-id="1493b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1493b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1493b-105">Представляет сведения об ошибке при попытке получить доступ к пользователю, списку рассылки или ресурсу.</span><span class="sxs-lookup"><span data-stu-id="1493b-105">Represents error information from attempting to get the availability of a user, distribution list, or resource.</span></span>

## <a name="properties"></a><span data-ttu-id="1493b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="1493b-106">Properties</span></span>
| <span data-ttu-id="1493b-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="1493b-107">Property</span></span>     | <span data-ttu-id="1493b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="1493b-108">Type</span></span>   |<span data-ttu-id="1493b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1493b-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1493b-110">message</span><span class="sxs-lookup"><span data-stu-id="1493b-110">message</span></span> |<span data-ttu-id="1493b-111">String</span><span class="sxs-lookup"><span data-stu-id="1493b-111">String</span></span> |<span data-ttu-id="1493b-112">Описание ошибки.</span><span class="sxs-lookup"><span data-stu-id="1493b-112">Describes the error.</span></span> |
|<span data-ttu-id="1493b-113">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="1493b-113">responseCode</span></span> |<span data-ttu-id="1493b-114">String</span><span class="sxs-lookup"><span data-stu-id="1493b-114">String</span></span> |<span data-ttu-id="1493b-115">Код ответа из запроса на доступность пользователя, списка рассылки или ресурса.</span><span class="sxs-lookup"><span data-stu-id="1493b-115">The response code from querying for the availability of the user, distribution list, or resource.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="1493b-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1493b-116">JSON representation</span></span>

<span data-ttu-id="1493b-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1493b-117">The following is a JSON representation of the resource.</span></span>

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

