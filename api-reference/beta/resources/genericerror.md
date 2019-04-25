---
title: Тип ресурса Женерицеррор
description: Общая ошибка общего назначения.
localization_priority: Normal
ms.openlocfilehash: d3c7e9cd7ff7be635adfbf329170068cd944f0b2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547502"
---
# <a name="genericerror-resource-type"></a><span data-ttu-id="05542-103">Тип ресурса Женерицеррор</span><span class="sxs-lookup"><span data-stu-id="05542-103">genericError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05542-104">Общая ошибка общего назначения.</span><span class="sxs-lookup"><span data-stu-id="05542-104">A general-purpose error.</span></span>

## <a name="properties"></a><span data-ttu-id="05542-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="05542-105">Properties</span></span>

| <span data-ttu-id="05542-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="05542-106">Property</span></span> | <span data-ttu-id="05542-107">Тип</span><span class="sxs-lookup"><span data-stu-id="05542-107">Type</span></span> | <span data-ttu-id="05542-108">Описание</span><span class="sxs-lookup"><span data-stu-id="05542-108">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="05542-109">message</span><span class="sxs-lookup"><span data-stu-id="05542-109">message</span></span> | <span data-ttu-id="05542-110">String</span><span class="sxs-lookup"><span data-stu-id="05542-110">String</span></span> | <span data-ttu-id="05542-111">Сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="05542-111">The error message.</span></span> |
| <span data-ttu-id="05542-112">code</span><span class="sxs-lookup"><span data-stu-id="05542-112">code</span></span> | <span data-ttu-id="05542-113">String</span><span class="sxs-lookup"><span data-stu-id="05542-113">String</span></span> | <span data-ttu-id="05542-114">Код ошибки.</span><span class="sxs-lookup"><span data-stu-id="05542-114">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="05542-115">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="05542-115">JSON representation</span></span>

<span data-ttu-id="05542-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="05542-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.genericError"
}-->

```json
{
  "message": "String",
  "code": "String"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/genericerror.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
