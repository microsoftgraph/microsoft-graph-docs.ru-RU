---
title: тип ресурса deviceManagementConfigurationSimpleSettingCollectionInstance
description: Экземпляр коллекции простых параметров
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 30dcfb5d02aebb1e7bf346c6dd1f4b37e1103b49
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52664925"
---
# <a name="devicemanagementconfigurationsimplesettingcollectioninstance-resource-type"></a><span data-ttu-id="fdbfd-103">тип ресурса deviceManagementConfigurationSimpleSettingCollectionInstance</span><span class="sxs-lookup"><span data-stu-id="fdbfd-103">deviceManagementConfigurationSimpleSettingCollectionInstance resource type</span></span>

<span data-ttu-id="fdbfd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fdbfd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fdbfd-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fdbfd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fdbfd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fdbfd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fdbfd-107">Экземпляр коллекции простых параметров</span><span class="sxs-lookup"><span data-stu-id="fdbfd-107">Simple setting collection instance</span></span>


<span data-ttu-id="fdbfd-108">Наследует [от deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="fdbfd-108">Inherits from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fdbfd-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="fdbfd-109">Properties</span></span>
|<span data-ttu-id="fdbfd-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="fdbfd-110">Property</span></span>|<span data-ttu-id="fdbfd-111">Тип</span><span class="sxs-lookup"><span data-stu-id="fdbfd-111">Type</span></span>|<span data-ttu-id="fdbfd-112">Описание</span><span class="sxs-lookup"><span data-stu-id="fdbfd-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fdbfd-113">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="fdbfd-113">settingDefinitionId</span></span>|<span data-ttu-id="fdbfd-114">Строка</span><span class="sxs-lookup"><span data-stu-id="fdbfd-114">String</span></span>|<span data-ttu-id="fdbfd-115">Параметр Определения Id, унаследованный от [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="fdbfd-115">Setting Definition Id Inherited from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>|
|<span data-ttu-id="fdbfd-116">settingInstanceTemplateReference</span><span class="sxs-lookup"><span data-stu-id="fdbfd-116">settingInstanceTemplateReference</span></span>|[<span data-ttu-id="fdbfd-117">deviceManagementConfigurationSettingInstanceTemplateReference</span><span class="sxs-lookup"><span data-stu-id="fdbfd-117">deviceManagementConfigurationSettingInstanceTemplateReference</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplatereference.md)|<span data-ttu-id="fdbfd-118">Настройка ссылки шаблона экземпляра, унаследованной от [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="fdbfd-118">Setting Instance Template Reference Inherited from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>|
|<span data-ttu-id="fdbfd-119">simpleSettingCollectionValue</span><span class="sxs-lookup"><span data-stu-id="fdbfd-119">simpleSettingCollectionValue</span></span>|<span data-ttu-id="fdbfd-120">[коллекция deviceManagementConfigurationSimpleSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="fdbfd-120">[deviceManagementConfigurationSimpleSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvalue.md) collection</span></span>|<span data-ttu-id="fdbfd-121">Простое значение экземпляра коллекции параметров</span><span class="sxs-lookup"><span data-stu-id="fdbfd-121">Simple setting collection instance value</span></span>|

## <a name="relationships"></a><span data-ttu-id="fdbfd-122">Связи</span><span class="sxs-lookup"><span data-stu-id="fdbfd-122">Relationships</span></span>
<span data-ttu-id="fdbfd-123">Нет</span><span class="sxs-lookup"><span data-stu-id="fdbfd-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fdbfd-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fdbfd-124">JSON Representation</span></span>
<span data-ttu-id="fdbfd-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fdbfd-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingCollectionInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSimpleSettingCollectionInstance",
  "settingDefinitionId": "String",
  "settingInstanceTemplateReference": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
    "settingInstanceTemplateId": "String"
  },
  "simpleSettingCollectionValue": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValue",
      "settingValueTemplateReference": {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
        "settingValueTemplateId": "String",
        "useTemplateDefault": true
      },
      "value": "String"
    }
  ]
}
```




