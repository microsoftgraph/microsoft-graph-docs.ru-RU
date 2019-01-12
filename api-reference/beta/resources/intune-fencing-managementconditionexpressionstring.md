---
title: Тип ресурса managementConditionExpressionString
description: Строковое выражение условия управления является представлением строковое выражение условия управления.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 872282914dc57be4e8e9bc7d476e7767907ec913
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968850"
---
# <a name="managementconditionexpressionstring-resource-type"></a><span data-ttu-id="4d9c6-103">Тип ресурса managementConditionExpressionString</span><span class="sxs-lookup"><span data-stu-id="4d9c6-103">managementConditionExpressionString resource type</span></span>

> <span data-ttu-id="4d9c6-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4d9c6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4d9c6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d9c6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4d9c6-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4d9c6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4d9c6-107">Строковое выражение условия управления является представлением строковое выражение условия управления.</span><span class="sxs-lookup"><span data-stu-id="4d9c6-107">A management condition expression string is a string representation of a management condition expression.</span></span>

<span data-ttu-id="4d9c6-108">Наследуется от [managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)</span><span class="sxs-lookup"><span data-stu-id="4d9c6-108">Inherits from [managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4d9c6-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="4d9c6-109">Properties</span></span>
|<span data-ttu-id="4d9c6-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="4d9c6-110">Property</span></span>|<span data-ttu-id="4d9c6-111">Тип</span><span class="sxs-lookup"><span data-stu-id="4d9c6-111">Type</span></span>|<span data-ttu-id="4d9c6-112">Описание</span><span class="sxs-lookup"><span data-stu-id="4d9c6-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d9c6-113">value</span><span class="sxs-lookup"><span data-stu-id="4d9c6-113">value</span></span>|<span data-ttu-id="4d9c6-114">Строка</span><span class="sxs-lookup"><span data-stu-id="4d9c6-114">String</span></span>|<span data-ttu-id="4d9c6-115">Управление условие оператора выражения строковое значение.</span><span class="sxs-lookup"><span data-stu-id="4d9c6-115">The management condition statement expression string value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4d9c6-116">Связи</span><span class="sxs-lookup"><span data-stu-id="4d9c6-116">Relationships</span></span>
<span data-ttu-id="4d9c6-117">Нет</span><span class="sxs-lookup"><span data-stu-id="4d9c6-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4d9c6-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4d9c6-118">JSON Representation</span></span>
<span data-ttu-id="4d9c6-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4d9c6-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managementConditionExpressionString"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementConditionExpressionString",
  "value": "String"
}
```





