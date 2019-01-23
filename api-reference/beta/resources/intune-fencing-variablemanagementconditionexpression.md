---
title: Тип ресурса variableManagementConditionExpression
description: Оценивает условие состояние управления как логическое выражение.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f6a5e7efd0c8213f40d1dfb5f86d2f86c999069d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399628"
---
# <a name="variablemanagementconditionexpression-resource-type"></a><span data-ttu-id="416b8-103">Тип ресурса variableManagementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="416b8-103">variableManagementConditionExpression resource type</span></span>

> <span data-ttu-id="416b8-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="416b8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="416b8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="416b8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="416b8-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="416b8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="416b8-107">Оценивает условие состояние управления как логическое выражение.</span><span class="sxs-lookup"><span data-stu-id="416b8-107">Evaluates the management condition state as a Boolean expression.</span></span>


<span data-ttu-id="416b8-108">Наследуется от [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="416b8-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="416b8-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="416b8-109">Properties</span></span>
|<span data-ttu-id="416b8-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="416b8-110">Property</span></span>|<span data-ttu-id="416b8-111">Тип</span><span class="sxs-lookup"><span data-stu-id="416b8-111">Type</span></span>|<span data-ttu-id="416b8-112">Описание</span><span class="sxs-lookup"><span data-stu-id="416b8-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="416b8-113">managementConditionId</span><span class="sxs-lookup"><span data-stu-id="416b8-113">managementConditionId</span></span>|<span data-ttu-id="416b8-114">String</span><span class="sxs-lookup"><span data-stu-id="416b8-114">String</span></span>|<span data-ttu-id="416b8-115">Идентификатор условия управления, которая используется для оценки выражения.</span><span class="sxs-lookup"><span data-stu-id="416b8-115">The management condition id that is used to evaluate the expression.</span></span>|

## <a name="relationships"></a><span data-ttu-id="416b8-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="416b8-116">Relationships</span></span>
<span data-ttu-id="416b8-117">Нет</span><span class="sxs-lookup"><span data-stu-id="416b8-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="416b8-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="416b8-118">JSON Representation</span></span>
<span data-ttu-id="416b8-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="416b8-119">Here is a JSON representation of the resource.</span></span>
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




