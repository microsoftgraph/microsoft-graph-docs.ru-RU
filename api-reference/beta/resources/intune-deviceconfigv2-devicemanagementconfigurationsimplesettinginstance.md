---
title: тип ресурса deviceManagementConfigurationSimpleSettingInstance
description: Простой экземпляр параметра
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6c815ec0b90211ede9429abe707856af27ed79b5
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666725"
---
# <a name="devicemanagementconfigurationsimplesettinginstance-resource-type"></a><span data-ttu-id="df6ca-103">тип ресурса deviceManagementConfigurationSimpleSettingInstance</span><span class="sxs-lookup"><span data-stu-id="df6ca-103">deviceManagementConfigurationSimpleSettingInstance resource type</span></span>

<span data-ttu-id="df6ca-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df6ca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="df6ca-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df6ca-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df6ca-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="df6ca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df6ca-107">Простой экземпляр параметра</span><span class="sxs-lookup"><span data-stu-id="df6ca-107">Simple setting instance</span></span>


<span data-ttu-id="df6ca-108">Наследует [от deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="df6ca-108">Inherits from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>

## <a name="properties"></a><span data-ttu-id="df6ca-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="df6ca-109">Properties</span></span>
|<span data-ttu-id="df6ca-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="df6ca-110">Property</span></span>|<span data-ttu-id="df6ca-111">Тип</span><span class="sxs-lookup"><span data-stu-id="df6ca-111">Type</span></span>|<span data-ttu-id="df6ca-112">Описание</span><span class="sxs-lookup"><span data-stu-id="df6ca-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df6ca-113">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="df6ca-113">settingDefinitionId</span></span>|<span data-ttu-id="df6ca-114">Строка</span><span class="sxs-lookup"><span data-stu-id="df6ca-114">String</span></span>|<span data-ttu-id="df6ca-115">Параметр Определения Id, унаследованный от [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="df6ca-115">Setting Definition Id Inherited from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>|
|<span data-ttu-id="df6ca-116">settingInstanceTemplateReference</span><span class="sxs-lookup"><span data-stu-id="df6ca-116">settingInstanceTemplateReference</span></span>|[<span data-ttu-id="df6ca-117">deviceManagementConfigurationSettingInstanceTemplateReference</span><span class="sxs-lookup"><span data-stu-id="df6ca-117">deviceManagementConfigurationSettingInstanceTemplateReference</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplatereference.md)|<span data-ttu-id="df6ca-118">Настройка ссылки шаблона экземпляра, унаследованной от [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="df6ca-118">Setting Instance Template Reference Inherited from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>|
|<span data-ttu-id="df6ca-119">simpleSettingValue</span><span class="sxs-lookup"><span data-stu-id="df6ca-119">simpleSettingValue</span></span>|[<span data-ttu-id="df6ca-120">deviceManagementConfigurationSimpleSettingValue</span><span class="sxs-lookup"><span data-stu-id="df6ca-120">deviceManagementConfigurationSimpleSettingValue</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvalue.md)|<span data-ttu-id="df6ca-121">Простое значение экземпляра параметра</span><span class="sxs-lookup"><span data-stu-id="df6ca-121">Simple setting instance value</span></span>|

## <a name="relationships"></a><span data-ttu-id="df6ca-122">Связи</span><span class="sxs-lookup"><span data-stu-id="df6ca-122">Relationships</span></span>
<span data-ttu-id="df6ca-123">Нет</span><span class="sxs-lookup"><span data-stu-id="df6ca-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="df6ca-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="df6ca-124">JSON Representation</span></span>
<span data-ttu-id="df6ca-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="df6ca-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSimpleSettingInstance",
  "settingDefinitionId": "String",
  "settingInstanceTemplateReference": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
    "settingInstanceTemplateId": "String"
  },
  "simpleSettingValue": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValue",
    "settingValueTemplateReference": {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
      "settingValueTemplateId": "String",
      "useTemplateDefault": true
    },
    "value": "String"
  }
}
```




