---
title: Тип ресурса Женерицеррор
description: Общая ошибка общего назначения.
localization_priority: Normal
ms.openlocfilehash: 314bb5f5e94e44c326fceb71f4a79463989f2129
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333673"
---
# <a name="genericerror-resource-type"></a><span data-ttu-id="02c77-103">Тип ресурса Женерицеррор</span><span class="sxs-lookup"><span data-stu-id="02c77-103">genericError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02c77-104">Общая ошибка общего назначения.</span><span class="sxs-lookup"><span data-stu-id="02c77-104">A general-purpose error.</span></span>

## <a name="properties"></a><span data-ttu-id="02c77-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="02c77-105">Properties</span></span>

| <span data-ttu-id="02c77-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="02c77-106">Property</span></span> | <span data-ttu-id="02c77-107">Тип</span><span class="sxs-lookup"><span data-stu-id="02c77-107">Type</span></span> | <span data-ttu-id="02c77-108">Описание</span><span class="sxs-lookup"><span data-stu-id="02c77-108">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="02c77-109">message</span><span class="sxs-lookup"><span data-stu-id="02c77-109">message</span></span> | <span data-ttu-id="02c77-110">String</span><span class="sxs-lookup"><span data-stu-id="02c77-110">String</span></span> | <span data-ttu-id="02c77-111">Сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="02c77-111">The error message.</span></span> |
| <span data-ttu-id="02c77-112">code</span><span class="sxs-lookup"><span data-stu-id="02c77-112">code</span></span> | <span data-ttu-id="02c77-113">String</span><span class="sxs-lookup"><span data-stu-id="02c77-113">String</span></span> | <span data-ttu-id="02c77-114">Код ошибки.</span><span class="sxs-lookup"><span data-stu-id="02c77-114">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="02c77-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="02c77-115">JSON representation</span></span>

<span data-ttu-id="02c77-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="02c77-116">Here is a JSON representation of the resource.</span></span>

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
