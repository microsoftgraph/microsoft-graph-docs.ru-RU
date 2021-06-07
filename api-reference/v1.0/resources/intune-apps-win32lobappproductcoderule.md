---
title: тип ресурса win32LobAppProductCodeRule
description: Сложный тип для хранения данных правил кода продукта и версии для приложения LOB Win32. Это правило не поддерживается в качестве правила требования.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fb77116ce3498023e011d83c6214c3050eaf1124
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52743002"
---
# <a name="win32lobappproductcoderule-resource-type"></a><span data-ttu-id="73a65-104">тип ресурса win32LobAppProductCodeRule</span><span class="sxs-lookup"><span data-stu-id="73a65-104">win32LobAppProductCodeRule resource type</span></span>

<span data-ttu-id="73a65-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73a65-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="73a65-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="73a65-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73a65-107">Сложный тип для хранения данных правил кода продукта и версии для приложения LOB Win32.</span><span class="sxs-lookup"><span data-stu-id="73a65-107">A complex type to store the product code and version rule data for a Win32 LOB app.</span></span> <span data-ttu-id="73a65-108">Это правило не поддерживается в качестве правила требования.</span><span class="sxs-lookup"><span data-stu-id="73a65-108">This rule is not supported as a requirement rule.</span></span>


<span data-ttu-id="73a65-109">Наследует [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="73a65-109">Inherits from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="73a65-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="73a65-110">Properties</span></span>
|<span data-ttu-id="73a65-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="73a65-111">Property</span></span>|<span data-ttu-id="73a65-112">Тип</span><span class="sxs-lookup"><span data-stu-id="73a65-112">Type</span></span>|<span data-ttu-id="73a65-113">Описание</span><span class="sxs-lookup"><span data-stu-id="73a65-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73a65-114">ruleType</span><span class="sxs-lookup"><span data-stu-id="73a65-114">ruleType</span></span>|[<span data-ttu-id="73a65-115">win32LobAppRuleType</span><span class="sxs-lookup"><span data-stu-id="73a65-115">win32LobAppRuleType</span></span>](../resources/intune-apps-win32lobappruletype.md)|<span data-ttu-id="73a65-116">Тип правила, указывающий цель правила.</span><span class="sxs-lookup"><span data-stu-id="73a65-116">The rule type indicating the purpose of the rule.</span></span> <span data-ttu-id="73a65-117">Унаследованный от [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span><span class="sxs-lookup"><span data-stu-id="73a65-117">Inherited from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span></span> <span data-ttu-id="73a65-118">Возможные значения: `detection`, `requirement`.</span><span class="sxs-lookup"><span data-stu-id="73a65-118">Possible values are: `detection`, `requirement`.</span></span>|
|<span data-ttu-id="73a65-119">productCode</span><span class="sxs-lookup"><span data-stu-id="73a65-119">productCode</span></span>|<span data-ttu-id="73a65-120">String</span><span class="sxs-lookup"><span data-stu-id="73a65-120">String</span></span>|<span data-ttu-id="73a65-121">Код продукта приложения.</span><span class="sxs-lookup"><span data-stu-id="73a65-121">The product code of the app.</span></span>|
|<span data-ttu-id="73a65-122">productVersionOperator</span><span class="sxs-lookup"><span data-stu-id="73a65-122">productVersionOperator</span></span>|[<span data-ttu-id="73a65-123">win32LobAppRuleOperator</span><span class="sxs-lookup"><span data-stu-id="73a65-123">win32LobAppRuleOperator</span></span>](../resources/intune-apps-win32lobappruleoperator.md)|<span data-ttu-id="73a65-124">Оператор сравнения версий продукта.</span><span class="sxs-lookup"><span data-stu-id="73a65-124">The product version comparison operator.</span></span> <span data-ttu-id="73a65-125">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="73a65-125">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="73a65-126">productVersion</span><span class="sxs-lookup"><span data-stu-id="73a65-126">productVersion</span></span>|<span data-ttu-id="73a65-127">String</span><span class="sxs-lookup"><span data-stu-id="73a65-127">String</span></span>|<span data-ttu-id="73a65-128">Значение сравнения версии продукта.</span><span class="sxs-lookup"><span data-stu-id="73a65-128">The product version comparison value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="73a65-129">Отношения</span><span class="sxs-lookup"><span data-stu-id="73a65-129">Relationships</span></span>
<span data-ttu-id="73a65-130">Нет</span><span class="sxs-lookup"><span data-stu-id="73a65-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="73a65-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="73a65-131">JSON Representation</span></span>
<span data-ttu-id="73a65-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="73a65-132">Here is a JSON representation of the resource.</span></span>
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




