---
title: Тип ресурса variableManagementConditionExpression
description: Оценивает условие состояние управления как логическое выражение.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5d0805f7c698f90cbcb10bfffdce9c95ce6705b2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890155"
---
# <a name="variablemanagementconditionexpression-resource-type"></a><span data-ttu-id="65266-103">Тип ресурса variableManagementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="65266-103">variableManagementConditionExpression resource type</span></span>

> <span data-ttu-id="65266-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="65266-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="65266-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65266-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="65266-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="65266-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="65266-107">Оценивает условие состояние управления как логическое выражение.</span><span class="sxs-lookup"><span data-stu-id="65266-107">Evaluates the management condition state as a Boolean expression.</span></span>

<span data-ttu-id="65266-108">Наследуется от [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="65266-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="65266-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="65266-109">Properties</span></span>
|<span data-ttu-id="65266-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="65266-110">Property</span></span>|<span data-ttu-id="65266-111">Тип</span><span class="sxs-lookup"><span data-stu-id="65266-111">Type</span></span>|<span data-ttu-id="65266-112">Описание</span><span class="sxs-lookup"><span data-stu-id="65266-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65266-113">managementConditionId</span><span class="sxs-lookup"><span data-stu-id="65266-113">managementConditionId</span></span>|<span data-ttu-id="65266-114">Строка</span><span class="sxs-lookup"><span data-stu-id="65266-114">String</span></span>|<span data-ttu-id="65266-115">Идентификатор условия управления, которая используется для оценки выражения.</span><span class="sxs-lookup"><span data-stu-id="65266-115">The management condition id that is used to evaluate the expression.</span></span>|

## <a name="relationships"></a><span data-ttu-id="65266-116">Связи</span><span class="sxs-lookup"><span data-stu-id="65266-116">Relationships</span></span>
<span data-ttu-id="65266-117">Нет</span><span class="sxs-lookup"><span data-stu-id="65266-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="65266-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="65266-118">JSON Representation</span></span>
<span data-ttu-id="65266-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="65266-119">Here is a JSON representation of the resource.</span></span>
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





