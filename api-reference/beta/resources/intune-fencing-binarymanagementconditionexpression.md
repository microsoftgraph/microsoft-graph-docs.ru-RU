---
title: Тип ресурса Бинариманажементкондитионекспрессион
description: Выражение условия управления, вычисляемое с помощью бинарной операции.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b16bd0ec8aecffd4f0221ca9cabbc925e26e059a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36326725"
---
# <a name="binarymanagementconditionexpression-resource-type"></a><span data-ttu-id="8d8c1-103">Тип ресурса Бинариманажементкондитионекспрессион</span><span class="sxs-lookup"><span data-stu-id="8d8c1-103">binaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="8d8c1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d8c1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d8c1-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8d8c1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d8c1-106">Выражение условия управления, вычисляемое с помощью бинарной операции.</span><span class="sxs-lookup"><span data-stu-id="8d8c1-106">A management condition expression that is evaluated using a binary operation.</span></span>


<span data-ttu-id="8d8c1-107">Наследуется от [манажементкондитионекспрессионмодел](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="8d8c1-107">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8d8c1-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="8d8c1-108">Properties</span></span>
|<span data-ttu-id="8d8c1-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="8d8c1-109">Property</span></span>|<span data-ttu-id="8d8c1-110">Тип</span><span class="sxs-lookup"><span data-stu-id="8d8c1-110">Type</span></span>|<span data-ttu-id="8d8c1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8d8c1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d8c1-112">operator</span><span class="sxs-lookup"><span data-stu-id="8d8c1-112">operator</span></span>|[<span data-ttu-id="8d8c1-113">бинариманажементкондитионекспрессионоператортипе</span><span class="sxs-lookup"><span data-stu-id="8d8c1-113">binaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-binarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="8d8c1-114">Оператор, используемый для оценки бинарной операции.</span><span class="sxs-lookup"><span data-stu-id="8d8c1-114">The operator used in the evaluation of the binary operation.</span></span> <span data-ttu-id="8d8c1-115">Возможные значения: `or`, `and`.</span><span class="sxs-lookup"><span data-stu-id="8d8c1-115">Possible values are: `or`, `and`.</span></span>|
|<span data-ttu-id="8d8c1-116">фирстоперанд</span><span class="sxs-lookup"><span data-stu-id="8d8c1-116">firstOperand</span></span>|[<span data-ttu-id="8d8c1-117">манажементкондитионекспрессионмодел</span><span class="sxs-lookup"><span data-stu-id="8d8c1-117">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="8d8c1-118">Первый операнд бинарной операции.</span><span class="sxs-lookup"><span data-stu-id="8d8c1-118">The first operand of the binary operation.</span></span>|
|<span data-ttu-id="8d8c1-119">секондоперанд</span><span class="sxs-lookup"><span data-stu-id="8d8c1-119">secondOperand</span></span>|[<span data-ttu-id="8d8c1-120">манажементкондитионекспрессионмодел</span><span class="sxs-lookup"><span data-stu-id="8d8c1-120">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="8d8c1-121">Второй операнд бинарной операции.</span><span class="sxs-lookup"><span data-stu-id="8d8c1-121">The second operand of the binary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8d8c1-122">Отношения</span><span class="sxs-lookup"><span data-stu-id="8d8c1-122">Relationships</span></span>
<span data-ttu-id="8d8c1-123">Нет</span><span class="sxs-lookup"><span data-stu-id="8d8c1-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8d8c1-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8d8c1-124">JSON Representation</span></span>
<span data-ttu-id="8d8c1-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8d8c1-125">Here is a JSON representation of the resource.</span></span>
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



