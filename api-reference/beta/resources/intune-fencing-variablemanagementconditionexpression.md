---
title: Тип ресурса variableManagementConditionExpression
description: Оценивает условие состояние управления как логическое выражение.
ms.openlocfilehash: 220cb54680755461edb9dab6edf076f8ae0c6a68
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079144"
---
# <a name="variablemanagementconditionexpression-resource-type"></a><span data-ttu-id="0c3a8-103">Тип ресурса variableManagementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="0c3a8-103">variableManagementConditionExpression resource type</span></span>

> <span data-ttu-id="0c3a8-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0c3a8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0c3a8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c3a8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0c3a8-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0c3a8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0c3a8-107">Оценивает условие состояние управления как логическое выражение.</span><span class="sxs-lookup"><span data-stu-id="0c3a8-107">Evaluates the management condition state as a Boolean expression.</span></span>

<span data-ttu-id="0c3a8-108">Наследуется от [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="0c3a8-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0c3a8-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="0c3a8-109">Properties</span></span>
|<span data-ttu-id="0c3a8-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="0c3a8-110">Property</span></span>|<span data-ttu-id="0c3a8-111">Тип</span><span class="sxs-lookup"><span data-stu-id="0c3a8-111">Type</span></span>|<span data-ttu-id="0c3a8-112">Description</span><span class="sxs-lookup"><span data-stu-id="0c3a8-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c3a8-113">managementConditionId</span><span class="sxs-lookup"><span data-stu-id="0c3a8-113">managementConditionId</span></span>|<span data-ttu-id="0c3a8-114">String</span><span class="sxs-lookup"><span data-stu-id="0c3a8-114">String</span></span>|<span data-ttu-id="0c3a8-115">Идентификатор условия управления, которая используется для оценки выражения.</span><span class="sxs-lookup"><span data-stu-id="0c3a8-115">The management condition id that is used to evaluate the expression.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c3a8-116">Связи</span><span class="sxs-lookup"><span data-stu-id="0c3a8-116">Relationships</span></span>
<span data-ttu-id="0c3a8-117">Нет</span><span class="sxs-lookup"><span data-stu-id="0c3a8-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0c3a8-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0c3a8-118">JSON Representation</span></span>
<span data-ttu-id="0c3a8-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0c3a8-119">Here is a JSON representation of the resource.</span></span>
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





