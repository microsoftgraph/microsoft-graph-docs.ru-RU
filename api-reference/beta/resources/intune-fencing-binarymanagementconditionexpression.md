---
title: Тип ресурса Бинариманажементкондитионекспрессион
description: Выражение условия управления, вычисляемое с помощью бинарной операции.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d0919ac70a5855900aef5f87ad5f63e35e28b60a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528197"
---
# <a name="binarymanagementconditionexpression-resource-type"></a><span data-ttu-id="7e6ed-103">Тип ресурса Бинариманажементкондитионекспрессион</span><span class="sxs-lookup"><span data-stu-id="7e6ed-103">binaryManagementConditionExpression resource type</span></span>

<span data-ttu-id="7e6ed-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7e6ed-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7e6ed-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e6ed-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e6ed-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7e6ed-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e6ed-107">Выражение условия управления, вычисляемое с помощью бинарной операции.</span><span class="sxs-lookup"><span data-stu-id="7e6ed-107">A management condition expression that is evaluated using a binary operation.</span></span>


<span data-ttu-id="7e6ed-108">Наследуется от [манажементкондитионекспрессионмодел](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="7e6ed-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7e6ed-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="7e6ed-109">Properties</span></span>
|<span data-ttu-id="7e6ed-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="7e6ed-110">Property</span></span>|<span data-ttu-id="7e6ed-111">Тип</span><span class="sxs-lookup"><span data-stu-id="7e6ed-111">Type</span></span>|<span data-ttu-id="7e6ed-112">Описание</span><span class="sxs-lookup"><span data-stu-id="7e6ed-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e6ed-113">operator</span><span class="sxs-lookup"><span data-stu-id="7e6ed-113">operator</span></span>|[<span data-ttu-id="7e6ed-114">бинариманажементкондитионекспрессионоператортипе</span><span class="sxs-lookup"><span data-stu-id="7e6ed-114">binaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-binarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="7e6ed-115">Оператор, используемый для оценки бинарной операции.</span><span class="sxs-lookup"><span data-stu-id="7e6ed-115">The operator used in the evaluation of the binary operation.</span></span> <span data-ttu-id="7e6ed-116">Возможные значения: `or`, `and`.</span><span class="sxs-lookup"><span data-stu-id="7e6ed-116">Possible values are: `or`, `and`.</span></span>|
|<span data-ttu-id="7e6ed-117">фирстоперанд</span><span class="sxs-lookup"><span data-stu-id="7e6ed-117">firstOperand</span></span>|[<span data-ttu-id="7e6ed-118">манажементкондитионекспрессионмодел</span><span class="sxs-lookup"><span data-stu-id="7e6ed-118">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="7e6ed-119">Первый операнд бинарной операции.</span><span class="sxs-lookup"><span data-stu-id="7e6ed-119">The first operand of the binary operation.</span></span>|
|<span data-ttu-id="7e6ed-120">секондоперанд</span><span class="sxs-lookup"><span data-stu-id="7e6ed-120">secondOperand</span></span>|[<span data-ttu-id="7e6ed-121">манажементкондитионекспрессионмодел</span><span class="sxs-lookup"><span data-stu-id="7e6ed-121">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="7e6ed-122">Второй операнд бинарной операции.</span><span class="sxs-lookup"><span data-stu-id="7e6ed-122">The second operand of the binary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e6ed-123">Связи</span><span class="sxs-lookup"><span data-stu-id="7e6ed-123">Relationships</span></span>
<span data-ttu-id="7e6ed-124">Нет</span><span class="sxs-lookup"><span data-stu-id="7e6ed-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7e6ed-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7e6ed-125">JSON Representation</span></span>
<span data-ttu-id="7e6ed-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7e6ed-126">Here is a JSON representation of the resource.</span></span>
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



