---
title: Тип ресурса Женерицеррор
description: Общая ошибка общего назначения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 4c68fa52046ccb48645aab1fbf2de4a772665328
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42497645"
---
# <a name="genericerror-resource-type"></a><span data-ttu-id="fdd02-103">Тип ресурса Женерицеррор</span><span class="sxs-lookup"><span data-stu-id="fdd02-103">genericError resource type</span></span>

<span data-ttu-id="fdd02-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="fdd02-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fdd02-105">Общая ошибка общего назначения.</span><span class="sxs-lookup"><span data-stu-id="fdd02-105">A general-purpose error.</span></span>

## <a name="properties"></a><span data-ttu-id="fdd02-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="fdd02-106">Properties</span></span>

| <span data-ttu-id="fdd02-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="fdd02-107">Property</span></span> | <span data-ttu-id="fdd02-108">Тип</span><span class="sxs-lookup"><span data-stu-id="fdd02-108">Type</span></span> | <span data-ttu-id="fdd02-109">Описание</span><span class="sxs-lookup"><span data-stu-id="fdd02-109">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="fdd02-110">message</span><span class="sxs-lookup"><span data-stu-id="fdd02-110">message</span></span> | <span data-ttu-id="fdd02-111">String</span><span class="sxs-lookup"><span data-stu-id="fdd02-111">String</span></span> | <span data-ttu-id="fdd02-112">Сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="fdd02-112">The error message.</span></span> |
| <span data-ttu-id="fdd02-113">code</span><span class="sxs-lookup"><span data-stu-id="fdd02-113">code</span></span> | <span data-ttu-id="fdd02-114">String</span><span class="sxs-lookup"><span data-stu-id="fdd02-114">String</span></span> | <span data-ttu-id="fdd02-115">Код ошибки.</span><span class="sxs-lookup"><span data-stu-id="fdd02-115">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fdd02-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fdd02-116">JSON representation</span></span>

<span data-ttu-id="fdd02-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fdd02-117">Here is a JSON representation of the resource.</span></span>

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
