---
title: Тип ресурса resultInfo
description: Тип resultInfo.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 0c924798715448e87c30cf2b65cc923c6ddc20bc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521084"
---
# <a name="resultinfo-resource-type"></a><span data-ttu-id="8d42f-103">Тип ресурса resultInfo</span><span class="sxs-lookup"><span data-stu-id="8d42f-103">resultInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d42f-104">Тип resultInfo.</span><span class="sxs-lookup"><span data-stu-id="8d42f-104">The resultInfo type.</span></span>

## <a name="properties"></a><span data-ttu-id="8d42f-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="8d42f-105">Properties</span></span>

| <span data-ttu-id="8d42f-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="8d42f-106">Property</span></span> | <span data-ttu-id="8d42f-107">Тип</span><span class="sxs-lookup"><span data-stu-id="8d42f-107">Type</span></span>   | <span data-ttu-id="8d42f-108">Описание</span><span class="sxs-lookup"><span data-stu-id="8d42f-108">Description</span></span>          |
| :------- | :----- | :------------------  |
| <span data-ttu-id="8d42f-109">code</span><span class="sxs-lookup"><span data-stu-id="8d42f-109">code</span></span>     | <span data-ttu-id="8d42f-110">String</span><span class="sxs-lookup"><span data-stu-id="8d42f-110">String</span></span> | <span data-ttu-id="8d42f-111">Код результата.</span><span class="sxs-lookup"><span data-stu-id="8d42f-111">The result code.</span></span>     |
| <span data-ttu-id="8d42f-112">message</span><span class="sxs-lookup"><span data-stu-id="8d42f-112">message</span></span>  | <span data-ttu-id="8d42f-113">String</span><span class="sxs-lookup"><span data-stu-id="8d42f-113">String</span></span> | <span data-ttu-id="8d42f-114">Сообщение.</span><span class="sxs-lookup"><span data-stu-id="8d42f-114">The message.</span></span>         |
| <span data-ttu-id="8d42f-115">дополнительный код</span><span class="sxs-lookup"><span data-stu-id="8d42f-115">subCode</span></span>  | <span data-ttu-id="8d42f-116">String</span><span class="sxs-lookup"><span data-stu-id="8d42f-116">String</span></span> | <span data-ttu-id="8d42f-117">Вложенный код результата.</span><span class="sxs-lookup"><span data-stu-id="8d42f-117">The result sub-code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8d42f-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8d42f-118">JSON representation</span></span>

<span data-ttu-id="8d42f-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8d42f-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resultInfo"
}-->
```json
{
  "code": "String",
  "message": "String",
  "subCode": "String"
}
```

## <a name="example-error-result"></a><span data-ttu-id="8d42f-120">Пример результат ошибки</span><span class="sxs-lookup"><span data-stu-id="8d42f-120">Example Error result</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.resultInfo"
}-->
```json
{
  "code": "100",
  "message": "Internal Server Error.",
  "subCode": "20"
}
```

## <a name="example-generic-success-result"></a><span data-ttu-id="8d42f-121">Пример универсального успеха результатов</span><span class="sxs-lookup"><span data-stu-id="8d42f-121">Example Generic success result</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.resultInfo"
}-->
```json
{
  "code": "200",
  "message": "",
  "subCode": "0"
}
```

## <a name="example-record-success-result"></a><span data-ttu-id="8d42f-122">Пример записи успеха результатов</span><span class="sxs-lookup"><span data-stu-id="8d42f-122">Example Record Success result</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.resultInfo"
}-->
```json
{
  "code": "200",
  "message": "",
  "subCode": "completedSilenceDetected"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "resultInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/resultinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
