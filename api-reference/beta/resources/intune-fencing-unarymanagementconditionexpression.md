---
title: Тип ресурса Унариманажементкондитионекспрессион
description: Выражение условия управления, вычисляемое с использованием унарной операции.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 403867dcbdcc0767043fbe873c6de6b415eb32f9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524506"
---
# <a name="unarymanagementconditionexpression-resource-type"></a><span data-ttu-id="dd572-103">Тип ресурса Унариманажементкондитионекспрессион</span><span class="sxs-lookup"><span data-stu-id="dd572-103">unaryManagementConditionExpression resource type</span></span>

<span data-ttu-id="dd572-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="dd572-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dd572-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd572-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dd572-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dd572-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd572-107">Выражение условия управления, вычисляемое с использованием унарной операции.</span><span class="sxs-lookup"><span data-stu-id="dd572-107">A management condition expression that is evaluated using a unary operation.</span></span>


<span data-ttu-id="dd572-108">Наследуется от [манажементкондитионекспрессионмодел](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="dd572-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="dd572-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="dd572-109">Properties</span></span>
|<span data-ttu-id="dd572-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd572-110">Property</span></span>|<span data-ttu-id="dd572-111">Тип</span><span class="sxs-lookup"><span data-stu-id="dd572-111">Type</span></span>|<span data-ttu-id="dd572-112">Описание</span><span class="sxs-lookup"><span data-stu-id="dd572-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd572-113">operator</span><span class="sxs-lookup"><span data-stu-id="dd572-113">operator</span></span>|[<span data-ttu-id="dd572-114">унариманажементкондитионекспрессионоператортипе</span><span class="sxs-lookup"><span data-stu-id="dd572-114">unaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-unarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="dd572-115">Оператор, используемый в оценке унарной операции.</span><span class="sxs-lookup"><span data-stu-id="dd572-115">The operator used in the evaluation of the unary operation.</span></span> <span data-ttu-id="dd572-116">Возможные значения: `not`.</span><span class="sxs-lookup"><span data-stu-id="dd572-116">Possible values are: `not`.</span></span>|
|<span data-ttu-id="dd572-117">начинается</span><span class="sxs-lookup"><span data-stu-id="dd572-117">operand</span></span>|[<span data-ttu-id="dd572-118">манажементкондитионекспрессионмодел</span><span class="sxs-lookup"><span data-stu-id="dd572-118">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="dd572-119">Операнд унарной операции.</span><span class="sxs-lookup"><span data-stu-id="dd572-119">The operand of the unary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dd572-120">Связи</span><span class="sxs-lookup"><span data-stu-id="dd572-120">Relationships</span></span>
<span data-ttu-id="dd572-121">Нет</span><span class="sxs-lookup"><span data-stu-id="dd572-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dd572-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dd572-122">JSON Representation</span></span>
<span data-ttu-id="dd572-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dd572-123">Here is a JSON representation of the resource.</span></span>
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



