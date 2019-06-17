---
title: Тип ресурса Бинариманажементкондитионекспрессион
description: Выражение условия управления, вычисляемое с помощью бинарной операции.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 97c812c3a26af0401bbdea87997167bcada05a37
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34994820"
---
# <a name="binarymanagementconditionexpression-resource-type"></a><span data-ttu-id="c72c8-103">Тип ресурса Бинариманажементкондитионекспрессион</span><span class="sxs-lookup"><span data-stu-id="c72c8-103">binaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="c72c8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c72c8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c72c8-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c72c8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c72c8-106">Выражение условия управления, вычисляемое с помощью бинарной операции.</span><span class="sxs-lookup"><span data-stu-id="c72c8-106">A management condition expression that is evaluated using a binary operation.</span></span>


<span data-ttu-id="c72c8-107">Наследуется от [манажементкондитионекспрессионмодел](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="c72c8-107">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c72c8-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c72c8-108">Properties</span></span>
|<span data-ttu-id="c72c8-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c72c8-109">Property</span></span>|<span data-ttu-id="c72c8-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c72c8-110">Type</span></span>|<span data-ttu-id="c72c8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c72c8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c72c8-112">operator</span><span class="sxs-lookup"><span data-stu-id="c72c8-112">operator</span></span>|[<span data-ttu-id="c72c8-113">Бинариманажементкондитионекспрессионоператортипе</span><span class="sxs-lookup"><span data-stu-id="c72c8-113">binaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-binarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="c72c8-114">Оператор, используемый для оценки бинарной операции.</span><span class="sxs-lookup"><span data-stu-id="c72c8-114">The operator used in the evaluation of the binary operation.</span></span> <span data-ttu-id="c72c8-115">Возможные значения: `or`, `and`.</span><span class="sxs-lookup"><span data-stu-id="c72c8-115">Possible values are: `or`, `and`.</span></span>|
|<span data-ttu-id="c72c8-116">Фирстоперанд</span><span class="sxs-lookup"><span data-stu-id="c72c8-116">firstOperand</span></span>|[<span data-ttu-id="c72c8-117">Манажементкондитионекспрессионмодел</span><span class="sxs-lookup"><span data-stu-id="c72c8-117">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="c72c8-118">Первый операнд бинарной операции.</span><span class="sxs-lookup"><span data-stu-id="c72c8-118">The first operand of the binary operation.</span></span>|
|<span data-ttu-id="c72c8-119">Секондоперанд</span><span class="sxs-lookup"><span data-stu-id="c72c8-119">secondOperand</span></span>|[<span data-ttu-id="c72c8-120">Манажементкондитионекспрессионмодел</span><span class="sxs-lookup"><span data-stu-id="c72c8-120">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="c72c8-121">Второй операнд бинарной операции.</span><span class="sxs-lookup"><span data-stu-id="c72c8-121">The second operand of the binary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c72c8-122">Отношения</span><span class="sxs-lookup"><span data-stu-id="c72c8-122">Relationships</span></span>
<span data-ttu-id="c72c8-123">Нет</span><span class="sxs-lookup"><span data-stu-id="c72c8-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c72c8-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c72c8-124">JSON Representation</span></span>
<span data-ttu-id="c72c8-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c72c8-125">Here is a JSON representation of the resource.</span></span>
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





