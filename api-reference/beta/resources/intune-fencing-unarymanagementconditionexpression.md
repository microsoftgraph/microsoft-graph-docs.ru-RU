---
title: Тип ресурса Унариманажементкондитионекспрессион
description: Выражение условия управления, вычисляемое с использованием унарной операции.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1f0bd5282307d1c8619f756d79209fb04a86bef2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43453239"
---
# <a name="unarymanagementconditionexpression-resource-type"></a><span data-ttu-id="6c44f-103">Тип ресурса Унариманажементкондитионекспрессион</span><span class="sxs-lookup"><span data-stu-id="6c44f-103">unaryManagementConditionExpression resource type</span></span>

<span data-ttu-id="6c44f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c44f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6c44f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c44f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c44f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6c44f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c44f-107">Выражение условия управления, вычисляемое с использованием унарной операции.</span><span class="sxs-lookup"><span data-stu-id="6c44f-107">A management condition expression that is evaluated using a unary operation.</span></span>


<span data-ttu-id="6c44f-108">Наследуется от [манажементкондитионекспрессионмодел](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="6c44f-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6c44f-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="6c44f-109">Properties</span></span>
|<span data-ttu-id="6c44f-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="6c44f-110">Property</span></span>|<span data-ttu-id="6c44f-111">Тип</span><span class="sxs-lookup"><span data-stu-id="6c44f-111">Type</span></span>|<span data-ttu-id="6c44f-112">Описание</span><span class="sxs-lookup"><span data-stu-id="6c44f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c44f-113">operator</span><span class="sxs-lookup"><span data-stu-id="6c44f-113">operator</span></span>|[<span data-ttu-id="6c44f-114">унариманажементкондитионекспрессионоператортипе</span><span class="sxs-lookup"><span data-stu-id="6c44f-114">unaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-unarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="6c44f-115">Оператор, используемый в оценке унарной операции.</span><span class="sxs-lookup"><span data-stu-id="6c44f-115">The operator used in the evaluation of the unary operation.</span></span> <span data-ttu-id="6c44f-116">Возможные значения: `not`.</span><span class="sxs-lookup"><span data-stu-id="6c44f-116">Possible values are: `not`.</span></span>|
|<span data-ttu-id="6c44f-117">начинается</span><span class="sxs-lookup"><span data-stu-id="6c44f-117">operand</span></span>|[<span data-ttu-id="6c44f-118">манажементкондитионекспрессионмодел</span><span class="sxs-lookup"><span data-stu-id="6c44f-118">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="6c44f-119">Операнд унарной операции.</span><span class="sxs-lookup"><span data-stu-id="6c44f-119">The operand of the unary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6c44f-120">Связи</span><span class="sxs-lookup"><span data-stu-id="6c44f-120">Relationships</span></span>
<span data-ttu-id="6c44f-121">Нет</span><span class="sxs-lookup"><span data-stu-id="6c44f-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6c44f-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6c44f-122">JSON Representation</span></span>
<span data-ttu-id="6c44f-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6c44f-123">Here is a JSON representation of the resource.</span></span>
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



