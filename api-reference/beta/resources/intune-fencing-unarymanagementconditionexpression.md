---
title: Тип ресурса Унариманажементкондитионекспрессион
description: Выражение условия управления, вычисляемое с использованием унарной операции.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4616a7b7bdb54d1bb205d545db4ff7eecbeedbb5
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783195"
---
# <a name="unarymanagementconditionexpression-resource-type"></a><span data-ttu-id="68d0a-103">Тип ресурса Унариманажементкондитионекспрессион</span><span class="sxs-lookup"><span data-stu-id="68d0a-103">unaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="68d0a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68d0a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="68d0a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="68d0a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68d0a-106">Выражение условия управления, вычисляемое с использованием унарной операции.</span><span class="sxs-lookup"><span data-stu-id="68d0a-106">A management condition expression that is evaluated using a unary operation.</span></span>


<span data-ttu-id="68d0a-107">Наследуется от [манажементкондитионекспрессионмодел](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="68d0a-107">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="68d0a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="68d0a-108">Properties</span></span>
|<span data-ttu-id="68d0a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="68d0a-109">Property</span></span>|<span data-ttu-id="68d0a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="68d0a-110">Type</span></span>|<span data-ttu-id="68d0a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="68d0a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68d0a-112">operator</span><span class="sxs-lookup"><span data-stu-id="68d0a-112">operator</span></span>|[<span data-ttu-id="68d0a-113">унариманажементкондитионекспрессионоператортипе</span><span class="sxs-lookup"><span data-stu-id="68d0a-113">unaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-unarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="68d0a-114">Оператор, используемый в оценке унарной операции.</span><span class="sxs-lookup"><span data-stu-id="68d0a-114">The operator used in the evaluation of the unary operation.</span></span> <span data-ttu-id="68d0a-115">Возможные значения: `not`.</span><span class="sxs-lookup"><span data-stu-id="68d0a-115">Possible values are: `not`.</span></span>|
|<span data-ttu-id="68d0a-116">начинается</span><span class="sxs-lookup"><span data-stu-id="68d0a-116">operand</span></span>|[<span data-ttu-id="68d0a-117">манажементкондитионекспрессионмодел</span><span class="sxs-lookup"><span data-stu-id="68d0a-117">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="68d0a-118">Операнд унарной операции.</span><span class="sxs-lookup"><span data-stu-id="68d0a-118">The operand of the unary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="68d0a-119">Связи</span><span class="sxs-lookup"><span data-stu-id="68d0a-119">Relationships</span></span>
<span data-ttu-id="68d0a-120">Нет</span><span class="sxs-lookup"><span data-stu-id="68d0a-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="68d0a-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="68d0a-121">JSON Representation</span></span>
<span data-ttu-id="68d0a-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="68d0a-122">Here is a JSON representation of the resource.</span></span>
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



