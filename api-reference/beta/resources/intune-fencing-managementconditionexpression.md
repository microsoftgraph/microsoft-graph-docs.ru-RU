---
title: Тип ресурса managementConditionExpression
description: Выражение условия управления — это выражение, результатом является значение типа boolean, при вычислении, то есть одно из значение true или false, указывающего на то, что условная инструкция управления активируется или деактивируется. Выражение условия управления может включать в себя сочетание выражения переменных и выражения логические операторы.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: b25469c3efb9f7985bf21ad47e83c34b47f96b64
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941879"
---
# <a name="managementconditionexpression-resource-type"></a><span data-ttu-id="59b49-104">Тип ресурса managementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="59b49-104">managementConditionExpression resource type</span></span>

> <span data-ttu-id="59b49-105">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="59b49-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="59b49-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59b49-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="59b49-107">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="59b49-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="59b49-108">Выражение условия управления — это выражение, результатом является значение типа boolean, при вычислении, то есть одно из значение true или false, указывающего на то, что условная инструкция управления активируется или деактивируется.</span><span class="sxs-lookup"><span data-stu-id="59b49-108">A management condition expression is an expression that produces a boolean value when evaluated, i.e. one of true or false, indicating that a management condition statement is activated/deactivated.</span></span> <span data-ttu-id="59b49-109">Выражение условия управления может включать в себя сочетание выражения переменных и выражения логические операторы.</span><span class="sxs-lookup"><span data-stu-id="59b49-109">A management condition expression may be composed of a combination of the expression variables and boolean-valued expression operators.</span></span>
## <a name="properties"></a><span data-ttu-id="59b49-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="59b49-110">Properties</span></span>
|<span data-ttu-id="59b49-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="59b49-111">Property</span></span>|<span data-ttu-id="59b49-112">Тип</span><span class="sxs-lookup"><span data-stu-id="59b49-112">Type</span></span>|<span data-ttu-id="59b49-113">Описание</span><span class="sxs-lookup"><span data-stu-id="59b49-113">Description</span></span>|
|:---|:---|:---|

## <a name="relationships"></a><span data-ttu-id="59b49-114">Связи</span><span class="sxs-lookup"><span data-stu-id="59b49-114">Relationships</span></span>
<span data-ttu-id="59b49-115">Нет</span><span class="sxs-lookup"><span data-stu-id="59b49-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="59b49-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="59b49-116">JSON Representation</span></span>
<span data-ttu-id="59b49-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="59b49-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managementConditionExpression"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementConditionExpression"
}
```





