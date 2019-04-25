---
title: Тип ресурса Конвертидресулт
description: Результат преобразования формата идентификатора, выполняемого функцией Транслатиксчанжеидс.
localization_priority: Normal
ms.openlocfilehash: db28172d009ee8a8a39b7e02733d893dc20a81e5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535393"
---
# <a name="convertidresult-resource-type"></a><span data-ttu-id="3ebae-103">Тип ресурса Конвертидресулт</span><span class="sxs-lookup"><span data-stu-id="3ebae-103">convertIdResult resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ebae-104">Результат преобразования формата идентификатора, выполняемого функцией [транслатиксчанжеидс](../api/user-translateexchangeids.md) .</span><span class="sxs-lookup"><span data-stu-id="3ebae-104">The result of an ID format conversion performed by the [translateExchangeIds](../api/user-translateexchangeids.md) function.</span></span>

## <a name="properties"></a><span data-ttu-id="3ebae-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="3ebae-105">Properties</span></span>

| <span data-ttu-id="3ebae-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="3ebae-106">Property</span></span> | <span data-ttu-id="3ebae-107">Тип</span><span class="sxs-lookup"><span data-stu-id="3ebae-107">Type</span></span> | <span data-ttu-id="3ebae-108">Описание</span><span class="sxs-lookup"><span data-stu-id="3ebae-108">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="3ebae-109">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="3ebae-109">sourceId</span></span> | <span data-ttu-id="3ebae-110">String</span><span class="sxs-lookup"><span data-stu-id="3ebae-110">String</span></span> | <span data-ttu-id="3ebae-111">Преобразованный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="3ebae-111">The identifier that was converted.</span></span> <span data-ttu-id="3ebae-112">Это значение является исходным непреобразуемым идентификатором.</span><span class="sxs-lookup"><span data-stu-id="3ebae-112">This value is the original, un-converted identifier.</span></span> |
| <span data-ttu-id="3ebae-113">targetId</span><span class="sxs-lookup"><span data-stu-id="3ebae-113">targetId</span></span> | <span data-ttu-id="3ebae-114">String</span><span class="sxs-lookup"><span data-stu-id="3ebae-114">String</span></span> | <span data-ttu-id="3ebae-115">Преобразованный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="3ebae-115">The converted identifier.</span></span> <span data-ttu-id="3ebae-116">Это значение отсутствует, если произошел сбой преобразования.</span><span class="sxs-lookup"><span data-stu-id="3ebae-116">This value is not present if the conversion failed.</span></span> |
| <span data-ttu-id="3ebae-117">Еррордетаилс</span><span class="sxs-lookup"><span data-stu-id="3ebae-117">errorDetails</span></span> | [<span data-ttu-id="3ebae-118">Женерицеррор</span><span class="sxs-lookup"><span data-stu-id="3ebae-118">genericError</span></span>](genericerror.md) | <span data-ttu-id="3ebae-119">Объект Error, указывающий причину сбоя преобразования.</span><span class="sxs-lookup"><span data-stu-id="3ebae-119">An error object indicating the reason for the conversion failure.</span></span> <span data-ttu-id="3ebae-120">Это значение отсутствует, если преобразование выполнено успешно.</span><span class="sxs-lookup"><span data-stu-id="3ebae-120">This value is not present if the conversion succeeded.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3ebae-121">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3ebae-121">JSON representation</span></span>

<span data-ttu-id="3ebae-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3ebae-122">Here is a JSON representation of the resource.</span></span>

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
