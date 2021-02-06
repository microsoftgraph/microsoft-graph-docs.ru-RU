---
title: Тип ресурса genericError
description: Ошибка общего назначения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: abheek-das
ms.openlocfilehash: 611671cc6e35fa9376bff2761719c58f0255f19d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129453"
---
# <a name="genericerror-resource-type"></a><span data-ttu-id="c23c5-103">Тип ресурса genericError</span><span class="sxs-lookup"><span data-stu-id="c23c5-103">genericError resource type</span></span>

<span data-ttu-id="c23c5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c23c5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c23c5-105">Ошибка общего назначения.</span><span class="sxs-lookup"><span data-stu-id="c23c5-105">A general-purpose error.</span></span>

## <a name="properties"></a><span data-ttu-id="c23c5-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c23c5-106">Properties</span></span>

| <span data-ttu-id="c23c5-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c23c5-107">Property</span></span> | <span data-ttu-id="c23c5-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c23c5-108">Type</span></span> | <span data-ttu-id="c23c5-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c23c5-109">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="c23c5-110">message</span><span class="sxs-lookup"><span data-stu-id="c23c5-110">message</span></span> | <span data-ttu-id="c23c5-111">String</span><span class="sxs-lookup"><span data-stu-id="c23c5-111">String</span></span> | <span data-ttu-id="c23c5-112">Сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="c23c5-112">The error message.</span></span> |
| <span data-ttu-id="c23c5-113">code</span><span class="sxs-lookup"><span data-stu-id="c23c5-113">code</span></span> | <span data-ttu-id="c23c5-114">Строка</span><span class="sxs-lookup"><span data-stu-id="c23c5-114">String</span></span> | <span data-ttu-id="c23c5-115">Код ошибки.</span><span class="sxs-lookup"><span data-stu-id="c23c5-115">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c23c5-116">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c23c5-116">JSON representation</span></span>

<span data-ttu-id="c23c5-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c23c5-117">Here is a JSON representation of the resource.</span></span>

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


