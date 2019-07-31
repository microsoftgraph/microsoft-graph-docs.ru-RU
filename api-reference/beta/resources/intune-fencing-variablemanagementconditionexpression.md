---
title: Тип ресурса Вариаблеманажементкондитионекспрессион
description: Оценивает состояние условия управления как логическое выражение.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8f091be4d717d57e447eacce08fb0a24905f1c14
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36011052"
---
# <a name="variablemanagementconditionexpression-resource-type"></a><span data-ttu-id="5def3-103">Тип ресурса Вариаблеманажементкондитионекспрессион</span><span class="sxs-lookup"><span data-stu-id="5def3-103">variableManagementConditionExpression resource type</span></span>

> <span data-ttu-id="5def3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5def3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5def3-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5def3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5def3-106">Оценивает состояние условия управления как логическое выражение.</span><span class="sxs-lookup"><span data-stu-id="5def3-106">Evaluates the management condition state as a Boolean expression.</span></span>


<span data-ttu-id="5def3-107">Наследуется от [манажементкондитионекспрессионмодел](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="5def3-107">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5def3-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="5def3-108">Properties</span></span>
|<span data-ttu-id="5def3-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="5def3-109">Property</span></span>|<span data-ttu-id="5def3-110">Тип</span><span class="sxs-lookup"><span data-stu-id="5def3-110">Type</span></span>|<span data-ttu-id="5def3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5def3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5def3-112">Манажементкондитионид</span><span class="sxs-lookup"><span data-stu-id="5def3-112">managementConditionId</span></span>|<span data-ttu-id="5def3-113">String</span><span class="sxs-lookup"><span data-stu-id="5def3-113">String</span></span>|<span data-ttu-id="5def3-114">Идентификатор условия управления, используемый для оценки выражения.</span><span class="sxs-lookup"><span data-stu-id="5def3-114">The management condition id that is used to evaluate the expression.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5def3-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="5def3-115">Relationships</span></span>
<span data-ttu-id="5def3-116">Нет</span><span class="sxs-lookup"><span data-stu-id="5def3-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5def3-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5def3-117">JSON Representation</span></span>
<span data-ttu-id="5def3-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5def3-118">Here is a JSON representation of the resource.</span></span>
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





