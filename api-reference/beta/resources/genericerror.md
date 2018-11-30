---
title: Тип ресурса Общая ошибка
description: Это ошибка.
ms.openlocfilehash: caf3fbb99ad521fd807138ab230f6a1b8ae7bb16
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075500"
---
# <a name="genericerror-resource-type"></a><span data-ttu-id="ef390-103">Тип ресурса Общая ошибка</span><span class="sxs-lookup"><span data-stu-id="ef390-103">genericError resource type</span></span>

> <span data-ttu-id="ef390-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ef390-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ef390-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef390-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ef390-106">Это ошибка.</span><span class="sxs-lookup"><span data-stu-id="ef390-106">A general-purpose error.</span></span>

## <a name="properties"></a><span data-ttu-id="ef390-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ef390-107">Properties</span></span>

| <span data-ttu-id="ef390-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ef390-108">Property</span></span> | <span data-ttu-id="ef390-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ef390-109">Type</span></span> | <span data-ttu-id="ef390-110">Description</span><span class="sxs-lookup"><span data-stu-id="ef390-110">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="ef390-111">message</span><span class="sxs-lookup"><span data-stu-id="ef390-111">message</span></span> | <span data-ttu-id="ef390-112">String</span><span class="sxs-lookup"><span data-stu-id="ef390-112">String</span></span> | <span data-ttu-id="ef390-113">Сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="ef390-113">The error message.</span></span> |
| <span data-ttu-id="ef390-114">code</span><span class="sxs-lookup"><span data-stu-id="ef390-114">code</span></span> | <span data-ttu-id="ef390-115">String</span><span class="sxs-lookup"><span data-stu-id="ef390-115">String</span></span> | <span data-ttu-id="ef390-116">Код ошибки.</span><span class="sxs-lookup"><span data-stu-id="ef390-116">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ef390-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ef390-117">JSON representation</span></span>

<span data-ttu-id="ef390-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ef390-118">Here is a JSON representation of the resource.</span></span>

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