---
title: Тип ресурса Манажементкондитионекспрессионстринг
description: Строка выражения условия управления — это строковое представление выражения условия управления.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fc4552ab6cc97676ced32ae7e7f5649262c4f4f7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151011"
---
# <a name="managementconditionexpressionstring-resource-type"></a><span data-ttu-id="13c2a-103">Тип ресурса Манажементкондитионекспрессионстринг</span><span class="sxs-lookup"><span data-stu-id="13c2a-103">managementConditionExpressionString resource type</span></span>

> <span data-ttu-id="13c2a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13c2a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13c2a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="13c2a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13c2a-106">Строка выражения условия управления — это строковое представление выражения условия управления.</span><span class="sxs-lookup"><span data-stu-id="13c2a-106">A management condition expression string is a string representation of a management condition expression.</span></span>


<span data-ttu-id="13c2a-107">НаСледуется от [манажементкондитионекспрессион](../resources/intune-fencing-managementconditionexpression.md)</span><span class="sxs-lookup"><span data-stu-id="13c2a-107">Inherits from [managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)</span></span>

## <a name="properties"></a><span data-ttu-id="13c2a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="13c2a-108">Properties</span></span>
|<span data-ttu-id="13c2a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="13c2a-109">Property</span></span>|<span data-ttu-id="13c2a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="13c2a-110">Type</span></span>|<span data-ttu-id="13c2a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="13c2a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13c2a-112">value</span><span class="sxs-lookup"><span data-stu-id="13c2a-112">value</span></span>|<span data-ttu-id="13c2a-113">String</span><span class="sxs-lookup"><span data-stu-id="13c2a-113">String</span></span>|<span data-ttu-id="13c2a-114">Строковое значение выражения оператора условия управления.</span><span class="sxs-lookup"><span data-stu-id="13c2a-114">The management condition statement expression string value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="13c2a-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="13c2a-115">Relationships</span></span>
<span data-ttu-id="13c2a-116">Нет</span><span class="sxs-lookup"><span data-stu-id="13c2a-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="13c2a-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="13c2a-117">JSON Representation</span></span>
<span data-ttu-id="13c2a-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="13c2a-118">Here is a JSON representation of the resource.</span></span>
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




