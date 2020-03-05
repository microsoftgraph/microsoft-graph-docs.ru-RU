---
title: Тип ресурса Експрессионинпутобжект
description: 'Представляет объект, который будет использоваться в качестве входных тестовых данных, когда действие [синчронизатионсчема: парсикспрессион](../api/synchronization_synchronizationschema_parseexpression.md) выполняет оценку выражения.'
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 107dd80187f7b00439ec248be513d921bc64888e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520207"
---
# <a name="expressioninputobject-resource-type"></a><span data-ttu-id="45e3a-103">Тип ресурса Експрессионинпутобжект</span><span class="sxs-lookup"><span data-stu-id="45e3a-103">expressionInputObject resource type</span></span>

<span data-ttu-id="45e3a-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="45e3a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45e3a-105">Представляет объект, который будет использоваться в качестве входных тестовых данных, когда действие [парсикспрессион](../api/synchronization-synchronizationschema-parseexpression.md) выполняет оценку выражения.</span><span class="sxs-lookup"><span data-stu-id="45e3a-105">Represents an object to be used as input test data when the [parseExpression](../api/synchronization-synchronizationschema-parseexpression.md) action performs an expression evaluation.</span></span>

## <a name="properties"></a><span data-ttu-id="45e3a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="45e3a-106">Properties</span></span>
| <span data-ttu-id="45e3a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="45e3a-107">Property</span></span>     | <span data-ttu-id="45e3a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="45e3a-108">Type</span></span>   |<span data-ttu-id="45e3a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="45e3a-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="45e3a-110">RDLC</span><span class="sxs-lookup"><span data-stu-id="45e3a-110">definition</span></span>|[<span data-ttu-id="45e3a-111">обжектдефинитион</span><span class="sxs-lookup"><span data-stu-id="45e3a-111">objectDefinition</span></span>](synchronization-objectdefinition.md)|<span data-ttu-id="45e3a-112">Определение тестового объекта.</span><span class="sxs-lookup"><span data-stu-id="45e3a-112">Definition of the test object.</span></span>|
|<span data-ttu-id="45e3a-113">properties</span><span class="sxs-lookup"><span data-stu-id="45e3a-113">properties</span></span>|<span data-ttu-id="45e3a-114">Коллекция [стрингкэйобжектвалуепаир](synchronization-stringkeyobjectvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="45e3a-114">[stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md) collection</span></span>|<span data-ttu-id="45e3a-115">Значения свойств тестового объекта.</span><span class="sxs-lookup"><span data-stu-id="45e3a-115">Property values of the test object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="45e3a-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="45e3a-116">JSON representation</span></span>

<span data-ttu-id="45e3a-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="45e3a-117">The following is a JSON representation of the resource.</span></span>

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
