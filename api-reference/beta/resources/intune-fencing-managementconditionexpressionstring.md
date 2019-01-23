---
title: Тип ресурса managementConditionExpressionString
description: Строковое выражение условия управления является представлением строковое выражение условия управления.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8b8abc3492690afe6709070decbfe050356fd614
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419193"
---
# <a name="managementconditionexpressionstring-resource-type"></a><span data-ttu-id="1abc5-103">Тип ресурса managementConditionExpressionString</span><span class="sxs-lookup"><span data-stu-id="1abc5-103">managementConditionExpressionString resource type</span></span>

> <span data-ttu-id="1abc5-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1abc5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1abc5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1abc5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1abc5-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1abc5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1abc5-107">Строковое выражение условия управления является представлением строковое выражение условия управления.</span><span class="sxs-lookup"><span data-stu-id="1abc5-107">A management condition expression string is a string representation of a management condition expression.</span></span>


<span data-ttu-id="1abc5-108">Наследуется от [managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)</span><span class="sxs-lookup"><span data-stu-id="1abc5-108">Inherits from [managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1abc5-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="1abc5-109">Properties</span></span>
|<span data-ttu-id="1abc5-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="1abc5-110">Property</span></span>|<span data-ttu-id="1abc5-111">Тип</span><span class="sxs-lookup"><span data-stu-id="1abc5-111">Type</span></span>|<span data-ttu-id="1abc5-112">Описание</span><span class="sxs-lookup"><span data-stu-id="1abc5-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1abc5-113">value</span><span class="sxs-lookup"><span data-stu-id="1abc5-113">value</span></span>|<span data-ttu-id="1abc5-114">String</span><span class="sxs-lookup"><span data-stu-id="1abc5-114">String</span></span>|<span data-ttu-id="1abc5-115">Управление условие оператора выражения строковое значение.</span><span class="sxs-lookup"><span data-stu-id="1abc5-115">The management condition statement expression string value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1abc5-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="1abc5-116">Relationships</span></span>
<span data-ttu-id="1abc5-117">Нет</span><span class="sxs-lookup"><span data-stu-id="1abc5-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1abc5-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1abc5-118">JSON Representation</span></span>
<span data-ttu-id="1abc5-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1abc5-119">Here is a JSON representation of the resource.</span></span>
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




