---
title: Тип ресурса Експрессионинпутобжект
description: Представляет объект, который будет использоваться в качестве входных тестовых данных, когда действие Синчронизатионсчема Парсикспрессион выполняет оценку выражения.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e9727f50b05eb8cdb5319883dd0058a91d9383cc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47968361"
---
# <a name="expressioninputobject-resource-type"></a><span data-ttu-id="89f5e-103">Тип ресурса Експрессионинпутобжект</span><span class="sxs-lookup"><span data-stu-id="89f5e-103">expressionInputObject resource type</span></span>

<span data-ttu-id="89f5e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89f5e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89f5e-105">Представляет объект, который будет использоваться в качестве входных тестовых данных, когда действие [парсикспрессион](../api/synchronization-synchronizationschema-parseexpression.md) выполняет оценку выражения.</span><span class="sxs-lookup"><span data-stu-id="89f5e-105">Represents an object to be used as input test data when the [parseExpression](../api/synchronization-synchronizationschema-parseexpression.md) action performs an expression evaluation.</span></span>

## <a name="properties"></a><span data-ttu-id="89f5e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="89f5e-106">Properties</span></span>
| <span data-ttu-id="89f5e-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="89f5e-107">Property</span></span>     | <span data-ttu-id="89f5e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="89f5e-108">Type</span></span>   |<span data-ttu-id="89f5e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="89f5e-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="89f5e-110">RDLC</span><span class="sxs-lookup"><span data-stu-id="89f5e-110">definition</span></span>|[<span data-ttu-id="89f5e-111">обжектдефинитион</span><span class="sxs-lookup"><span data-stu-id="89f5e-111">objectDefinition</span></span>](synchronization-objectdefinition.md)|<span data-ttu-id="89f5e-112">Определение тестового объекта.</span><span class="sxs-lookup"><span data-stu-id="89f5e-112">Definition of the test object.</span></span>|
|<span data-ttu-id="89f5e-113">properties</span><span class="sxs-lookup"><span data-stu-id="89f5e-113">properties</span></span>|<span data-ttu-id="89f5e-114">Коллекция [стрингкэйобжектвалуепаир](synchronization-stringkeyobjectvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="89f5e-114">[stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md) collection</span></span>|<span data-ttu-id="89f5e-115">Значения свойств тестового объекта.</span><span class="sxs-lookup"><span data-stu-id="89f5e-115">Property values of the test object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="89f5e-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="89f5e-116">JSON representation</span></span>

<span data-ttu-id="89f5e-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="89f5e-117">The following is a JSON representation of the resource.</span></span>

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


