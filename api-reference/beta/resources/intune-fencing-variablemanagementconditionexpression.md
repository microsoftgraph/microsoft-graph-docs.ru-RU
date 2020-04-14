---
title: Тип ресурса Вариаблеманажементкондитионекспрессион
description: Оценивает состояние условия управления как логическое выражение.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0195c897c125d7152c346155e63f7bf120883cd4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43458485"
---
# <a name="variablemanagementconditionexpression-resource-type"></a><span data-ttu-id="dbc63-103">Тип ресурса Вариаблеманажементкондитионекспрессион</span><span class="sxs-lookup"><span data-stu-id="dbc63-103">variableManagementConditionExpression resource type</span></span>

<span data-ttu-id="dbc63-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dbc63-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dbc63-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dbc63-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dbc63-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dbc63-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dbc63-107">Оценивает состояние условия управления как логическое выражение.</span><span class="sxs-lookup"><span data-stu-id="dbc63-107">Evaluates the management condition state as a Boolean expression.</span></span>


<span data-ttu-id="dbc63-108">Наследуется от [манажементкондитионекспрессионмодел](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="dbc63-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="dbc63-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="dbc63-109">Properties</span></span>
|<span data-ttu-id="dbc63-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="dbc63-110">Property</span></span>|<span data-ttu-id="dbc63-111">Тип</span><span class="sxs-lookup"><span data-stu-id="dbc63-111">Type</span></span>|<span data-ttu-id="dbc63-112">Описание</span><span class="sxs-lookup"><span data-stu-id="dbc63-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dbc63-113">манажементкондитионид</span><span class="sxs-lookup"><span data-stu-id="dbc63-113">managementConditionId</span></span>|<span data-ttu-id="dbc63-114">String</span><span class="sxs-lookup"><span data-stu-id="dbc63-114">String</span></span>|<span data-ttu-id="dbc63-115">Идентификатор условия управления, используемый для оценки выражения.</span><span class="sxs-lookup"><span data-stu-id="dbc63-115">The management condition id that is used to evaluate the expression.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dbc63-116">Связи</span><span class="sxs-lookup"><span data-stu-id="dbc63-116">Relationships</span></span>
<span data-ttu-id="dbc63-117">Нет</span><span class="sxs-lookup"><span data-stu-id="dbc63-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dbc63-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dbc63-118">JSON Representation</span></span>
<span data-ttu-id="dbc63-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dbc63-119">Here is a JSON representation of the resource.</span></span>
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



