---
title: Тип ресурса Фрибусеррор
description: Представляет сведения об ошибке при попытке получить доступ к пользователю, списку рассылки или ресурсу.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: harini84
ms.openlocfilehash: 565abb49b82a2d8fa41120a9df556113d790ed36
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973960"
---
# <a name="freebusyerror-resource-type"></a><span data-ttu-id="0c63e-103">Тип ресурса Фрибусеррор</span><span class="sxs-lookup"><span data-stu-id="0c63e-103">freeBusyError resource type</span></span>

<span data-ttu-id="0c63e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c63e-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c63e-105">Представляет сведения об ошибке при попытке получить доступ к пользователю, списку рассылки или ресурсу.</span><span class="sxs-lookup"><span data-stu-id="0c63e-105">Represents error information from attempting to get the availability of a user, distribution list, or resource.</span></span>

## <a name="properties"></a><span data-ttu-id="0c63e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="0c63e-106">Properties</span></span>
| <span data-ttu-id="0c63e-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="0c63e-107">Property</span></span>     | <span data-ttu-id="0c63e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="0c63e-108">Type</span></span>   |<span data-ttu-id="0c63e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0c63e-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c63e-110">message</span><span class="sxs-lookup"><span data-stu-id="0c63e-110">message</span></span> |<span data-ttu-id="0c63e-111">String</span><span class="sxs-lookup"><span data-stu-id="0c63e-111">String</span></span> |<span data-ttu-id="0c63e-112">Описание ошибки.</span><span class="sxs-lookup"><span data-stu-id="0c63e-112">Describes the error.</span></span> |
|<span data-ttu-id="0c63e-113">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="0c63e-113">responseCode</span></span> |<span data-ttu-id="0c63e-114">String</span><span class="sxs-lookup"><span data-stu-id="0c63e-114">String</span></span> |<span data-ttu-id="0c63e-115">Код ответа из запроса на доступность пользователя, списка рассылки или ресурса.</span><span class="sxs-lookup"><span data-stu-id="0c63e-115">The response code from querying for the availability of the user, distribution list, or resource.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="0c63e-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0c63e-116">JSON representation</span></span>

<span data-ttu-id="0c63e-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0c63e-117">The following is a JSON representation of the resource.</span></span>

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


