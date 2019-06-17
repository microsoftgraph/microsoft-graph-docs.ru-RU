---
title: Тип ресурса Унариманажементкондитионекспрессион
description: Выражение условия управления, вычисляемое с использованием унарной операции.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5eb5e7ed67b0731cc795ab791c2463294764ead6
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34990108"
---
# <a name="unarymanagementconditionexpression-resource-type"></a><span data-ttu-id="e8fa8-103">Тип ресурса Унариманажементкондитионекспрессион</span><span class="sxs-lookup"><span data-stu-id="e8fa8-103">unaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="e8fa8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8fa8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8fa8-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e8fa8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8fa8-106">Выражение условия управления, вычисляемое с использованием унарной операции.</span><span class="sxs-lookup"><span data-stu-id="e8fa8-106">A management condition expression that is evaluated using a unary operation.</span></span>


<span data-ttu-id="e8fa8-107">Наследуется от [манажементкондитионекспрессионмодел](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="e8fa8-107">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e8fa8-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e8fa8-108">Properties</span></span>
|<span data-ttu-id="e8fa8-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e8fa8-109">Property</span></span>|<span data-ttu-id="e8fa8-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e8fa8-110">Type</span></span>|<span data-ttu-id="e8fa8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e8fa8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8fa8-112">operator</span><span class="sxs-lookup"><span data-stu-id="e8fa8-112">operator</span></span>|[<span data-ttu-id="e8fa8-113">Унариманажементкондитионекспрессионоператортипе</span><span class="sxs-lookup"><span data-stu-id="e8fa8-113">unaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-unarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="e8fa8-114">Оператор, используемый в оценке унарной операции.</span><span class="sxs-lookup"><span data-stu-id="e8fa8-114">The operator used in the evaluation of the unary operation.</span></span> <span data-ttu-id="e8fa8-115">Возможные значения: `not`.</span><span class="sxs-lookup"><span data-stu-id="e8fa8-115">Possible values are: `not`.</span></span>|
|<span data-ttu-id="e8fa8-116">начинается</span><span class="sxs-lookup"><span data-stu-id="e8fa8-116">operand</span></span>|[<span data-ttu-id="e8fa8-117">Манажементкондитионекспрессионмодел</span><span class="sxs-lookup"><span data-stu-id="e8fa8-117">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="e8fa8-118">Операнд унарной операции.</span><span class="sxs-lookup"><span data-stu-id="e8fa8-118">The operand of the unary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e8fa8-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="e8fa8-119">Relationships</span></span>
<span data-ttu-id="e8fa8-120">Нет</span><span class="sxs-lookup"><span data-stu-id="e8fa8-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e8fa8-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e8fa8-121">JSON Representation</span></span>
<span data-ttu-id="e8fa8-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e8fa8-122">Here is a JSON representation of the resource.</span></span>
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





