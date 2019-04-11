---
title: Тип ресурса Вариаблеманажементкондитионекспрессион
description: Оценивает состояние условия управления как логическое выражение.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 548c0ffd27f76dacf5f88d9e783ce793e64cc434
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31802760"
---
# <a name="variablemanagementconditionexpression-resource-type"></a><span data-ttu-id="4cf5f-103">Тип ресурса Вариаблеманажементкондитионекспрессион</span><span class="sxs-lookup"><span data-stu-id="4cf5f-103">variableManagementConditionExpression resource type</span></span>

> <span data-ttu-id="4cf5f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4cf5f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4cf5f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4cf5f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4cf5f-106">Оценивает состояние условия управления как логическое выражение.</span><span class="sxs-lookup"><span data-stu-id="4cf5f-106">Evaluates the management condition state as a Boolean expression.</span></span>


<span data-ttu-id="4cf5f-107">НаСледуется от [манажементкондитионекспрессионмодел](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="4cf5f-107">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4cf5f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="4cf5f-108">Properties</span></span>
|<span data-ttu-id="4cf5f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="4cf5f-109">Property</span></span>|<span data-ttu-id="4cf5f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="4cf5f-110">Type</span></span>|<span data-ttu-id="4cf5f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4cf5f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4cf5f-112">Манажементкондитионид</span><span class="sxs-lookup"><span data-stu-id="4cf5f-112">managementConditionId</span></span>|<span data-ttu-id="4cf5f-113">String</span><span class="sxs-lookup"><span data-stu-id="4cf5f-113">String</span></span>|<span data-ttu-id="4cf5f-114">Идентификатор условия управления, используемый для оценки выражения.</span><span class="sxs-lookup"><span data-stu-id="4cf5f-114">The management condition id that is used to evaluate the expression.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4cf5f-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="4cf5f-115">Relationships</span></span>
<span data-ttu-id="4cf5f-116">Нет</span><span class="sxs-lookup"><span data-stu-id="4cf5f-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4cf5f-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4cf5f-117">JSON Representation</span></span>
<span data-ttu-id="4cf5f-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4cf5f-118">Here is a JSON representation of the resource.</span></span>
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





