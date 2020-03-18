---
title: Тип ресурса Вариаблеманажементкондитионекспрессион
description: Оценивает состояние условия управления как логическое выражение.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 363f19e2f8b6860ba0228cd6a29a07dd82bd8277
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783181"
---
# <a name="variablemanagementconditionexpression-resource-type"></a><span data-ttu-id="19443-103">Тип ресурса Вариаблеманажементкондитионекспрессион</span><span class="sxs-lookup"><span data-stu-id="19443-103">variableManagementConditionExpression resource type</span></span>

> <span data-ttu-id="19443-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19443-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="19443-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="19443-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19443-106">Оценивает состояние условия управления как логическое выражение.</span><span class="sxs-lookup"><span data-stu-id="19443-106">Evaluates the management condition state as a Boolean expression.</span></span>


<span data-ttu-id="19443-107">Наследуется от [манажементкондитионекспрессионмодел](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="19443-107">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="19443-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="19443-108">Properties</span></span>
|<span data-ttu-id="19443-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="19443-109">Property</span></span>|<span data-ttu-id="19443-110">Тип</span><span class="sxs-lookup"><span data-stu-id="19443-110">Type</span></span>|<span data-ttu-id="19443-111">Описание</span><span class="sxs-lookup"><span data-stu-id="19443-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19443-112">манажементкондитионид</span><span class="sxs-lookup"><span data-stu-id="19443-112">managementConditionId</span></span>|<span data-ttu-id="19443-113">String</span><span class="sxs-lookup"><span data-stu-id="19443-113">String</span></span>|<span data-ttu-id="19443-114">Идентификатор условия управления, используемый для оценки выражения.</span><span class="sxs-lookup"><span data-stu-id="19443-114">The management condition id that is used to evaluate the expression.</span></span>|

## <a name="relationships"></a><span data-ttu-id="19443-115">Связи</span><span class="sxs-lookup"><span data-stu-id="19443-115">Relationships</span></span>
<span data-ttu-id="19443-116">Нет</span><span class="sxs-lookup"><span data-stu-id="19443-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="19443-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="19443-117">JSON Representation</span></span>
<span data-ttu-id="19443-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="19443-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.variableManagementConditionExpression"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.variableManagementConditionExpression",
  "managementConditionId": "String"
}
```



