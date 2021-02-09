---
title: Тип ресурса deviceComplianceScriptValidationResult
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d76d96acf8dc96275902d1fba30f8ba6f49cc088
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154280"
---
# <a name="devicecompliancescriptvalidationresult-resource-type"></a><span data-ttu-id="ea86f-103">Тип ресурса deviceComplianceScriptValidationResult</span><span class="sxs-lookup"><span data-stu-id="ea86f-103">deviceComplianceScriptValidationResult resource type</span></span>

<span data-ttu-id="ea86f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea86f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ea86f-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea86f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea86f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ea86f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea86f-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ea86f-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="ea86f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ea86f-108">Properties</span></span>
|<span data-ttu-id="ea86f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ea86f-109">Property</span></span>|<span data-ttu-id="ea86f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ea86f-110">Type</span></span>|<span data-ttu-id="ea86f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ea86f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea86f-112">правила</span><span class="sxs-lookup"><span data-stu-id="ea86f-112">rules</span></span>|<span data-ttu-id="ea86f-113">[Коллекция deviceComplianceScriptRule](../resources/intune-deviceconfig-devicecompliancescriptrule.md)</span><span class="sxs-lookup"><span data-stu-id="ea86f-113">[deviceComplianceScriptRule](../resources/intune-deviceconfig-devicecompliancescriptrule.md) collection</span></span>|<span data-ttu-id="ea86f-114">Правила для различенного из json.</span><span class="sxs-lookup"><span data-stu-id="ea86f-114">Parsed rules from json.</span></span>|
|<span data-ttu-id="ea86f-115">scriptErrors</span><span class="sxs-lookup"><span data-stu-id="ea86f-115">scriptErrors</span></span>|<span data-ttu-id="ea86f-116">[Коллекция deviceComplianceScriptError](../resources/intune-deviceconfig-devicecompliancescripterror.md)</span><span class="sxs-lookup"><span data-stu-id="ea86f-116">[deviceComplianceScriptError](../resources/intune-deviceconfig-devicecompliancescripterror.md) collection</span></span>|<span data-ttu-id="ea86f-117">Ошибки в json для сценария.</span><span class="sxs-lookup"><span data-stu-id="ea86f-117">Errors in json for the script.</span></span>|
|<span data-ttu-id="ea86f-118">ruleErrors</span><span class="sxs-lookup"><span data-stu-id="ea86f-118">ruleErrors</span></span>|<span data-ttu-id="ea86f-119">[Коллекция deviceComplianceScriptRuleError](../resources/intune-deviceconfig-devicecompliancescriptruleerror.md)</span><span class="sxs-lookup"><span data-stu-id="ea86f-119">[deviceComplianceScriptRuleError](../resources/intune-deviceconfig-devicecompliancescriptruleerror.md) collection</span></span>|<span data-ttu-id="ea86f-120">Ошибки в json для скрипта для правил.</span><span class="sxs-lookup"><span data-stu-id="ea86f-120">Errors in json for the script for rules.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ea86f-121">Связи</span><span class="sxs-lookup"><span data-stu-id="ea86f-121">Relationships</span></span>
<span data-ttu-id="ea86f-122">Нет</span><span class="sxs-lookup"><span data-stu-id="ea86f-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ea86f-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ea86f-123">JSON Representation</span></span>
<span data-ttu-id="ea86f-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ea86f-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceComplianceScriptValidationResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptValidationResult",
  "rules": [
    {
      "@odata.type": "microsoft.graph.deviceComplianceScriptRule",
      "settingName": "String",
      "operator": "String",
      "deviceComplianceScriptRulOperator": "String",
      "dataType": "String",
      "deviceComplianceScriptRuleDataType": "String",
      "operand": "String"
    }
  ],
  "scriptErrors": [
    {
      "@odata.type": "microsoft.graph.deviceComplianceScriptError",
      "code": "String",
      "deviceComplianceScriptRulesValidationError": "String",
      "message": "String"
    }
  ],
  "ruleErrors": [
    {
      "@odata.type": "microsoft.graph.deviceComplianceScriptRuleError",
      "code": "String",
      "deviceComplianceScriptRulesValidationError": "String",
      "message": "String",
      "settingName": "String"
    }
  ]
}
```




