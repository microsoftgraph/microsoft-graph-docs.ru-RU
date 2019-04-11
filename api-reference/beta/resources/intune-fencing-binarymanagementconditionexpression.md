---
title: Тип ресурса Бинариманажементкондитионекспрессион
description: Выражение условия управления, вычисляемое с помощью бинарной операции.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 50092f7031719fb1050706ed81280a347638117d
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31799414"
---
# <a name="binarymanagementconditionexpression-resource-type"></a><span data-ttu-id="52d41-103">Тип ресурса Бинариманажементкондитионекспрессион</span><span class="sxs-lookup"><span data-stu-id="52d41-103">binaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="52d41-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52d41-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="52d41-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="52d41-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52d41-106">Выражение условия управления, вычисляемое с помощью бинарной операции.</span><span class="sxs-lookup"><span data-stu-id="52d41-106">A management condition expression that is evaluated using a binary operation.</span></span>


<span data-ttu-id="52d41-107">НаСледуется от [манажементкондитионекспрессионмодел](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="52d41-107">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="52d41-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="52d41-108">Properties</span></span>
|<span data-ttu-id="52d41-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="52d41-109">Property</span></span>|<span data-ttu-id="52d41-110">Тип</span><span class="sxs-lookup"><span data-stu-id="52d41-110">Type</span></span>|<span data-ttu-id="52d41-111">Описание</span><span class="sxs-lookup"><span data-stu-id="52d41-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52d41-112">operator</span><span class="sxs-lookup"><span data-stu-id="52d41-112">operator</span></span>|[<span data-ttu-id="52d41-113">Бинариманажементкондитионекспрессионоператортипе</span><span class="sxs-lookup"><span data-stu-id="52d41-113">binaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-binarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="52d41-114">Оператор, используемый для оценки бинарной операции.</span><span class="sxs-lookup"><span data-stu-id="52d41-114">The operator used in the evaluation of the binary operation.</span></span> <span data-ttu-id="52d41-115">Возможные значения: `or`, `and`.</span><span class="sxs-lookup"><span data-stu-id="52d41-115">Possible values are: `or`, `and`.</span></span>|
|<span data-ttu-id="52d41-116">Фирстоперанд</span><span class="sxs-lookup"><span data-stu-id="52d41-116">firstOperand</span></span>|[<span data-ttu-id="52d41-117">Манажементкондитионекспрессионмодел</span><span class="sxs-lookup"><span data-stu-id="52d41-117">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="52d41-118">Первый операнд бинарной операции.</span><span class="sxs-lookup"><span data-stu-id="52d41-118">The first operand of the binary operation.</span></span>|
|<span data-ttu-id="52d41-119">Секондоперанд</span><span class="sxs-lookup"><span data-stu-id="52d41-119">secondOperand</span></span>|[<span data-ttu-id="52d41-120">Манажементкондитионекспрессионмодел</span><span class="sxs-lookup"><span data-stu-id="52d41-120">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="52d41-121">Второй операнд бинарной операции.</span><span class="sxs-lookup"><span data-stu-id="52d41-121">The second operand of the binary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="52d41-122">Отношения</span><span class="sxs-lookup"><span data-stu-id="52d41-122">Relationships</span></span>
<span data-ttu-id="52d41-123">Нет</span><span class="sxs-lookup"><span data-stu-id="52d41-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="52d41-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="52d41-124">JSON Representation</span></span>
<span data-ttu-id="52d41-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="52d41-125">Here is a JSON representation of the resource.</span></span>
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





