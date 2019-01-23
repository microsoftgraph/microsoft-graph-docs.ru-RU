---
title: Тип ресурса managementConditionExpression
description: Выражение условия управления — это выражение, результатом является значение типа boolean, при вычислении, то есть одно из значение true или false, указывающего на то, что условная инструкция управления активируется или деактивируется. Выражение условия управления может включать в себя сочетание выражения переменных и выражения логические операторы.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e572cdae0104cf5bbb929286b4c3452dfd38eeea
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415511"
---
# <a name="managementconditionexpression-resource-type"></a><span data-ttu-id="f660f-104">Тип ресурса managementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="f660f-104">managementConditionExpression resource type</span></span>

> <span data-ttu-id="f660f-105">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f660f-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f660f-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f660f-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f660f-107">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f660f-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f660f-108">Выражение условия управления — это выражение, результатом является значение типа boolean, при вычислении, то есть одно из значение true или false, указывающего на то, что условная инструкция управления активируется или деактивируется.</span><span class="sxs-lookup"><span data-stu-id="f660f-108">A management condition expression is an expression that produces a boolean value when evaluated, i.e. one of true or false, indicating that a management condition statement is activated/deactivated.</span></span> <span data-ttu-id="f660f-109">Выражение условия управления может включать в себя сочетание выражения переменных и выражения логические операторы.</span><span class="sxs-lookup"><span data-stu-id="f660f-109">A management condition expression may be composed of a combination of the expression variables and boolean-valued expression operators.</span></span>

## <a name="properties"></a><span data-ttu-id="f660f-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="f660f-110">Properties</span></span>
|<span data-ttu-id="f660f-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="f660f-111">Property</span></span>|<span data-ttu-id="f660f-112">Тип</span><span class="sxs-lookup"><span data-stu-id="f660f-112">Type</span></span>|<span data-ttu-id="f660f-113">Описание</span><span class="sxs-lookup"><span data-stu-id="f660f-113">Description</span></span>|
|:---|:---|:---|

## <a name="relationships"></a><span data-ttu-id="f660f-114">Связи</span><span class="sxs-lookup"><span data-stu-id="f660f-114">Relationships</span></span>
<span data-ttu-id="f660f-115">Нет</span><span class="sxs-lookup"><span data-stu-id="f660f-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f660f-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f660f-116">JSON Representation</span></span>
<span data-ttu-id="f660f-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f660f-117">Here is a JSON representation of the resource.</span></span>
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




