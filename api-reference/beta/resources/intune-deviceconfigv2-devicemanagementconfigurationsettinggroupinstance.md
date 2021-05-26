---
title: тип ресурса deviceManagementConfigurationSettingGroupInstance
description: Настройка экземпляра в политике
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3a86aa25a13c7f3a089229640186e70c13f19797
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665611"
---
# <a name="devicemanagementconfigurationsettinggroupinstance-resource-type"></a><span data-ttu-id="8c5a5-103">тип ресурса deviceManagementConfigurationSettingGroupInstance</span><span class="sxs-lookup"><span data-stu-id="8c5a5-103">deviceManagementConfigurationSettingGroupInstance resource type</span></span>

<span data-ttu-id="8c5a5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c5a5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8c5a5-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c5a5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c5a5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8c5a5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c5a5-107">Настройка экземпляра в политике</span><span class="sxs-lookup"><span data-stu-id="8c5a5-107">Setting instance within policy</span></span>


<span data-ttu-id="8c5a5-108">Наследует [от deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="8c5a5-108">Inherits from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8c5a5-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="8c5a5-109">Properties</span></span>
|<span data-ttu-id="8c5a5-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="8c5a5-110">Property</span></span>|<span data-ttu-id="8c5a5-111">Тип</span><span class="sxs-lookup"><span data-stu-id="8c5a5-111">Type</span></span>|<span data-ttu-id="8c5a5-112">Описание</span><span class="sxs-lookup"><span data-stu-id="8c5a5-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c5a5-113">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="8c5a5-113">settingDefinitionId</span></span>|<span data-ttu-id="8c5a5-114">Строка</span><span class="sxs-lookup"><span data-stu-id="8c5a5-114">String</span></span>|<span data-ttu-id="8c5a5-115">Параметр Определения Id, унаследованный от [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="8c5a5-115">Setting Definition Id Inherited from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>|
|<span data-ttu-id="8c5a5-116">settingInstanceTemplateReference</span><span class="sxs-lookup"><span data-stu-id="8c5a5-116">settingInstanceTemplateReference</span></span>|[<span data-ttu-id="8c5a5-117">deviceManagementConfigurationSettingInstanceTemplateReference</span><span class="sxs-lookup"><span data-stu-id="8c5a5-117">deviceManagementConfigurationSettingInstanceTemplateReference</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplatereference.md)|<span data-ttu-id="8c5a5-118">Настройка ссылки шаблона экземпляра, унаследованной от [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="8c5a5-118">Setting Instance Template Reference Inherited from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c5a5-119">Связи</span><span class="sxs-lookup"><span data-stu-id="8c5a5-119">Relationships</span></span>
<span data-ttu-id="8c5a5-120">Нет</span><span class="sxs-lookup"><span data-stu-id="8c5a5-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8c5a5-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8c5a5-121">JSON Representation</span></span>
<span data-ttu-id="8c5a5-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8c5a5-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingGroupInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingGroupInstance",
  "settingDefinitionId": "String",
  "settingInstanceTemplateReference": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
    "settingInstanceTemplateId": "String"
  }
}
```




