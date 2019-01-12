---
title: Тип ресурса unaryManagementConditionExpression
description: Выражение условия управления, который вычисляется с использованием унарного.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 06a379a53d6d85956a54bede444714e082196ba3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949425"
---
# <a name="unarymanagementconditionexpression-resource-type"></a><span data-ttu-id="d2ef5-103">Тип ресурса unaryManagementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="d2ef5-103">unaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="d2ef5-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d2ef5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d2ef5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2ef5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d2ef5-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d2ef5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d2ef5-107">Выражение условия управления, который вычисляется с использованием унарного.</span><span class="sxs-lookup"><span data-stu-id="d2ef5-107">A management condition expression that is evaluated using a unary operation.</span></span>

<span data-ttu-id="d2ef5-108">Наследуется от [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="d2ef5-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d2ef5-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="d2ef5-109">Properties</span></span>
|<span data-ttu-id="d2ef5-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="d2ef5-110">Property</span></span>|<span data-ttu-id="d2ef5-111">Тип</span><span class="sxs-lookup"><span data-stu-id="d2ef5-111">Type</span></span>|<span data-ttu-id="d2ef5-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d2ef5-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2ef5-113">operator</span><span class="sxs-lookup"><span data-stu-id="d2ef5-113">operator</span></span>|[<span data-ttu-id="d2ef5-114">unaryManagementConditionExpressionOperatorType</span><span class="sxs-lookup"><span data-stu-id="d2ef5-114">unaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-unarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="d2ef5-115">Оператор, используемый в оценке унарного.</span><span class="sxs-lookup"><span data-stu-id="d2ef5-115">The operator used in the evaluation of the unary operation.</span></span> <span data-ttu-id="d2ef5-116">Возможные значения: `not`.</span><span class="sxs-lookup"><span data-stu-id="d2ef5-116">Possible values are: `not`.</span></span>|
|<span data-ttu-id="d2ef5-117">операнд</span><span class="sxs-lookup"><span data-stu-id="d2ef5-117">operand</span></span>|[<span data-ttu-id="d2ef5-118">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="d2ef5-118">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="d2ef5-119">Операнд унарного.</span><span class="sxs-lookup"><span data-stu-id="d2ef5-119">The operand of the unary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2ef5-120">Связи</span><span class="sxs-lookup"><span data-stu-id="d2ef5-120">Relationships</span></span>
<span data-ttu-id="d2ef5-121">Нет</span><span class="sxs-lookup"><span data-stu-id="d2ef5-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d2ef5-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d2ef5-122">JSON Representation</span></span>
<span data-ttu-id="d2ef5-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d2ef5-123">Here is a JSON representation of the resource.</span></span>
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





