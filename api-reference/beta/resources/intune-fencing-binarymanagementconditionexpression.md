---
title: Тип ресурса Бинариманажементкондитионекспрессион
description: Выражение условия управления, вычисляемое с помощью бинарной операции.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f4782fb9fc7f1af9110622d9714c6f67e59bd89e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36011136"
---
# <a name="binarymanagementconditionexpression-resource-type"></a><span data-ttu-id="98b90-103">Тип ресурса Бинариманажементкондитионекспрессион</span><span class="sxs-lookup"><span data-stu-id="98b90-103">binaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="98b90-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98b90-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="98b90-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="98b90-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98b90-106">Выражение условия управления, вычисляемое с помощью бинарной операции.</span><span class="sxs-lookup"><span data-stu-id="98b90-106">A management condition expression that is evaluated using a binary operation.</span></span>


<span data-ttu-id="98b90-107">Наследуется от [манажементкондитионекспрессионмодел](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="98b90-107">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="98b90-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="98b90-108">Properties</span></span>
|<span data-ttu-id="98b90-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="98b90-109">Property</span></span>|<span data-ttu-id="98b90-110">Тип</span><span class="sxs-lookup"><span data-stu-id="98b90-110">Type</span></span>|<span data-ttu-id="98b90-111">Описание</span><span class="sxs-lookup"><span data-stu-id="98b90-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98b90-112">operator</span><span class="sxs-lookup"><span data-stu-id="98b90-112">operator</span></span>|[<span data-ttu-id="98b90-113">Бинариманажементкондитионекспрессионоператортипе</span><span class="sxs-lookup"><span data-stu-id="98b90-113">binaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-binarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="98b90-114">Оператор, используемый для оценки бинарной операции.</span><span class="sxs-lookup"><span data-stu-id="98b90-114">The operator used in the evaluation of the binary operation.</span></span> <span data-ttu-id="98b90-115">Возможные значения: `or`, `and`.</span><span class="sxs-lookup"><span data-stu-id="98b90-115">Possible values are: `or`, `and`.</span></span>|
|<span data-ttu-id="98b90-116">Фирстоперанд</span><span class="sxs-lookup"><span data-stu-id="98b90-116">firstOperand</span></span>|[<span data-ttu-id="98b90-117">Манажементкондитионекспрессионмодел</span><span class="sxs-lookup"><span data-stu-id="98b90-117">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="98b90-118">Первый операнд бинарной операции.</span><span class="sxs-lookup"><span data-stu-id="98b90-118">The first operand of the binary operation.</span></span>|
|<span data-ttu-id="98b90-119">Секондоперанд</span><span class="sxs-lookup"><span data-stu-id="98b90-119">secondOperand</span></span>|[<span data-ttu-id="98b90-120">Манажементкондитионекспрессионмодел</span><span class="sxs-lookup"><span data-stu-id="98b90-120">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="98b90-121">Второй операнд бинарной операции.</span><span class="sxs-lookup"><span data-stu-id="98b90-121">The second operand of the binary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="98b90-122">Отношения</span><span class="sxs-lookup"><span data-stu-id="98b90-122">Relationships</span></span>
<span data-ttu-id="98b90-123">Нет</span><span class="sxs-lookup"><span data-stu-id="98b90-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="98b90-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="98b90-124">JSON Representation</span></span>
<span data-ttu-id="98b90-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="98b90-125">Here is a JSON representation of the resource.</span></span>
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





