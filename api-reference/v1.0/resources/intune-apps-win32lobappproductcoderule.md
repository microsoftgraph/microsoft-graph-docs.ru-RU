---
title: Тип ресурса win32LobAppProductCodeRule
description: Сложный тип для хранения кода продукта и данных правила версий для бизнес-приложения Win32. Это правило не поддерживается в качестве правила для требования.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 101818fdea0dd87966abdd08d4cfbbffd1a81680
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080124"
---
# <a name="win32lobappproductcoderule-resource-type"></a><span data-ttu-id="d282d-104">Тип ресурса win32LobAppProductCodeRule</span><span class="sxs-lookup"><span data-stu-id="d282d-104">win32LobAppProductCodeRule resource type</span></span>

<span data-ttu-id="d282d-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d282d-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d282d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d282d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d282d-107">Сложный тип для хранения кода продукта и данных правила версий для бизнес-приложения Win32.</span><span class="sxs-lookup"><span data-stu-id="d282d-107">A complex type to store the product code and version rule data for a Win32 LOB app.</span></span> <span data-ttu-id="d282d-108">Это правило не поддерживается в качестве правила для требования.</span><span class="sxs-lookup"><span data-stu-id="d282d-108">This rule is not supported as a requirement rule.</span></span>


<span data-ttu-id="d282d-109">Наследуется от [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="d282d-109">Inherits from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d282d-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="d282d-110">Properties</span></span>
|<span data-ttu-id="d282d-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="d282d-111">Property</span></span>|<span data-ttu-id="d282d-112">Тип</span><span class="sxs-lookup"><span data-stu-id="d282d-112">Type</span></span>|<span data-ttu-id="d282d-113">Описание</span><span class="sxs-lookup"><span data-stu-id="d282d-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d282d-114">ruleType</span><span class="sxs-lookup"><span data-stu-id="d282d-114">ruleType</span></span>|[<span data-ttu-id="d282d-115">win32LobAppRuleType</span><span class="sxs-lookup"><span data-stu-id="d282d-115">win32LobAppRuleType</span></span>](../resources/intune-apps-win32lobappruletype.md)|<span data-ttu-id="d282d-116">Тип правила, указывающий назначение правила.</span><span class="sxs-lookup"><span data-stu-id="d282d-116">The rule type indicating the purpose of the rule.</span></span> <span data-ttu-id="d282d-117">Наследуется от [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span><span class="sxs-lookup"><span data-stu-id="d282d-117">Inherited from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span></span> <span data-ttu-id="d282d-118">Возможные значения: `detection`, `requirement`.</span><span class="sxs-lookup"><span data-stu-id="d282d-118">Possible values are: `detection`, `requirement`.</span></span>|
|<span data-ttu-id="d282d-119">productCode</span><span class="sxs-lookup"><span data-stu-id="d282d-119">productCode</span></span>|<span data-ttu-id="d282d-120">String</span><span class="sxs-lookup"><span data-stu-id="d282d-120">String</span></span>|<span data-ttu-id="d282d-121">Код продукта приложения.</span><span class="sxs-lookup"><span data-stu-id="d282d-121">The product code of the app.</span></span>|
|<span data-ttu-id="d282d-122">продуктверсионоператор</span><span class="sxs-lookup"><span data-stu-id="d282d-122">productVersionOperator</span></span>|[<span data-ttu-id="d282d-123">win32LobAppRuleOperator</span><span class="sxs-lookup"><span data-stu-id="d282d-123">win32LobAppRuleOperator</span></span>](../resources/intune-apps-win32lobappruleoperator.md)|<span data-ttu-id="d282d-124">Оператор сравнения версий продукта.</span><span class="sxs-lookup"><span data-stu-id="d282d-124">The product version comparison operator.</span></span> <span data-ttu-id="d282d-125">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="d282d-125">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="d282d-126">productVersion</span><span class="sxs-lookup"><span data-stu-id="d282d-126">productVersion</span></span>|<span data-ttu-id="d282d-127">String</span><span class="sxs-lookup"><span data-stu-id="d282d-127">String</span></span>|<span data-ttu-id="d282d-128">Значение сравнения версий продукта.</span><span class="sxs-lookup"><span data-stu-id="d282d-128">The product version comparison value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d282d-129">Связи</span><span class="sxs-lookup"><span data-stu-id="d282d-129">Relationships</span></span>
<span data-ttu-id="d282d-130">Нет</span><span class="sxs-lookup"><span data-stu-id="d282d-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d282d-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d282d-131">JSON Representation</span></span>
<span data-ttu-id="d282d-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d282d-132">Here is a JSON representation of the resource.</span></span>
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





