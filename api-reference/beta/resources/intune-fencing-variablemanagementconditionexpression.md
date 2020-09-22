---
title: Тип ресурса Вариаблеманажементкондитионекспрессион
description: Оценивает состояние условия управления как логическое выражение.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2cb61473401d868fb98a9ea041f268252168d5be
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48031244"
---
# <a name="variablemanagementconditionexpression-resource-type"></a><span data-ttu-id="1e897-103">Тип ресурса Вариаблеманажементкондитионекспрессион</span><span class="sxs-lookup"><span data-stu-id="1e897-103">variableManagementConditionExpression resource type</span></span>

<span data-ttu-id="1e897-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e897-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1e897-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e897-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e897-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1e897-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e897-107">Оценивает состояние условия управления как логическое выражение.</span><span class="sxs-lookup"><span data-stu-id="1e897-107">Evaluates the management condition state as a Boolean expression.</span></span>


<span data-ttu-id="1e897-108">Наследуется от [манажементкондитионекспрессионмодел](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="1e897-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1e897-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="1e897-109">Properties</span></span>
|<span data-ttu-id="1e897-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="1e897-110">Property</span></span>|<span data-ttu-id="1e897-111">Тип</span><span class="sxs-lookup"><span data-stu-id="1e897-111">Type</span></span>|<span data-ttu-id="1e897-112">Описание</span><span class="sxs-lookup"><span data-stu-id="1e897-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e897-113">манажементкондитионид</span><span class="sxs-lookup"><span data-stu-id="1e897-113">managementConditionId</span></span>|<span data-ttu-id="1e897-114">String</span><span class="sxs-lookup"><span data-stu-id="1e897-114">String</span></span>|<span data-ttu-id="1e897-115">Идентификатор условия управления, используемый для оценки выражения.</span><span class="sxs-lookup"><span data-stu-id="1e897-115">The management condition id that is used to evaluate the expression.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1e897-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="1e897-116">Relationships</span></span>
<span data-ttu-id="1e897-117">Нет</span><span class="sxs-lookup"><span data-stu-id="1e897-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1e897-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1e897-118">JSON Representation</span></span>
<span data-ttu-id="1e897-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1e897-119">Here is a JSON representation of the resource.</span></span>
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






