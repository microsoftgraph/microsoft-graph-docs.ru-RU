---
title: Тип ресурса Експрессионинпутобжект
description: 'Представляет объект, который будет использоваться в качестве входных тестовых данных, когда действие [синчронизатионсчема: парсикспрессион](../api/synchronization_synchronizationschema_parseexpression.md) выполняет оценку выражения.'
localization_priority: Normal
ms.openlocfilehash: 3e631102505408b955404c4badb33b98f314236f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582111"
---
# <a name="expressioninputobject-resource-type"></a><span data-ttu-id="8f852-103">Тип ресурса Експрессионинпутобжект</span><span class="sxs-lookup"><span data-stu-id="8f852-103">expressionInputObject resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f852-104">Представляет объект, который будет использоваться в качестве входных тестовых данных, когда действие [синчронизатионсчема: парсикспрессион](../api/synchronization_synchronizationschema_parseexpression.md) выполняет оценку выражения.</span><span class="sxs-lookup"><span data-stu-id="8f852-104">Represents an object to be used as input test data when the [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md) action performs an expression evaluation.</span></span>

## <a name="properties"></a><span data-ttu-id="8f852-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="8f852-105">Properties</span></span>
| <span data-ttu-id="8f852-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="8f852-106">Property</span></span>     | <span data-ttu-id="8f852-107">Тип</span><span class="sxs-lookup"><span data-stu-id="8f852-107">Type</span></span>   |<span data-ttu-id="8f852-108">Описание</span><span class="sxs-lookup"><span data-stu-id="8f852-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8f852-109">RDLC</span><span class="sxs-lookup"><span data-stu-id="8f852-109">definition</span></span>|[<span data-ttu-id="8f852-110">Обжектдефинитион</span><span class="sxs-lookup"><span data-stu-id="8f852-110">objectDefinition</span></span>](synchronization-objectdefinition.md)|<span data-ttu-id="8f852-111">Определение тестового объекта.</span><span class="sxs-lookup"><span data-stu-id="8f852-111">Definition of the test object.</span></span>|
|<span data-ttu-id="8f852-112">properties</span><span class="sxs-lookup"><span data-stu-id="8f852-112">properties</span></span>|<span data-ttu-id="8f852-113">Коллекция [стрингкэйобжектвалуепаир](synchronization-stringkeyobjectvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="8f852-113">[stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md) collection</span></span>|<span data-ttu-id="8f852-114">Значения свойств тестового объекта.</span><span class="sxs-lookup"><span data-stu-id="8f852-114">Property values of the test object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8f852-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8f852-115">JSON representation</span></span>

<span data-ttu-id="8f852-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8f852-116">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-expressioninputobject.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
