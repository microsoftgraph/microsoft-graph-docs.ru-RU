---
title: Тип ресурса unaryManagementConditionExpression
description: Выражение условия управления, который вычисляется с использованием унарного.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 619d931e53fbd65419e07ab1b2f27341ccb5dd41
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829773"
---
# <a name="unarymanagementconditionexpression-resource-type"></a><span data-ttu-id="91ff4-103">Тип ресурса unaryManagementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="91ff4-103">unaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="91ff4-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="91ff4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="91ff4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91ff4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="91ff4-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="91ff4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="91ff4-107">Выражение условия управления, который вычисляется с использованием унарного.</span><span class="sxs-lookup"><span data-stu-id="91ff4-107">A management condition expression that is evaluated using a unary operation.</span></span>

<span data-ttu-id="91ff4-108">Наследуется от [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="91ff4-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="91ff4-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="91ff4-109">Properties</span></span>
|<span data-ttu-id="91ff4-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="91ff4-110">Property</span></span>|<span data-ttu-id="91ff4-111">Тип</span><span class="sxs-lookup"><span data-stu-id="91ff4-111">Type</span></span>|<span data-ttu-id="91ff4-112">Описание</span><span class="sxs-lookup"><span data-stu-id="91ff4-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91ff4-113">operator</span><span class="sxs-lookup"><span data-stu-id="91ff4-113">operator</span></span>|[<span data-ttu-id="91ff4-114">unaryManagementConditionExpressionOperatorType</span><span class="sxs-lookup"><span data-stu-id="91ff4-114">unaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-unarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="91ff4-115">Оператор, используемый в оценке унарного.</span><span class="sxs-lookup"><span data-stu-id="91ff4-115">The operator used in the evaluation of the unary operation.</span></span> <span data-ttu-id="91ff4-116">Возможные значения: `not`.</span><span class="sxs-lookup"><span data-stu-id="91ff4-116">Possible values are: `not`.</span></span>|
|<span data-ttu-id="91ff4-117">операнд</span><span class="sxs-lookup"><span data-stu-id="91ff4-117">operand</span></span>|[<span data-ttu-id="91ff4-118">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="91ff4-118">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="91ff4-119">Операнд унарного.</span><span class="sxs-lookup"><span data-stu-id="91ff4-119">The operand of the unary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="91ff4-120">Связи</span><span class="sxs-lookup"><span data-stu-id="91ff4-120">Relationships</span></span>
<span data-ttu-id="91ff4-121">Нет</span><span class="sxs-lookup"><span data-stu-id="91ff4-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="91ff4-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="91ff4-122">JSON Representation</span></span>
<span data-ttu-id="91ff4-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="91ff4-123">Here is a JSON representation of the resource.</span></span>
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





