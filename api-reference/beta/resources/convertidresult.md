---
title: Тип ресурса convertIdResult
description: Результат преобразования формата код выполняется с помощью функции translateExchangeIds.
localization_priority: Normal
ms.openlocfilehash: db28172d009ee8a8a39b7e02733d893dc20a81e5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516527"
---
# <a name="convertidresult-resource-type"></a><span data-ttu-id="a111d-103">Тип ресурса convertIdResult</span><span class="sxs-lookup"><span data-stu-id="a111d-103">convertIdResult resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a111d-104">Результат преобразования формата код выполняется с помощью функции [translateExchangeIds](../api/user-translateexchangeids.md) .</span><span class="sxs-lookup"><span data-stu-id="a111d-104">The result of an ID format conversion performed by the [translateExchangeIds](../api/user-translateexchangeids.md) function.</span></span>

## <a name="properties"></a><span data-ttu-id="a111d-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="a111d-105">Properties</span></span>

| <span data-ttu-id="a111d-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="a111d-106">Property</span></span> | <span data-ttu-id="a111d-107">Тип</span><span class="sxs-lookup"><span data-stu-id="a111d-107">Type</span></span> | <span data-ttu-id="a111d-108">Описание</span><span class="sxs-lookup"><span data-stu-id="a111d-108">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="a111d-109">SourceId</span><span class="sxs-lookup"><span data-stu-id="a111d-109">sourceId</span></span> | <span data-ttu-id="a111d-110">String</span><span class="sxs-lookup"><span data-stu-id="a111d-110">String</span></span> | <span data-ttu-id="a111d-111">Идентификатор, который был преобразован.</span><span class="sxs-lookup"><span data-stu-id="a111d-111">The identifier that was converted.</span></span> <span data-ttu-id="a111d-112">Это значение является идентификатором исходного, без преобразованные.</span><span class="sxs-lookup"><span data-stu-id="a111d-112">This value is the original, un-converted identifier.</span></span> |
| <span data-ttu-id="a111d-113">targetId</span><span class="sxs-lookup"><span data-stu-id="a111d-113">targetId</span></span> | <span data-ttu-id="a111d-114">String</span><span class="sxs-lookup"><span data-stu-id="a111d-114">String</span></span> | <span data-ttu-id="a111d-115">Преобразованные идентификатор.</span><span class="sxs-lookup"><span data-stu-id="a111d-115">The converted identifier.</span></span> <span data-ttu-id="a111d-116">Это значение не задано, если не удалось выполнить преобразование.</span><span class="sxs-lookup"><span data-stu-id="a111d-116">This value is not present if the conversion failed.</span></span> |
| <span data-ttu-id="a111d-117">errorDetails</span><span class="sxs-lookup"><span data-stu-id="a111d-117">errorDetails</span></span> | [<span data-ttu-id="a111d-118">Общая ошибка</span><span class="sxs-lookup"><span data-stu-id="a111d-118">genericError</span></span>](genericerror.md) | <span data-ttu-id="a111d-119">Объект error, которое указывает причину сбоя преобразования.</span><span class="sxs-lookup"><span data-stu-id="a111d-119">An error object indicating the reason for the conversion failure.</span></span> <span data-ttu-id="a111d-120">Это значение не задано, если преобразование выполнено успешно.</span><span class="sxs-lookup"><span data-stu-id="a111d-120">This value is not present if the conversion succeeded.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a111d-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a111d-121">JSON representation</span></span>

<span data-ttu-id="a111d-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a111d-122">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "targetId",
    "errorDetails"
  ],
  "@odata.type": "microsoft.graph.convertIdResult"
}-->

```json
{
  "sourceId": "String",
  "targetId": "String",
  "errorDetails": {
    "@odata.type": "microsoft.graph.genericError"
  }
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/convertidresult.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
