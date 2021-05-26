---
title: тип ресурса deviceManagementConfigurationSettingGroupCollectionInstance
description: Настройка экземпляра в политике
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: af7bab6d165780c66a7f61ce0143be98bd0195b7
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665618"
---
# <a name="devicemanagementconfigurationsettinggroupcollectioninstance-resource-type"></a><span data-ttu-id="ba850-103">тип ресурса deviceManagementConfigurationSettingGroupCollectionInstance</span><span class="sxs-lookup"><span data-stu-id="ba850-103">deviceManagementConfigurationSettingGroupCollectionInstance resource type</span></span>

<span data-ttu-id="ba850-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba850-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ba850-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba850-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba850-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ba850-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba850-107">Настройка экземпляра в политике</span><span class="sxs-lookup"><span data-stu-id="ba850-107">Setting instance within policy</span></span>


<span data-ttu-id="ba850-108">Наследует [от deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="ba850-108">Inherits from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ba850-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="ba850-109">Properties</span></span>
|<span data-ttu-id="ba850-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="ba850-110">Property</span></span>|<span data-ttu-id="ba850-111">Тип</span><span class="sxs-lookup"><span data-stu-id="ba850-111">Type</span></span>|<span data-ttu-id="ba850-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ba850-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba850-113">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="ba850-113">settingDefinitionId</span></span>|<span data-ttu-id="ba850-114">Строка</span><span class="sxs-lookup"><span data-stu-id="ba850-114">String</span></span>|<span data-ttu-id="ba850-115">Параметр Определения Id, унаследованный от [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="ba850-115">Setting Definition Id Inherited from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>|
|<span data-ttu-id="ba850-116">settingInstanceTemplateReference</span><span class="sxs-lookup"><span data-stu-id="ba850-116">settingInstanceTemplateReference</span></span>|[<span data-ttu-id="ba850-117">deviceManagementConfigurationSettingInstanceTemplateReference</span><span class="sxs-lookup"><span data-stu-id="ba850-117">deviceManagementConfigurationSettingInstanceTemplateReference</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplatereference.md)|<span data-ttu-id="ba850-118">Настройка ссылки шаблона экземпляра, унаследованной от [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="ba850-118">Setting Instance Template Reference Inherited from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="ba850-119">Связи</span><span class="sxs-lookup"><span data-stu-id="ba850-119">Relationships</span></span>
<span data-ttu-id="ba850-120">Нет</span><span class="sxs-lookup"><span data-stu-id="ba850-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ba850-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ba850-121">JSON Representation</span></span>
<span data-ttu-id="ba850-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ba850-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingGroupCollectionInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingGroupCollectionInstance",
  "settingDefinitionId": "String",
  "settingInstanceTemplateReference": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
    "settingInstanceTemplateId": "String"
  }
}
```




