---
title: Тип ресурса Общая ошибка
description: Это ошибка.
localization_priority: Normal
ms.openlocfilehash: 744266ef8ffb17c4af4168d6239e5a5a30561936
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823571"
---
# <a name="genericerror-resource-type"></a><span data-ttu-id="5f0d9-103">Тип ресурса Общая ошибка</span><span class="sxs-lookup"><span data-stu-id="5f0d9-103">genericError resource type</span></span>

> <span data-ttu-id="5f0d9-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5f0d9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5f0d9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f0d9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5f0d9-106">Это ошибка.</span><span class="sxs-lookup"><span data-stu-id="5f0d9-106">A general-purpose error.</span></span>

## <a name="properties"></a><span data-ttu-id="5f0d9-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5f0d9-107">Properties</span></span>

| <span data-ttu-id="5f0d9-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5f0d9-108">Property</span></span> | <span data-ttu-id="5f0d9-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5f0d9-109">Type</span></span> | <span data-ttu-id="5f0d9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5f0d9-110">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="5f0d9-111">message</span><span class="sxs-lookup"><span data-stu-id="5f0d9-111">message</span></span> | <span data-ttu-id="5f0d9-112">String</span><span class="sxs-lookup"><span data-stu-id="5f0d9-112">String</span></span> | <span data-ttu-id="5f0d9-113">Сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="5f0d9-113">The error message.</span></span> |
| <span data-ttu-id="5f0d9-114">code</span><span class="sxs-lookup"><span data-stu-id="5f0d9-114">code</span></span> | <span data-ttu-id="5f0d9-115">Строка</span><span class="sxs-lookup"><span data-stu-id="5f0d9-115">String</span></span> | <span data-ttu-id="5f0d9-116">Код ошибки.</span><span class="sxs-lookup"><span data-stu-id="5f0d9-116">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5f0d9-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5f0d9-117">JSON representation</span></span>

<span data-ttu-id="5f0d9-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5f0d9-118">Here is a JSON representation of the resource.</span></span>

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
