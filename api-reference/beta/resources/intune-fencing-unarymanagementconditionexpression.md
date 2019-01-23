---
title: Тип ресурса unaryManagementConditionExpression
description: Выражение условия управления, который вычисляется с использованием унарного.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f1224a869ec2ec9cae2f38273f7a68b64d3d7333
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406782"
---
# <a name="unarymanagementconditionexpression-resource-type"></a><span data-ttu-id="c5ae1-103">Тип ресурса unaryManagementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="c5ae1-103">unaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="c5ae1-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c5ae1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c5ae1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5ae1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c5ae1-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c5ae1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5ae1-107">Выражение условия управления, который вычисляется с использованием унарного.</span><span class="sxs-lookup"><span data-stu-id="c5ae1-107">A management condition expression that is evaluated using a unary operation.</span></span>


<span data-ttu-id="c5ae1-108">Наследуется от [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="c5ae1-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c5ae1-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="c5ae1-109">Properties</span></span>
|<span data-ttu-id="c5ae1-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="c5ae1-110">Property</span></span>|<span data-ttu-id="c5ae1-111">Тип</span><span class="sxs-lookup"><span data-stu-id="c5ae1-111">Type</span></span>|<span data-ttu-id="c5ae1-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c5ae1-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5ae1-113">operator</span><span class="sxs-lookup"><span data-stu-id="c5ae1-113">operator</span></span>|[<span data-ttu-id="c5ae1-114">unaryManagementConditionExpressionOperatorType</span><span class="sxs-lookup"><span data-stu-id="c5ae1-114">unaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-unarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="c5ae1-115">Оператор, используемый в оценке унарного.</span><span class="sxs-lookup"><span data-stu-id="c5ae1-115">The operator used in the evaluation of the unary operation.</span></span> <span data-ttu-id="c5ae1-116">Возможные значения: `not`.</span><span class="sxs-lookup"><span data-stu-id="c5ae1-116">Possible values are: `not`.</span></span>|
|<span data-ttu-id="c5ae1-117">операнд</span><span class="sxs-lookup"><span data-stu-id="c5ae1-117">operand</span></span>|[<span data-ttu-id="c5ae1-118">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="c5ae1-118">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="c5ae1-119">Операнд унарного.</span><span class="sxs-lookup"><span data-stu-id="c5ae1-119">The operand of the unary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c5ae1-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="c5ae1-120">Relationships</span></span>
<span data-ttu-id="c5ae1-121">Нет</span><span class="sxs-lookup"><span data-stu-id="c5ae1-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c5ae1-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c5ae1-122">JSON Representation</span></span>
<span data-ttu-id="c5ae1-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c5ae1-123">Here is a JSON representation of the resource.</span></span>
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




