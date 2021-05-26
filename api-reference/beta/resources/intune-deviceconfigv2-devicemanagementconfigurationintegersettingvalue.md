---
title: тип ресурса deviceManagementConfigurationIntegerSettingValue
description: Простое значение параметра
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 24717f3a3d983c25198a3f94ecb5027f49f763c3
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666529"
---
# <a name="devicemanagementconfigurationintegersettingvalue-resource-type"></a><span data-ttu-id="766b9-103">тип ресурса deviceManagementConfigurationIntegerSettingValue</span><span class="sxs-lookup"><span data-stu-id="766b9-103">deviceManagementConfigurationIntegerSettingValue resource type</span></span>

<span data-ttu-id="766b9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="766b9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="766b9-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="766b9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="766b9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="766b9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="766b9-107">Простое значение параметра</span><span class="sxs-lookup"><span data-stu-id="766b9-107">Simple setting value</span></span>


<span data-ttu-id="766b9-108">Наследует [от deviceManagementConfigurationSimpleSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="766b9-108">Inherits from [deviceManagementConfigurationSimpleSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvalue.md)</span></span>

## <a name="properties"></a><span data-ttu-id="766b9-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="766b9-109">Properties</span></span>
|<span data-ttu-id="766b9-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="766b9-110">Property</span></span>|<span data-ttu-id="766b9-111">Тип</span><span class="sxs-lookup"><span data-stu-id="766b9-111">Type</span></span>|<span data-ttu-id="766b9-112">Описание</span><span class="sxs-lookup"><span data-stu-id="766b9-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="766b9-113">settingValueTemplateReference</span><span class="sxs-lookup"><span data-stu-id="766b9-113">settingValueTemplateReference</span></span>|[<span data-ttu-id="766b9-114">deviceManagementConfigurationSettingValueTemplateReference</span><span class="sxs-lookup"><span data-stu-id="766b9-114">deviceManagementConfigurationSettingValueTemplateReference</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvaluetemplatereference.md)|<span data-ttu-id="766b9-115">Настройка ссылки шаблона значений, унаследованной от [deviceManagementConfigurationSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="766b9-115">Setting value template reference Inherited from [deviceManagementConfigurationSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)</span></span>|
|<span data-ttu-id="766b9-116">value</span><span class="sxs-lookup"><span data-stu-id="766b9-116">value</span></span>|<span data-ttu-id="766b9-117">Int32</span><span class="sxs-lookup"><span data-stu-id="766b9-117">Int32</span></span>|<span data-ttu-id="766b9-118">Значение параметра integer.</span><span class="sxs-lookup"><span data-stu-id="766b9-118">Value of the integer setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="766b9-119">Связи</span><span class="sxs-lookup"><span data-stu-id="766b9-119">Relationships</span></span>
<span data-ttu-id="766b9-120">Нет</span><span class="sxs-lookup"><span data-stu-id="766b9-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="766b9-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="766b9-121">JSON Representation</span></span>
<span data-ttu-id="766b9-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="766b9-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationIntegerSettingValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationIntegerSettingValue",
  "settingValueTemplateReference": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
    "settingValueTemplateId": "String",
    "useTemplateDefault": true
  },
  "value": 1024
}
```




