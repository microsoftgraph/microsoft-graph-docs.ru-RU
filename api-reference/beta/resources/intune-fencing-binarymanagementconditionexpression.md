---
title: Тип ресурса binaryManagementConditionExpression
description: Выражение условия управления, который вычисляется с помощью операции двоичного файла.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b15938d0bb29fdfdad8abb1b37b02ad1e6468cf9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978538"
---
# <a name="binarymanagementconditionexpression-resource-type"></a><span data-ttu-id="e0bf1-103">Тип ресурса binaryManagementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="e0bf1-103">binaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="e0bf1-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e0bf1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e0bf1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0bf1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e0bf1-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e0bf1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e0bf1-107">Выражение условия управления, который вычисляется с помощью операции двоичного файла.</span><span class="sxs-lookup"><span data-stu-id="e0bf1-107">A management condition expression that is evaluated using a binary operation.</span></span>

<span data-ttu-id="e0bf1-108">Наследуется от [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="e0bf1-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e0bf1-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="e0bf1-109">Properties</span></span>
|<span data-ttu-id="e0bf1-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="e0bf1-110">Property</span></span>|<span data-ttu-id="e0bf1-111">Тип</span><span class="sxs-lookup"><span data-stu-id="e0bf1-111">Type</span></span>|<span data-ttu-id="e0bf1-112">Описание</span><span class="sxs-lookup"><span data-stu-id="e0bf1-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0bf1-113">operator</span><span class="sxs-lookup"><span data-stu-id="e0bf1-113">operator</span></span>|[<span data-ttu-id="e0bf1-114">binaryManagementConditionExpressionOperatorType</span><span class="sxs-lookup"><span data-stu-id="e0bf1-114">binaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-binarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="e0bf1-115">Оператор, используемый в оценке двоичной операции.</span><span class="sxs-lookup"><span data-stu-id="e0bf1-115">The operator used in the evaluation of the binary operation.</span></span> <span data-ttu-id="e0bf1-116">Возможные значения: `or`, `and`.</span><span class="sxs-lookup"><span data-stu-id="e0bf1-116">Possible values are: `or`, `and`.</span></span>|
|<span data-ttu-id="e0bf1-117">firstOperand</span><span class="sxs-lookup"><span data-stu-id="e0bf1-117">firstOperand</span></span>|[<span data-ttu-id="e0bf1-118">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="e0bf1-118">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="e0bf1-119">Первый операнд двоичной операции.</span><span class="sxs-lookup"><span data-stu-id="e0bf1-119">The first operand of the binary operation.</span></span>|
|<span data-ttu-id="e0bf1-120">secondOperand</span><span class="sxs-lookup"><span data-stu-id="e0bf1-120">secondOperand</span></span>|[<span data-ttu-id="e0bf1-121">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="e0bf1-121">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="e0bf1-122">Второй операнд двоичной операции.</span><span class="sxs-lookup"><span data-stu-id="e0bf1-122">The second operand of the binary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e0bf1-123">Связи</span><span class="sxs-lookup"><span data-stu-id="e0bf1-123">Relationships</span></span>
<span data-ttu-id="e0bf1-124">Нет</span><span class="sxs-lookup"><span data-stu-id="e0bf1-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e0bf1-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e0bf1-125">JSON Representation</span></span>
<span data-ttu-id="e0bf1-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e0bf1-126">Here is a JSON representation of the resource.</span></span>
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





