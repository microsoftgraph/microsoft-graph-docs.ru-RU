---
title: Тип ресурса Вариаблеманажементкондитионекспрессион
description: Оценивает состояние условия управления как логическое выражение.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8be06947bfce0e032965d3704ab9eec3a401845f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49298759"
---
# <a name="variablemanagementconditionexpression-resource-type"></a><span data-ttu-id="cf8b4-103">Тип ресурса Вариаблеманажементкондитионекспрессион</span><span class="sxs-lookup"><span data-stu-id="cf8b4-103">variableManagementConditionExpression resource type</span></span>

<span data-ttu-id="cf8b4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf8b4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cf8b4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf8b4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cf8b4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cf8b4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf8b4-107">Оценивает состояние условия управления как логическое выражение.</span><span class="sxs-lookup"><span data-stu-id="cf8b4-107">Evaluates the management condition state as a Boolean expression.</span></span>


<span data-ttu-id="cf8b4-108">Наследуется от [манажементкондитионекспрессионмодел](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="cf8b4-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="cf8b4-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="cf8b4-109">Properties</span></span>
|<span data-ttu-id="cf8b4-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="cf8b4-110">Property</span></span>|<span data-ttu-id="cf8b4-111">Тип</span><span class="sxs-lookup"><span data-stu-id="cf8b4-111">Type</span></span>|<span data-ttu-id="cf8b4-112">Описание</span><span class="sxs-lookup"><span data-stu-id="cf8b4-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf8b4-113">манажементкондитионид</span><span class="sxs-lookup"><span data-stu-id="cf8b4-113">managementConditionId</span></span>|<span data-ttu-id="cf8b4-114">String</span><span class="sxs-lookup"><span data-stu-id="cf8b4-114">String</span></span>|<span data-ttu-id="cf8b4-115">Идентификатор условия управления, используемый для оценки выражения.</span><span class="sxs-lookup"><span data-stu-id="cf8b4-115">The management condition id that is used to evaluate the expression.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cf8b4-116">Связи</span><span class="sxs-lookup"><span data-stu-id="cf8b4-116">Relationships</span></span>
<span data-ttu-id="cf8b4-117">Нет</span><span class="sxs-lookup"><span data-stu-id="cf8b4-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cf8b4-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cf8b4-118">JSON Representation</span></span>
<span data-ttu-id="cf8b4-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cf8b4-119">Here is a JSON representation of the resource.</span></span>
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




