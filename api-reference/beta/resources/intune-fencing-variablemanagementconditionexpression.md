---
title: Тип ресурса variableManagementConditionExpression
description: Оценивает условие состояние управления как логическое выражение.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8fc3e49e7ba55cf10a1dac36690d0b1e419890a8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939765"
---
# <a name="variablemanagementconditionexpression-resource-type"></a><span data-ttu-id="032da-103">Тип ресурса variableManagementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="032da-103">variableManagementConditionExpression resource type</span></span>

> <span data-ttu-id="032da-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="032da-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="032da-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="032da-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="032da-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="032da-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="032da-107">Оценивает условие состояние управления как логическое выражение.</span><span class="sxs-lookup"><span data-stu-id="032da-107">Evaluates the management condition state as a Boolean expression.</span></span>

<span data-ttu-id="032da-108">Наследуется от [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="032da-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="032da-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="032da-109">Properties</span></span>
|<span data-ttu-id="032da-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="032da-110">Property</span></span>|<span data-ttu-id="032da-111">Тип</span><span class="sxs-lookup"><span data-stu-id="032da-111">Type</span></span>|<span data-ttu-id="032da-112">Описание</span><span class="sxs-lookup"><span data-stu-id="032da-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="032da-113">managementConditionId</span><span class="sxs-lookup"><span data-stu-id="032da-113">managementConditionId</span></span>|<span data-ttu-id="032da-114">Строка</span><span class="sxs-lookup"><span data-stu-id="032da-114">String</span></span>|<span data-ttu-id="032da-115">Идентификатор условия управления, которая используется для оценки выражения.</span><span class="sxs-lookup"><span data-stu-id="032da-115">The management condition id that is used to evaluate the expression.</span></span>|

## <a name="relationships"></a><span data-ttu-id="032da-116">Связи</span><span class="sxs-lookup"><span data-stu-id="032da-116">Relationships</span></span>
<span data-ttu-id="032da-117">Нет</span><span class="sxs-lookup"><span data-stu-id="032da-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="032da-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="032da-118">JSON Representation</span></span>
<span data-ttu-id="032da-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="032da-119">Here is a JSON representation of the resource.</span></span>
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





