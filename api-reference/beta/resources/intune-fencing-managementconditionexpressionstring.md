---
title: Тип ресурса managementConditionExpressionString
description: Строковое выражение условия управления является представлением строковое выражение условия управления.
author: tfitzmac
ms.openlocfilehash: eabcc730e86f74e2afc7c93874d47e787579c899
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361042"
---
# <a name="managementconditionexpressionstring-resource-type"></a><span data-ttu-id="59f86-103">Тип ресурса managementConditionExpressionString</span><span class="sxs-lookup"><span data-stu-id="59f86-103">managementConditionExpressionString resource type</span></span>

> <span data-ttu-id="59f86-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="59f86-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="59f86-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59f86-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="59f86-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="59f86-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="59f86-107">Строковое выражение условия управления является представлением строковое выражение условия управления.</span><span class="sxs-lookup"><span data-stu-id="59f86-107">A management condition expression string is a string representation of a management condition expression.</span></span>

<span data-ttu-id="59f86-108">Наследуется от [managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)</span><span class="sxs-lookup"><span data-stu-id="59f86-108">Inherits from [managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)</span></span>

## <a name="properties"></a><span data-ttu-id="59f86-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="59f86-109">Properties</span></span>
|<span data-ttu-id="59f86-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="59f86-110">Property</span></span>|<span data-ttu-id="59f86-111">Тип</span><span class="sxs-lookup"><span data-stu-id="59f86-111">Type</span></span>|<span data-ttu-id="59f86-112">Описание</span><span class="sxs-lookup"><span data-stu-id="59f86-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59f86-113">value</span><span class="sxs-lookup"><span data-stu-id="59f86-113">value</span></span>|<span data-ttu-id="59f86-114">Строка</span><span class="sxs-lookup"><span data-stu-id="59f86-114">String</span></span>|<span data-ttu-id="59f86-115">Управление условие оператора выражения строковое значение.</span><span class="sxs-lookup"><span data-stu-id="59f86-115">The management condition statement expression string value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="59f86-116">Связи</span><span class="sxs-lookup"><span data-stu-id="59f86-116">Relationships</span></span>
<span data-ttu-id="59f86-117">Нет</span><span class="sxs-lookup"><span data-stu-id="59f86-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="59f86-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="59f86-118">JSON Representation</span></span>
<span data-ttu-id="59f86-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="59f86-119">Here is a JSON representation of the resource.</span></span>
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





