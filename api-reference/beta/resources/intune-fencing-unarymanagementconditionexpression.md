---
title: Тип ресурса Унариманажементкондитионекспрессион
description: Выражение условия управления, вычисляемое с использованием унарной операции.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6554f62805bcd1d45f6db165367624434e794117
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561882"
---
# <a name="unarymanagementconditionexpression-resource-type"></a><span data-ttu-id="52512-103">Тип ресурса Унариманажементкондитионекспрессион</span><span class="sxs-lookup"><span data-stu-id="52512-103">unaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="52512-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52512-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="52512-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="52512-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52512-106">Выражение условия управления, вычисляемое с использованием унарной операции.</span><span class="sxs-lookup"><span data-stu-id="52512-106">A management condition expression that is evaluated using a unary operation.</span></span>


<span data-ttu-id="52512-107">НаСледуется от [манажементкондитионекспрессионмодел](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="52512-107">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="52512-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="52512-108">Properties</span></span>
|<span data-ttu-id="52512-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="52512-109">Property</span></span>|<span data-ttu-id="52512-110">Тип</span><span class="sxs-lookup"><span data-stu-id="52512-110">Type</span></span>|<span data-ttu-id="52512-111">Описание</span><span class="sxs-lookup"><span data-stu-id="52512-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52512-112">operator</span><span class="sxs-lookup"><span data-stu-id="52512-112">operator</span></span>|[<span data-ttu-id="52512-113">Унариманажементкондитионекспрессионоператортипе</span><span class="sxs-lookup"><span data-stu-id="52512-113">unaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-unarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="52512-114">Оператор, используемый в оценке унарной операции.</span><span class="sxs-lookup"><span data-stu-id="52512-114">The operator used in the evaluation of the unary operation.</span></span> <span data-ttu-id="52512-115">Возможные значения: `not`.</span><span class="sxs-lookup"><span data-stu-id="52512-115">Possible values are: `not`.</span></span>|
|<span data-ttu-id="52512-116">начинается</span><span class="sxs-lookup"><span data-stu-id="52512-116">operand</span></span>|[<span data-ttu-id="52512-117">Манажементкондитионекспрессионмодел</span><span class="sxs-lookup"><span data-stu-id="52512-117">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="52512-118">Операнд унарной операции.</span><span class="sxs-lookup"><span data-stu-id="52512-118">The operand of the unary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="52512-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="52512-119">Relationships</span></span>
<span data-ttu-id="52512-120">Нет</span><span class="sxs-lookup"><span data-stu-id="52512-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="52512-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="52512-121">JSON Representation</span></span>
<span data-ttu-id="52512-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="52512-122">Here is a JSON representation of the resource.</span></span>
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





