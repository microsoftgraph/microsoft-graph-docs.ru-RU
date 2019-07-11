---
title: Тип ресурса Експрессионинпутобжект
description: 'Представляет объект, который будет использоваться в качестве входных тестовых данных, когда действие [синчронизатионсчема: парсикспрессион](../api/synchronization_synchronizationschema_parseexpression.md) выполняет оценку выражения.'
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b5fb11471757328bf0b84ae5ea0977d43587d7e4
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/11/2019
ms.locfileid: "35621384"
---
# <a name="expressioninputobject-resource-type"></a><span data-ttu-id="0de50-103">Тип ресурса Експрессионинпутобжект</span><span class="sxs-lookup"><span data-stu-id="0de50-103">expressionInputObject resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0de50-104">Представляет объект, который будет использоваться в качестве входных тестовых данных, когда действие [парсикспрессион](../api/synchronization-synchronizationschema-parseexpression.md) выполняет оценку выражения.</span><span class="sxs-lookup"><span data-stu-id="0de50-104">Represents an object to be used as input test data when the [parseExpression](../api/synchronization-synchronizationschema-parseexpression.md) action performs an expression evaluation.</span></span>

## <a name="properties"></a><span data-ttu-id="0de50-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="0de50-105">Properties</span></span>
| <span data-ttu-id="0de50-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="0de50-106">Property</span></span>     | <span data-ttu-id="0de50-107">Тип</span><span class="sxs-lookup"><span data-stu-id="0de50-107">Type</span></span>   |<span data-ttu-id="0de50-108">Описание</span><span class="sxs-lookup"><span data-stu-id="0de50-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0de50-109">RDLC</span><span class="sxs-lookup"><span data-stu-id="0de50-109">definition</span></span>|[<span data-ttu-id="0de50-110">Обжектдефинитион</span><span class="sxs-lookup"><span data-stu-id="0de50-110">objectDefinition</span></span>](synchronization-objectdefinition.md)|<span data-ttu-id="0de50-111">Определение тестового объекта.</span><span class="sxs-lookup"><span data-stu-id="0de50-111">Definition of the test object.</span></span>|
|<span data-ttu-id="0de50-112">properties</span><span class="sxs-lookup"><span data-stu-id="0de50-112">properties</span></span>|<span data-ttu-id="0de50-113">Коллекция [стрингкэйобжектвалуепаир](synchronization-stringkeyobjectvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="0de50-113">[stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md) collection</span></span>|<span data-ttu-id="0de50-114">Значения свойств тестового объекта.</span><span class="sxs-lookup"><span data-stu-id="0de50-114">Property values of the test object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0de50-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0de50-115">JSON representation</span></span>

<span data-ttu-id="0de50-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0de50-116">The following is a JSON representation of the resource.</span></span>

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
