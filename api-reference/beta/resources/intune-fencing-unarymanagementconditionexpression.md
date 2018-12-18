---
title: Тип ресурса unaryManagementConditionExpression
description: Выражение условия управления, который вычисляется с использованием унарного.
author: tfitzmac
ms.openlocfilehash: 43711e68d88bdf0854e8501377fbf3e30b25b3ec
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344347"
---
# <a name="unarymanagementconditionexpression-resource-type"></a><span data-ttu-id="6f347-103">Тип ресурса unaryManagementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="6f347-103">unaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="6f347-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6f347-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6f347-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f347-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6f347-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6f347-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6f347-107">Выражение условия управления, который вычисляется с использованием унарного.</span><span class="sxs-lookup"><span data-stu-id="6f347-107">A management condition expression that is evaluated using a unary operation.</span></span>

<span data-ttu-id="6f347-108">Наследуется от [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="6f347-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6f347-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="6f347-109">Properties</span></span>
|<span data-ttu-id="6f347-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f347-110">Property</span></span>|<span data-ttu-id="6f347-111">Тип</span><span class="sxs-lookup"><span data-stu-id="6f347-111">Type</span></span>|<span data-ttu-id="6f347-112">Описание</span><span class="sxs-lookup"><span data-stu-id="6f347-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f347-113">operator</span><span class="sxs-lookup"><span data-stu-id="6f347-113">operator</span></span>|[<span data-ttu-id="6f347-114">unaryManagementConditionExpressionOperatorType</span><span class="sxs-lookup"><span data-stu-id="6f347-114">unaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-unarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="6f347-115">Оператор, используемый в оценке унарного.</span><span class="sxs-lookup"><span data-stu-id="6f347-115">The operator used in the evaluation of the unary operation.</span></span> <span data-ttu-id="6f347-116">Возможные значения: `not`.</span><span class="sxs-lookup"><span data-stu-id="6f347-116">Possible values are: `not`.</span></span>|
|<span data-ttu-id="6f347-117">операнд</span><span class="sxs-lookup"><span data-stu-id="6f347-117">operand</span></span>|[<span data-ttu-id="6f347-118">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="6f347-118">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="6f347-119">Операнд унарного.</span><span class="sxs-lookup"><span data-stu-id="6f347-119">The operand of the unary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6f347-120">Связи</span><span class="sxs-lookup"><span data-stu-id="6f347-120">Relationships</span></span>
<span data-ttu-id="6f347-121">Нет</span><span class="sxs-lookup"><span data-stu-id="6f347-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6f347-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6f347-122">JSON Representation</span></span>
<span data-ttu-id="6f347-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6f347-123">Here is a JSON representation of the resource.</span></span>
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





