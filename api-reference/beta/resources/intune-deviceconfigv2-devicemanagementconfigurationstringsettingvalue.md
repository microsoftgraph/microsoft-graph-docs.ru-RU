---
title: тип ресурса deviceManagementConfigurationStringSettingValue
description: Простое значение параметра
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2e2374fd660fbfdcebee46ec6053d8ddc93f2010
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666704"
---
# <a name="devicemanagementconfigurationstringsettingvalue-resource-type"></a><span data-ttu-id="4c49e-103">тип ресурса deviceManagementConfigurationStringSettingValue</span><span class="sxs-lookup"><span data-stu-id="4c49e-103">deviceManagementConfigurationStringSettingValue resource type</span></span>

<span data-ttu-id="4c49e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c49e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4c49e-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c49e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4c49e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4c49e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c49e-107">Простое значение параметра</span><span class="sxs-lookup"><span data-stu-id="4c49e-107">Simple setting value</span></span>


<span data-ttu-id="4c49e-108">Наследует [от deviceManagementConfigurationSimpleSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="4c49e-108">Inherits from [deviceManagementConfigurationSimpleSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvalue.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4c49e-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="4c49e-109">Properties</span></span>
|<span data-ttu-id="4c49e-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c49e-110">Property</span></span>|<span data-ttu-id="4c49e-111">Тип</span><span class="sxs-lookup"><span data-stu-id="4c49e-111">Type</span></span>|<span data-ttu-id="4c49e-112">Описание</span><span class="sxs-lookup"><span data-stu-id="4c49e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c49e-113">settingValueTemplateReference</span><span class="sxs-lookup"><span data-stu-id="4c49e-113">settingValueTemplateReference</span></span>|[<span data-ttu-id="4c49e-114">deviceManagementConfigurationSettingValueTemplateReference</span><span class="sxs-lookup"><span data-stu-id="4c49e-114">deviceManagementConfigurationSettingValueTemplateReference</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvaluetemplatereference.md)|<span data-ttu-id="4c49e-115">Настройка ссылки шаблона значений, унаследованной от [deviceManagementConfigurationSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="4c49e-115">Setting value template reference Inherited from [deviceManagementConfigurationSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)</span></span>|
|<span data-ttu-id="4c49e-116">value</span><span class="sxs-lookup"><span data-stu-id="4c49e-116">value</span></span>|<span data-ttu-id="4c49e-117">String</span><span class="sxs-lookup"><span data-stu-id="4c49e-117">String</span></span>|<span data-ttu-id="4c49e-118">Значение параметра строки.</span><span class="sxs-lookup"><span data-stu-id="4c49e-118">Value of the string setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4c49e-119">Связи</span><span class="sxs-lookup"><span data-stu-id="4c49e-119">Relationships</span></span>
<span data-ttu-id="4c49e-120">Нет</span><span class="sxs-lookup"><span data-stu-id="4c49e-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4c49e-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4c49e-121">JSON Representation</span></span>
<span data-ttu-id="4c49e-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4c49e-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationStringSettingValue",
  "settingValueTemplateReference": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
    "settingValueTemplateId": "String",
    "useTemplateDefault": true
  },
  "value": "String"
}
```




