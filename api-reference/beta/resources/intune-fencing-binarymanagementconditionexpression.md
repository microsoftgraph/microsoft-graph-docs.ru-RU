---
title: Тип ресурса binaryManagementConditionExpression
description: Выражение условия управления, который вычисляется с помощью операции двоичного файла.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 722387492e6167c3bd74d306fa03e4835bc12dbe
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402729"
---
# <a name="binarymanagementconditionexpression-resource-type"></a><span data-ttu-id="46db3-103">Тип ресурса binaryManagementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="46db3-103">binaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="46db3-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="46db3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="46db3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46db3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="46db3-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="46db3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46db3-107">Выражение условия управления, который вычисляется с помощью операции двоичного файла.</span><span class="sxs-lookup"><span data-stu-id="46db3-107">A management condition expression that is evaluated using a binary operation.</span></span>


<span data-ttu-id="46db3-108">Наследуется от [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="46db3-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="46db3-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="46db3-109">Properties</span></span>
|<span data-ttu-id="46db3-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="46db3-110">Property</span></span>|<span data-ttu-id="46db3-111">Тип</span><span class="sxs-lookup"><span data-stu-id="46db3-111">Type</span></span>|<span data-ttu-id="46db3-112">Описание</span><span class="sxs-lookup"><span data-stu-id="46db3-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46db3-113">operator</span><span class="sxs-lookup"><span data-stu-id="46db3-113">operator</span></span>|[<span data-ttu-id="46db3-114">binaryManagementConditionExpressionOperatorType</span><span class="sxs-lookup"><span data-stu-id="46db3-114">binaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-binarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="46db3-115">Оператор, используемый в оценке двоичной операции.</span><span class="sxs-lookup"><span data-stu-id="46db3-115">The operator used in the evaluation of the binary operation.</span></span> <span data-ttu-id="46db3-116">Возможные значения: `or`, `and`.</span><span class="sxs-lookup"><span data-stu-id="46db3-116">Possible values are: `or`, `and`.</span></span>|
|<span data-ttu-id="46db3-117">firstOperand</span><span class="sxs-lookup"><span data-stu-id="46db3-117">firstOperand</span></span>|[<span data-ttu-id="46db3-118">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="46db3-118">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="46db3-119">Первый операнд двоичной операции.</span><span class="sxs-lookup"><span data-stu-id="46db3-119">The first operand of the binary operation.</span></span>|
|<span data-ttu-id="46db3-120">secondOperand</span><span class="sxs-lookup"><span data-stu-id="46db3-120">secondOperand</span></span>|[<span data-ttu-id="46db3-121">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="46db3-121">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="46db3-122">Второй операнд двоичной операции.</span><span class="sxs-lookup"><span data-stu-id="46db3-122">The second operand of the binary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="46db3-123">Отношения</span><span class="sxs-lookup"><span data-stu-id="46db3-123">Relationships</span></span>
<span data-ttu-id="46db3-124">Нет</span><span class="sxs-lookup"><span data-stu-id="46db3-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="46db3-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="46db3-125">JSON Representation</span></span>
<span data-ttu-id="46db3-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="46db3-126">Here is a JSON representation of the resource.</span></span>
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




