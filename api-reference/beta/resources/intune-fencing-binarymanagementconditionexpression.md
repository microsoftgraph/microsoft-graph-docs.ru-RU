---
title: Тип ресурса binaryManagementConditionExpression
description: Выражение условия управления, который вычисляется с помощью операции двоичного файла.
author: tfitzmac
ms.openlocfilehash: 6f271be2527427daaa04436899552abb4d21475e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27357521"
---
# <a name="binarymanagementconditionexpression-resource-type"></a><span data-ttu-id="698d0-103">Тип ресурса binaryManagementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="698d0-103">binaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="698d0-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="698d0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="698d0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="698d0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="698d0-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="698d0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="698d0-107">Выражение условия управления, который вычисляется с помощью операции двоичного файла.</span><span class="sxs-lookup"><span data-stu-id="698d0-107">A management condition expression that is evaluated using a binary operation.</span></span>

<span data-ttu-id="698d0-108">Наследуется от [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="698d0-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="698d0-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="698d0-109">Properties</span></span>
|<span data-ttu-id="698d0-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="698d0-110">Property</span></span>|<span data-ttu-id="698d0-111">Тип</span><span class="sxs-lookup"><span data-stu-id="698d0-111">Type</span></span>|<span data-ttu-id="698d0-112">Описание</span><span class="sxs-lookup"><span data-stu-id="698d0-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="698d0-113">operator</span><span class="sxs-lookup"><span data-stu-id="698d0-113">operator</span></span>|[<span data-ttu-id="698d0-114">binaryManagementConditionExpressionOperatorType</span><span class="sxs-lookup"><span data-stu-id="698d0-114">binaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-binarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="698d0-115">Оператор, используемый в оценке двоичной операции.</span><span class="sxs-lookup"><span data-stu-id="698d0-115">The operator used in the evaluation of the binary operation.</span></span> <span data-ttu-id="698d0-116">Возможные значения: `or`, `and`.</span><span class="sxs-lookup"><span data-stu-id="698d0-116">Possible values are: `or`, `and`.</span></span>|
|<span data-ttu-id="698d0-117">firstOperand</span><span class="sxs-lookup"><span data-stu-id="698d0-117">firstOperand</span></span>|[<span data-ttu-id="698d0-118">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="698d0-118">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="698d0-119">Первый операнд двоичной операции.</span><span class="sxs-lookup"><span data-stu-id="698d0-119">The first operand of the binary operation.</span></span>|
|<span data-ttu-id="698d0-120">secondOperand</span><span class="sxs-lookup"><span data-stu-id="698d0-120">secondOperand</span></span>|[<span data-ttu-id="698d0-121">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="698d0-121">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="698d0-122">Второй операнд двоичной операции.</span><span class="sxs-lookup"><span data-stu-id="698d0-122">The second operand of the binary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="698d0-123">Связи</span><span class="sxs-lookup"><span data-stu-id="698d0-123">Relationships</span></span>
<span data-ttu-id="698d0-124">Нет</span><span class="sxs-lookup"><span data-stu-id="698d0-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="698d0-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="698d0-125">JSON Representation</span></span>
<span data-ttu-id="698d0-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="698d0-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.binaryManagementConditionExpression"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.binaryManagementConditionExpression",
  "operator": "String",
  "firstOperand": {
    "@odata.type": "microsoft.graph.managementConditionExpressionModel"
  },
  "secondOperand": {
    "@odata.type": "microsoft.graph.managementConditionExpressionModel"
  }
}
```





