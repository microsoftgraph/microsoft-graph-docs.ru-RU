---
title: Тип ресурса win32LobAppProductCodeRule
description: Сложный тип для хранения кода продукта и данных правила версий для бизнес-приложения Win32. Это правило не поддерживается в качестве правила для требования.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bd3dde2386c76b5ed7dee6174789667d44839c58
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44790819"
---
# <a name="win32lobappproductcoderule-resource-type"></a><span data-ttu-id="14665-104">Тип ресурса win32LobAppProductCodeRule</span><span class="sxs-lookup"><span data-stu-id="14665-104">win32LobAppProductCodeRule resource type</span></span>

<span data-ttu-id="14665-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14665-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="14665-106">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14665-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14665-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="14665-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14665-108">Сложный тип для хранения кода продукта и данных правила версий для бизнес-приложения Win32.</span><span class="sxs-lookup"><span data-stu-id="14665-108">A complex type to store the product code and version rule data for a Win32 LOB app.</span></span> <span data-ttu-id="14665-109">Это правило не поддерживается в качестве правила для требования.</span><span class="sxs-lookup"><span data-stu-id="14665-109">This rule is not supported as a requirement rule.</span></span>


<span data-ttu-id="14665-110">Наследуется от [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="14665-110">Inherits from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="14665-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="14665-111">Properties</span></span>
|<span data-ttu-id="14665-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="14665-112">Property</span></span>|<span data-ttu-id="14665-113">Тип</span><span class="sxs-lookup"><span data-stu-id="14665-113">Type</span></span>|<span data-ttu-id="14665-114">Описание</span><span class="sxs-lookup"><span data-stu-id="14665-114">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14665-115">ruleType</span><span class="sxs-lookup"><span data-stu-id="14665-115">ruleType</span></span>|[<span data-ttu-id="14665-116">win32LobAppRuleType</span><span class="sxs-lookup"><span data-stu-id="14665-116">win32LobAppRuleType</span></span>](../resources/intune-apps-win32lobappruletype.md)|<span data-ttu-id="14665-117">Тип правила, указывающий назначение правила.</span><span class="sxs-lookup"><span data-stu-id="14665-117">The rule type indicating the purpose of the rule.</span></span> <span data-ttu-id="14665-118">Наследуется от [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span><span class="sxs-lookup"><span data-stu-id="14665-118">Inherited from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span></span> <span data-ttu-id="14665-119">Возможные значения: `detection`, `requirement`.</span><span class="sxs-lookup"><span data-stu-id="14665-119">Possible values are: `detection`, `requirement`.</span></span>|
|<span data-ttu-id="14665-120">productCode</span><span class="sxs-lookup"><span data-stu-id="14665-120">productCode</span></span>|<span data-ttu-id="14665-121">String</span><span class="sxs-lookup"><span data-stu-id="14665-121">String</span></span>|<span data-ttu-id="14665-122">Код продукта приложения.</span><span class="sxs-lookup"><span data-stu-id="14665-122">The product code of the app.</span></span>|
|<span data-ttu-id="14665-123">продуктверсионоператор</span><span class="sxs-lookup"><span data-stu-id="14665-123">productVersionOperator</span></span>|[<span data-ttu-id="14665-124">win32LobAppRuleOperator</span><span class="sxs-lookup"><span data-stu-id="14665-124">win32LobAppRuleOperator</span></span>](../resources/intune-apps-win32lobappruleoperator.md)|<span data-ttu-id="14665-125">Оператор сравнения версий продукта.</span><span class="sxs-lookup"><span data-stu-id="14665-125">The product version comparison operator.</span></span> <span data-ttu-id="14665-126">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="14665-126">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="14665-127">productVersion</span><span class="sxs-lookup"><span data-stu-id="14665-127">productVersion</span></span>|<span data-ttu-id="14665-128">String</span><span class="sxs-lookup"><span data-stu-id="14665-128">String</span></span>|<span data-ttu-id="14665-129">Значение сравнения версий продукта.</span><span class="sxs-lookup"><span data-stu-id="14665-129">The product version comparison value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="14665-130">Связи</span><span class="sxs-lookup"><span data-stu-id="14665-130">Relationships</span></span>
<span data-ttu-id="14665-131">Нет</span><span class="sxs-lookup"><span data-stu-id="14665-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="14665-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="14665-132">JSON Representation</span></span>
<span data-ttu-id="14665-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="14665-133">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppProductCodeRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppProductCodeRule",
  "ruleType": "String",
  "productCode": "String",
  "productVersionOperator": "String",
  "productVersion": "String"
}
```



