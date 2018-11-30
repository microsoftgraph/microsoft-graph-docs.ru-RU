---
title: Тип ресурса unaryManagementConditionExpression
description: Выражение условия управления, который вычисляется с использованием унарного.
ms.openlocfilehash: 958c180e52a268f849eca1fe0d2a2b75ff81333b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078859"
---
# <a name="unarymanagementconditionexpression-resource-type"></a><span data-ttu-id="5a699-103">Тип ресурса unaryManagementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="5a699-103">unaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="5a699-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5a699-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5a699-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a699-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5a699-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5a699-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5a699-107">Выражение условия управления, который вычисляется с использованием унарного.</span><span class="sxs-lookup"><span data-stu-id="5a699-107">A management condition expression that is evaluated using a unary operation.</span></span>

<span data-ttu-id="5a699-108">Наследуется от [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="5a699-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5a699-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="5a699-109">Properties</span></span>
|<span data-ttu-id="5a699-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="5a699-110">Property</span></span>|<span data-ttu-id="5a699-111">Тип</span><span class="sxs-lookup"><span data-stu-id="5a699-111">Type</span></span>|<span data-ttu-id="5a699-112">Description</span><span class="sxs-lookup"><span data-stu-id="5a699-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a699-113">operator</span><span class="sxs-lookup"><span data-stu-id="5a699-113">operator</span></span>|[<span data-ttu-id="5a699-114">unaryManagementConditionExpressionOperatorType</span><span class="sxs-lookup"><span data-stu-id="5a699-114">unaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-unarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="5a699-115">Оператор, используемый в оценке унарного.</span><span class="sxs-lookup"><span data-stu-id="5a699-115">The operator used in the evaluation of the unary operation.</span></span> <span data-ttu-id="5a699-116">Возможные значения: `not`.</span><span class="sxs-lookup"><span data-stu-id="5a699-116">Possible values are: `not`.</span></span>|
|<span data-ttu-id="5a699-117">операнд</span><span class="sxs-lookup"><span data-stu-id="5a699-117">operand</span></span>|[<span data-ttu-id="5a699-118">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="5a699-118">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="5a699-119">Операнд унарного.</span><span class="sxs-lookup"><span data-stu-id="5a699-119">The operand of the unary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5a699-120">Связи</span><span class="sxs-lookup"><span data-stu-id="5a699-120">Relationships</span></span>
<span data-ttu-id="5a699-121">Нет</span><span class="sxs-lookup"><span data-stu-id="5a699-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5a699-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5a699-122">JSON Representation</span></span>
<span data-ttu-id="5a699-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5a699-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.unaryManagementConditionExpression"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unaryManagementConditionExpression",
  "operator": "String",
  "operand": {
    "@odata.type": "microsoft.graph.managementConditionExpressionModel"
  }
}
```





