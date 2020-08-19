---
title: Тип ресурса Фрибусеррор
description: Представляет сведения об ошибке при попытке получить доступ к пользователю, списку рассылки или ресурсу.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: harini84
ms.openlocfilehash: e259685415a37e89429b5e0522e89a4fbe2f9fd2
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809539"
---
# <a name="freebusyerror-resource-type"></a><span data-ttu-id="3cb13-103">Тип ресурса Фрибусеррор</span><span class="sxs-lookup"><span data-stu-id="3cb13-103">freeBusyError resource type</span></span>

<span data-ttu-id="3cb13-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3cb13-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3cb13-105">Представляет сведения об ошибке при попытке получить доступ к пользователю, списку рассылки или ресурсу.</span><span class="sxs-lookup"><span data-stu-id="3cb13-105">Represents error information from attempting to get the availability of a user, distribution list, or resource.</span></span>

## <a name="properties"></a><span data-ttu-id="3cb13-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="3cb13-106">Properties</span></span>
| <span data-ttu-id="3cb13-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="3cb13-107">Property</span></span>     | <span data-ttu-id="3cb13-108">Тип</span><span class="sxs-lookup"><span data-stu-id="3cb13-108">Type</span></span>   |<span data-ttu-id="3cb13-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3cb13-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3cb13-110">message</span><span class="sxs-lookup"><span data-stu-id="3cb13-110">message</span></span> |<span data-ttu-id="3cb13-111">String</span><span class="sxs-lookup"><span data-stu-id="3cb13-111">String</span></span> |<span data-ttu-id="3cb13-112">Описание ошибки.</span><span class="sxs-lookup"><span data-stu-id="3cb13-112">Describes the error.</span></span> |
|<span data-ttu-id="3cb13-113">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="3cb13-113">responseCode</span></span> |<span data-ttu-id="3cb13-114">String</span><span class="sxs-lookup"><span data-stu-id="3cb13-114">String</span></span> |<span data-ttu-id="3cb13-115">Код ответа из запроса на доступность пользователя, списка рассылки или ресурса.</span><span class="sxs-lookup"><span data-stu-id="3cb13-115">The response code from querying for the availability of the user, distribution list, or resource.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="3cb13-116">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3cb13-116">JSON representation</span></span>

<span data-ttu-id="3cb13-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3cb13-117">The following is a JSON representation of the resource.</span></span>

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
