---
title: Тип ресурса Вариаблеманажементкондитионекспрессион
description: Оценивает состояние условия управления как логическое выражение.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 21b2d7e9af445ac7d439b7d0dd6a37517aeeaf2a
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941221"
---
# <a name="variablemanagementconditionexpression-resource-type"></a><span data-ttu-id="0b440-103">Тип ресурса Вариаблеманажементкондитионекспрессион</span><span class="sxs-lookup"><span data-stu-id="0b440-103">variableManagementConditionExpression resource type</span></span>

> <span data-ttu-id="0b440-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b440-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0b440-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0b440-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b440-106">Оценивает состояние условия управления как логическое выражение.</span><span class="sxs-lookup"><span data-stu-id="0b440-106">Evaluates the management condition state as a Boolean expression.</span></span>


<span data-ttu-id="0b440-107">Наследуется от [манажементкондитионекспрессионмодел](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="0b440-107">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0b440-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0b440-108">Properties</span></span>
|<span data-ttu-id="0b440-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0b440-109">Property</span></span>|<span data-ttu-id="0b440-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0b440-110">Type</span></span>|<span data-ttu-id="0b440-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0b440-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b440-112">Манажементкондитионид</span><span class="sxs-lookup"><span data-stu-id="0b440-112">managementConditionId</span></span>|<span data-ttu-id="0b440-113">Строка</span><span class="sxs-lookup"><span data-stu-id="0b440-113">String</span></span>|<span data-ttu-id="0b440-114">Идентификатор условия управления, используемый для оценки выражения.</span><span class="sxs-lookup"><span data-stu-id="0b440-114">The management condition id that is used to evaluate the expression.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0b440-115">Связи</span><span class="sxs-lookup"><span data-stu-id="0b440-115">Relationships</span></span>
<span data-ttu-id="0b440-116">Нет</span><span class="sxs-lookup"><span data-stu-id="0b440-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0b440-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0b440-117">JSON Representation</span></span>
<span data-ttu-id="0b440-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0b440-118">Here is a JSON representation of the resource.</span></span>
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




