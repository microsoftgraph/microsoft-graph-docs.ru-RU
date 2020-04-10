---
title: Тип ресурса Експрессионинпутобжект
description: Представляет объект, который будет использоваться в качестве входных тестовых данных, когда действие Синчронизатионсчема Парсикспрессион выполняет оценку выражения.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0756e14f9a35e1ff1b5a63d563d4bca742be566d
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218445"
---
# <a name="expressioninputobject-resource-type"></a><span data-ttu-id="b7da6-103">Тип ресурса Експрессионинпутобжект</span><span class="sxs-lookup"><span data-stu-id="b7da6-103">expressionInputObject resource type</span></span>

<span data-ttu-id="b7da6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7da6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7da6-105">Представляет объект, который будет использоваться в качестве входных тестовых данных, когда действие [парсикспрессион](../api/synchronization-synchronizationschema-parseexpression.md) выполняет оценку выражения.</span><span class="sxs-lookup"><span data-stu-id="b7da6-105">Represents an object to be used as input test data when the [parseExpression](../api/synchronization-synchronizationschema-parseexpression.md) action performs an expression evaluation.</span></span>

## <a name="properties"></a><span data-ttu-id="b7da6-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b7da6-106">Properties</span></span>
| <span data-ttu-id="b7da6-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b7da6-107">Property</span></span>     | <span data-ttu-id="b7da6-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b7da6-108">Type</span></span>   |<span data-ttu-id="b7da6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b7da6-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b7da6-110">RDLC</span><span class="sxs-lookup"><span data-stu-id="b7da6-110">definition</span></span>|[<span data-ttu-id="b7da6-111">обжектдефинитион</span><span class="sxs-lookup"><span data-stu-id="b7da6-111">objectDefinition</span></span>](synchronization-objectdefinition.md)|<span data-ttu-id="b7da6-112">Определение тестового объекта.</span><span class="sxs-lookup"><span data-stu-id="b7da6-112">Definition of the test object.</span></span>|
|<span data-ttu-id="b7da6-113">properties</span><span class="sxs-lookup"><span data-stu-id="b7da6-113">properties</span></span>|<span data-ttu-id="b7da6-114">Коллекция [стрингкэйобжектвалуепаир](synchronization-stringkeyobjectvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="b7da6-114">[stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md) collection</span></span>|<span data-ttu-id="b7da6-115">Значения свойств тестового объекта.</span><span class="sxs-lookup"><span data-stu-id="b7da6-115">Property values of the test object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b7da6-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b7da6-116">JSON representation</span></span>

<span data-ttu-id="b7da6-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b7da6-117">The following is a JSON representation of the resource.</span></span>

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
