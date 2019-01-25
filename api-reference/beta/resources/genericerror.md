---
title: Тип ресурса Общая ошибка
description: Это ошибка.
localization_priority: Normal
ms.openlocfilehash: d3c7e9cd7ff7be635adfbf329170068cd944f0b2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524130"
---
# <a name="genericerror-resource-type"></a><span data-ttu-id="df4da-103">Тип ресурса Общая ошибка</span><span class="sxs-lookup"><span data-stu-id="df4da-103">genericError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df4da-104">Это ошибка.</span><span class="sxs-lookup"><span data-stu-id="df4da-104">A general-purpose error.</span></span>

## <a name="properties"></a><span data-ttu-id="df4da-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="df4da-105">Properties</span></span>

| <span data-ttu-id="df4da-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="df4da-106">Property</span></span> | <span data-ttu-id="df4da-107">Тип</span><span class="sxs-lookup"><span data-stu-id="df4da-107">Type</span></span> | <span data-ttu-id="df4da-108">Описание</span><span class="sxs-lookup"><span data-stu-id="df4da-108">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="df4da-109">message</span><span class="sxs-lookup"><span data-stu-id="df4da-109">message</span></span> | <span data-ttu-id="df4da-110">String</span><span class="sxs-lookup"><span data-stu-id="df4da-110">String</span></span> | <span data-ttu-id="df4da-111">Сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="df4da-111">The error message.</span></span> |
| <span data-ttu-id="df4da-112">code</span><span class="sxs-lookup"><span data-stu-id="df4da-112">code</span></span> | <span data-ttu-id="df4da-113">String</span><span class="sxs-lookup"><span data-stu-id="df4da-113">String</span></span> | <span data-ttu-id="df4da-114">Код ошибки.</span><span class="sxs-lookup"><span data-stu-id="df4da-114">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="df4da-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="df4da-115">JSON representation</span></span>

<span data-ttu-id="df4da-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="df4da-116">Here is a JSON representation of the resource.</span></span>

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
