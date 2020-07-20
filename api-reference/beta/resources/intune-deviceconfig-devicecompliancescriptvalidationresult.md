---
title: Тип ресурса Девицекомплианцескриптвалидатионресулт
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2d91c9ca3b234971a6acc58b7dee8cc736745d85
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44789429"
---
# <a name="devicecompliancescriptvalidationresult-resource-type"></a><span data-ttu-id="8e33f-103">Тип ресурса Девицекомплианцескриптвалидатионресулт</span><span class="sxs-lookup"><span data-stu-id="8e33f-103">deviceComplianceScriptValidationResult resource type</span></span>

<span data-ttu-id="8e33f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e33f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8e33f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e33f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8e33f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8e33f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e33f-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8e33f-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="8e33f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="8e33f-108">Properties</span></span>
|<span data-ttu-id="8e33f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="8e33f-109">Property</span></span>|<span data-ttu-id="8e33f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="8e33f-110">Type</span></span>|<span data-ttu-id="8e33f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8e33f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e33f-112">правила</span><span class="sxs-lookup"><span data-stu-id="8e33f-112">rules</span></span>|<span data-ttu-id="8e33f-113">Коллекция [девицекомплианцескриптруле](../resources/intune-deviceconfig-devicecompliancescriptrule.md)</span><span class="sxs-lookup"><span data-stu-id="8e33f-113">[deviceComplianceScriptRule](../resources/intune-deviceconfig-devicecompliancescriptrule.md) collection</span></span>|<span data-ttu-id="8e33f-114">Проанализированные правила из JSON.</span><span class="sxs-lookup"><span data-stu-id="8e33f-114">Parsed rules from json.</span></span>|
|<span data-ttu-id="8e33f-115">скриптеррорс</span><span class="sxs-lookup"><span data-stu-id="8e33f-115">scriptErrors</span></span>|<span data-ttu-id="8e33f-116">Коллекция [девицекомплианцескриптеррор](../resources/intune-deviceconfig-devicecompliancescripterror.md)</span><span class="sxs-lookup"><span data-stu-id="8e33f-116">[deviceComplianceScriptError](../resources/intune-deviceconfig-devicecompliancescripterror.md) collection</span></span>|<span data-ttu-id="8e33f-117">Ошибки в JSON для скрипта.</span><span class="sxs-lookup"><span data-stu-id="8e33f-117">Errors in json for the script.</span></span>|
|<span data-ttu-id="8e33f-118">рулиррорс</span><span class="sxs-lookup"><span data-stu-id="8e33f-118">ruleErrors</span></span>|<span data-ttu-id="8e33f-119">Коллекция [девицекомплианцескриптрулиррор](../resources/intune-deviceconfig-devicecompliancescriptruleerror.md)</span><span class="sxs-lookup"><span data-stu-id="8e33f-119">[deviceComplianceScriptRuleError](../resources/intune-deviceconfig-devicecompliancescriptruleerror.md) collection</span></span>|<span data-ttu-id="8e33f-120">Ошибки в JSON для сценария для правил.</span><span class="sxs-lookup"><span data-stu-id="8e33f-120">Errors in json for the script for rules.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8e33f-121">Связи</span><span class="sxs-lookup"><span data-stu-id="8e33f-121">Relationships</span></span>
<span data-ttu-id="8e33f-122">Нет</span><span class="sxs-lookup"><span data-stu-id="8e33f-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8e33f-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8e33f-123">JSON Representation</span></span>
<span data-ttu-id="8e33f-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8e33f-124">Here is a JSON representation of the resource.</span></span>
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



