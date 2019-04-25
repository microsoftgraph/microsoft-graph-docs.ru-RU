---
title: Тип ресурса Вариаблеманажементкондитионекспрессион
description: Оценивает состояние условия управления как логическое выражение.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 548c0ffd27f76dacf5f88d9e783ce793e64cc434
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32552891"
---
# <a name="variablemanagementconditionexpression-resource-type"></a><span data-ttu-id="be8b1-103">Тип ресурса Вариаблеманажементкондитионекспрессион</span><span class="sxs-lookup"><span data-stu-id="be8b1-103">variableManagementConditionExpression resource type</span></span>

> <span data-ttu-id="be8b1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be8b1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="be8b1-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="be8b1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be8b1-106">Оценивает состояние условия управления как логическое выражение.</span><span class="sxs-lookup"><span data-stu-id="be8b1-106">Evaluates the management condition state as a Boolean expression.</span></span>


<span data-ttu-id="be8b1-107">НаСледуется от [манажементкондитионекспрессионмодел](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="be8b1-107">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="be8b1-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="be8b1-108">Properties</span></span>
|<span data-ttu-id="be8b1-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="be8b1-109">Property</span></span>|<span data-ttu-id="be8b1-110">Тип</span><span class="sxs-lookup"><span data-stu-id="be8b1-110">Type</span></span>|<span data-ttu-id="be8b1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="be8b1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be8b1-112">Манажементкондитионид</span><span class="sxs-lookup"><span data-stu-id="be8b1-112">managementConditionId</span></span>|<span data-ttu-id="be8b1-113">String</span><span class="sxs-lookup"><span data-stu-id="be8b1-113">String</span></span>|<span data-ttu-id="be8b1-114">Идентификатор условия управления, используемый для оценки выражения.</span><span class="sxs-lookup"><span data-stu-id="be8b1-114">The management condition id that is used to evaluate the expression.</span></span>|

## <a name="relationships"></a><span data-ttu-id="be8b1-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="be8b1-115">Relationships</span></span>
<span data-ttu-id="be8b1-116">Нет</span><span class="sxs-lookup"><span data-stu-id="be8b1-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="be8b1-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="be8b1-117">JSON Representation</span></span>
<span data-ttu-id="be8b1-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="be8b1-118">Here is a JSON representation of the resource.</span></span>
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





