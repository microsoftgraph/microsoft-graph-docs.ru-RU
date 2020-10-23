---
title: Тип ресурса Девицекомплианцескриптвалидатионресулт
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 08b79c44d65c896f0b7a4190678f3569189cd075
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729723"
---
# <a name="devicecompliancescriptvalidationresult-resource-type"></a><span data-ttu-id="98887-103">Тип ресурса Девицекомплианцескриптвалидатионресулт</span><span class="sxs-lookup"><span data-stu-id="98887-103">deviceComplianceScriptValidationResult resource type</span></span>

<span data-ttu-id="98887-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98887-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="98887-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98887-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="98887-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="98887-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98887-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="98887-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="98887-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="98887-108">Properties</span></span>
|<span data-ttu-id="98887-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="98887-109">Property</span></span>|<span data-ttu-id="98887-110">Тип</span><span class="sxs-lookup"><span data-stu-id="98887-110">Type</span></span>|<span data-ttu-id="98887-111">Описание</span><span class="sxs-lookup"><span data-stu-id="98887-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98887-112">правила</span><span class="sxs-lookup"><span data-stu-id="98887-112">rules</span></span>|<span data-ttu-id="98887-113">Коллекция [девицекомплианцескриптруле](../resources/intune-deviceconfig-devicecompliancescriptrule.md)</span><span class="sxs-lookup"><span data-stu-id="98887-113">[deviceComplianceScriptRule](../resources/intune-deviceconfig-devicecompliancescriptrule.md) collection</span></span>|<span data-ttu-id="98887-114">Проанализированные правила из JSON.</span><span class="sxs-lookup"><span data-stu-id="98887-114">Parsed rules from json.</span></span>|
|<span data-ttu-id="98887-115">скриптеррорс</span><span class="sxs-lookup"><span data-stu-id="98887-115">scriptErrors</span></span>|<span data-ttu-id="98887-116">Коллекция [девицекомплианцескриптеррор](../resources/intune-deviceconfig-devicecompliancescripterror.md)</span><span class="sxs-lookup"><span data-stu-id="98887-116">[deviceComplianceScriptError](../resources/intune-deviceconfig-devicecompliancescripterror.md) collection</span></span>|<span data-ttu-id="98887-117">Ошибки в JSON для скрипта.</span><span class="sxs-lookup"><span data-stu-id="98887-117">Errors in json for the script.</span></span>|
|<span data-ttu-id="98887-118">рулиррорс</span><span class="sxs-lookup"><span data-stu-id="98887-118">ruleErrors</span></span>|<span data-ttu-id="98887-119">Коллекция [девицекомплианцескриптрулиррор](../resources/intune-deviceconfig-devicecompliancescriptruleerror.md)</span><span class="sxs-lookup"><span data-stu-id="98887-119">[deviceComplianceScriptRuleError](../resources/intune-deviceconfig-devicecompliancescriptruleerror.md) collection</span></span>|<span data-ttu-id="98887-120">Ошибки в JSON для сценария для правил.</span><span class="sxs-lookup"><span data-stu-id="98887-120">Errors in json for the script for rules.</span></span>|

## <a name="relationships"></a><span data-ttu-id="98887-121">Связи</span><span class="sxs-lookup"><span data-stu-id="98887-121">Relationships</span></span>
<span data-ttu-id="98887-122">Нет</span><span class="sxs-lookup"><span data-stu-id="98887-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="98887-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="98887-123">JSON Representation</span></span>
<span data-ttu-id="98887-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="98887-124">Here is a JSON representation of the resource.</span></span>
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
      "dataType": "String",
      "operand": "String"
    }
  ],
  "scriptErrors": [
    {
      "@odata.type": "microsoft.graph.deviceComplianceScriptError",
      "code": "String",
      "message": "String"
    }
  ],
  "ruleErrors": [
    {
      "@odata.type": "microsoft.graph.deviceComplianceScriptRuleError",
      "code": "String",
      "message": "String",
      "settingName": "String"
    }
  ]
}
```





