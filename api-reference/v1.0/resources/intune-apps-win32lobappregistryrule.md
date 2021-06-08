---
title: тип ресурса win32LobAppRegistryRule
description: Сложный тип для хранения данных правил реестра для приложения LOB Win32.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bfa6ed9e95a86abe1d87646a7c57f953be539f69
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758983"
---
# <a name="win32lobappregistryrule-resource-type"></a><span data-ttu-id="19ab3-103">тип ресурса win32LobAppRegistryRule</span><span class="sxs-lookup"><span data-stu-id="19ab3-103">win32LobAppRegistryRule resource type</span></span>

<span data-ttu-id="19ab3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19ab3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="19ab3-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="19ab3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19ab3-106">Сложный тип для хранения данных правил реестра для приложения LOB Win32.</span><span class="sxs-lookup"><span data-stu-id="19ab3-106">A complex type to store registry rule data for a Win32 LOB app.</span></span>


<span data-ttu-id="19ab3-107">Наследует [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="19ab3-107">Inherits from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="19ab3-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="19ab3-108">Properties</span></span>
|<span data-ttu-id="19ab3-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="19ab3-109">Property</span></span>|<span data-ttu-id="19ab3-110">Тип</span><span class="sxs-lookup"><span data-stu-id="19ab3-110">Type</span></span>|<span data-ttu-id="19ab3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="19ab3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19ab3-112">ruleType</span><span class="sxs-lookup"><span data-stu-id="19ab3-112">ruleType</span></span>|[<span data-ttu-id="19ab3-113">win32LobAppRuleType</span><span class="sxs-lookup"><span data-stu-id="19ab3-113">win32LobAppRuleType</span></span>](../resources/intune-apps-win32lobappruletype.md)|<span data-ttu-id="19ab3-114">Тип правила, указывающий цель правила.</span><span class="sxs-lookup"><span data-stu-id="19ab3-114">The rule type indicating the purpose of the rule.</span></span> <span data-ttu-id="19ab3-115">Унаследованный от [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span><span class="sxs-lookup"><span data-stu-id="19ab3-115">Inherited from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span></span> <span data-ttu-id="19ab3-116">Возможные значения: `detection`, `requirement`.</span><span class="sxs-lookup"><span data-stu-id="19ab3-116">Possible values are: `detection`, `requirement`.</span></span>|
|<span data-ttu-id="19ab3-117">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="19ab3-117">check32BitOn64System</span></span>|<span data-ttu-id="19ab3-118">Логический</span><span class="sxs-lookup"><span data-stu-id="19ab3-118">Boolean</span></span>|<span data-ttu-id="19ab3-119">Значение, указывающее, следует ли искать 32-битный реестр в 64-битных системах.</span><span class="sxs-lookup"><span data-stu-id="19ab3-119">A value indicating whether to search the 32-bit registry on 64-bit systems.</span></span>|
|<span data-ttu-id="19ab3-120">keyPath</span><span class="sxs-lookup"><span data-stu-id="19ab3-120">keyPath</span></span>|<span data-ttu-id="19ab3-121">String</span><span class="sxs-lookup"><span data-stu-id="19ab3-121">String</span></span>|<span data-ttu-id="19ab3-122">Полный путь записи реестра, содержащей значение для обнаружения.</span><span class="sxs-lookup"><span data-stu-id="19ab3-122">The full path of the registry entry containing the value to detect.</span></span>|
|<span data-ttu-id="19ab3-123">valueName</span><span class="sxs-lookup"><span data-stu-id="19ab3-123">valueName</span></span>|<span data-ttu-id="19ab3-124">String</span><span class="sxs-lookup"><span data-stu-id="19ab3-124">String</span></span>|<span data-ttu-id="19ab3-125">Имя значения реестра для обнаружения.</span><span class="sxs-lookup"><span data-stu-id="19ab3-125">The name of the registry value to detect.</span></span>|
|<span data-ttu-id="19ab3-126">operationType</span><span class="sxs-lookup"><span data-stu-id="19ab3-126">operationType</span></span>|[<span data-ttu-id="19ab3-127">win32LobAppRegistryRuleOperationType</span><span class="sxs-lookup"><span data-stu-id="19ab3-127">win32LobAppRegistryRuleOperationType</span></span>](../resources/intune-apps-win32lobappregistryruleoperationtype.md)|<span data-ttu-id="19ab3-128">Тип операции реестра.</span><span class="sxs-lookup"><span data-stu-id="19ab3-128">The registry operation type.</span></span> <span data-ttu-id="19ab3-129">Возможные значения: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span><span class="sxs-lookup"><span data-stu-id="19ab3-129">Possible values are: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span></span>|
|<span data-ttu-id="19ab3-130">operator</span><span class="sxs-lookup"><span data-stu-id="19ab3-130">operator</span></span>|[<span data-ttu-id="19ab3-131">win32LobAppRuleOperator</span><span class="sxs-lookup"><span data-stu-id="19ab3-131">win32LobAppRuleOperator</span></span>](../resources/intune-apps-win32lobappruleoperator.md)|<span data-ttu-id="19ab3-132">Оператор обнаружения реестра.</span><span class="sxs-lookup"><span data-stu-id="19ab3-132">The operator for registry detection.</span></span> <span data-ttu-id="19ab3-133">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="19ab3-133">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="19ab3-134">comparisonValue</span><span class="sxs-lookup"><span data-stu-id="19ab3-134">comparisonValue</span></span>|<span data-ttu-id="19ab3-135">String</span><span class="sxs-lookup"><span data-stu-id="19ab3-135">String</span></span>|<span data-ttu-id="19ab3-136">Значение сравнения реестра.</span><span class="sxs-lookup"><span data-stu-id="19ab3-136">The registry comparison value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="19ab3-137">Связи</span><span class="sxs-lookup"><span data-stu-id="19ab3-137">Relationships</span></span>
<span data-ttu-id="19ab3-138">Нет</span><span class="sxs-lookup"><span data-stu-id="19ab3-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="19ab3-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="19ab3-139">JSON Representation</span></span>
<span data-ttu-id="19ab3-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="19ab3-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppRegistryRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppRegistryRule",
  "ruleType": "String",
  "check32BitOn64System": true,
  "keyPath": "String",
  "valueName": "String",
  "operationType": "String",
  "operator": "String",
  "comparisonValue": "String"
}
```




