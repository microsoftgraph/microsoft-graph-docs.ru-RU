---
title: Тип ресурса Бинариманажементкондитионекспрессион
description: Выражение условия управления, вычисляемое с помощью бинарной операции.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ff87c376bd88e49d8dc2c3d4657607e7bddcb503
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783279"
---
# <a name="binarymanagementconditionexpression-resource-type"></a><span data-ttu-id="1a740-103">Тип ресурса Бинариманажементкондитионекспрессион</span><span class="sxs-lookup"><span data-stu-id="1a740-103">binaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="1a740-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a740-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a740-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1a740-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a740-106">Выражение условия управления, вычисляемое с помощью бинарной операции.</span><span class="sxs-lookup"><span data-stu-id="1a740-106">A management condition expression that is evaluated using a binary operation.</span></span>


<span data-ttu-id="1a740-107">Наследуется от [манажементкондитионекспрессионмодел](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="1a740-107">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1a740-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="1a740-108">Properties</span></span>
|<span data-ttu-id="1a740-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="1a740-109">Property</span></span>|<span data-ttu-id="1a740-110">Тип</span><span class="sxs-lookup"><span data-stu-id="1a740-110">Type</span></span>|<span data-ttu-id="1a740-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1a740-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a740-112">operator</span><span class="sxs-lookup"><span data-stu-id="1a740-112">operator</span></span>|[<span data-ttu-id="1a740-113">бинариманажементкондитионекспрессионоператортипе</span><span class="sxs-lookup"><span data-stu-id="1a740-113">binaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-binarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="1a740-114">Оператор, используемый для оценки бинарной операции.</span><span class="sxs-lookup"><span data-stu-id="1a740-114">The operator used in the evaluation of the binary operation.</span></span> <span data-ttu-id="1a740-115">Возможные значения: `or`, `and`.</span><span class="sxs-lookup"><span data-stu-id="1a740-115">Possible values are: `or`, `and`.</span></span>|
|<span data-ttu-id="1a740-116">фирстоперанд</span><span class="sxs-lookup"><span data-stu-id="1a740-116">firstOperand</span></span>|[<span data-ttu-id="1a740-117">манажементкондитионекспрессионмодел</span><span class="sxs-lookup"><span data-stu-id="1a740-117">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="1a740-118">Первый операнд бинарной операции.</span><span class="sxs-lookup"><span data-stu-id="1a740-118">The first operand of the binary operation.</span></span>|
|<span data-ttu-id="1a740-119">секондоперанд</span><span class="sxs-lookup"><span data-stu-id="1a740-119">secondOperand</span></span>|[<span data-ttu-id="1a740-120">манажементкондитионекспрессионмодел</span><span class="sxs-lookup"><span data-stu-id="1a740-120">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="1a740-121">Второй операнд бинарной операции.</span><span class="sxs-lookup"><span data-stu-id="1a740-121">The second operand of the binary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a740-122">Связи</span><span class="sxs-lookup"><span data-stu-id="1a740-122">Relationships</span></span>
<span data-ttu-id="1a740-123">Нет</span><span class="sxs-lookup"><span data-stu-id="1a740-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1a740-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1a740-124">JSON Representation</span></span>
<span data-ttu-id="1a740-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1a740-125">Here is a JSON representation of the resource.</span></span>
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



