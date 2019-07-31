---
title: Тип ресурса Експрессионинпутобжект
description: 'Представляет объект, который будет использоваться в качестве входных тестовых данных, когда действие [синчронизатионсчема: парсикспрессион](../api/synchronization_synchronizationschema_parseexpression.md) выполняет оценку выражения.'
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 113c38e540b8c41fb3d3156b27f6f5e1f1df42f2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007951"
---
# <a name="expressioninputobject-resource-type"></a><span data-ttu-id="e1ab8-103">Тип ресурса Експрессионинпутобжект</span><span class="sxs-lookup"><span data-stu-id="e1ab8-103">expressionInputObject resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1ab8-104">Представляет объект, который будет использоваться в качестве входных тестовых данных, когда действие [парсикспрессион](../api/synchronization-synchronizationschema-parseexpression.md) выполняет оценку выражения.</span><span class="sxs-lookup"><span data-stu-id="e1ab8-104">Represents an object to be used as input test data when the [parseExpression](../api/synchronization-synchronizationschema-parseexpression.md) action performs an expression evaluation.</span></span>

## <a name="properties"></a><span data-ttu-id="e1ab8-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="e1ab8-105">Properties</span></span>
| <span data-ttu-id="e1ab8-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="e1ab8-106">Property</span></span>     | <span data-ttu-id="e1ab8-107">Тип</span><span class="sxs-lookup"><span data-stu-id="e1ab8-107">Type</span></span>   |<span data-ttu-id="e1ab8-108">Описание</span><span class="sxs-lookup"><span data-stu-id="e1ab8-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e1ab8-109">RDLC</span><span class="sxs-lookup"><span data-stu-id="e1ab8-109">definition</span></span>|[<span data-ttu-id="e1ab8-110">Обжектдефинитион</span><span class="sxs-lookup"><span data-stu-id="e1ab8-110">objectDefinition</span></span>](synchronization-objectdefinition.md)|<span data-ttu-id="e1ab8-111">Определение тестового объекта.</span><span class="sxs-lookup"><span data-stu-id="e1ab8-111">Definition of the test object.</span></span>|
|<span data-ttu-id="e1ab8-112">properties</span><span class="sxs-lookup"><span data-stu-id="e1ab8-112">properties</span></span>|<span data-ttu-id="e1ab8-113">Коллекция [стрингкэйобжектвалуепаир](synchronization-stringkeyobjectvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="e1ab8-113">[stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md) collection</span></span>|<span data-ttu-id="e1ab8-114">Значения свойств тестового объекта.</span><span class="sxs-lookup"><span data-stu-id="e1ab8-114">Property values of the test object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e1ab8-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e1ab8-115">JSON representation</span></span>

<span data-ttu-id="e1ab8-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e1ab8-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.expressionInputObject"
}-->

```json
{
  "definition": {"@odata.type": "microsoft.graph.objectDefinition"},
  "properties": [{"@odata.type": "microsoft.graph.stringKeyObjectValuePair"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "expressionInputObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
