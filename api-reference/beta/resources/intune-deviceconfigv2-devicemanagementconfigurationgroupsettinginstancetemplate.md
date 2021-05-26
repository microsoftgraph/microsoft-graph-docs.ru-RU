---
title: тип ресурса deviceManagementConfigurationGroupSettingInstanceTemplate
description: Шаблон экземпляра настройки группы
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 71536897dd8a214e0e4b1c794b7329a3b004afbf
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666550"
---
# <a name="devicemanagementconfigurationgroupsettinginstancetemplate-resource-type"></a><span data-ttu-id="838dd-103">тип ресурса deviceManagementConfigurationGroupSettingInstanceTemplate</span><span class="sxs-lookup"><span data-stu-id="838dd-103">deviceManagementConfigurationGroupSettingInstanceTemplate resource type</span></span>

<span data-ttu-id="838dd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="838dd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="838dd-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="838dd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="838dd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="838dd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="838dd-107">Шаблон экземпляра настройки группы</span><span class="sxs-lookup"><span data-stu-id="838dd-107">Group Setting Instance Template</span></span>


<span data-ttu-id="838dd-108">Наследует [от deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="838dd-108">Inherits from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>

## <a name="properties"></a><span data-ttu-id="838dd-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="838dd-109">Properties</span></span>
|<span data-ttu-id="838dd-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="838dd-110">Property</span></span>|<span data-ttu-id="838dd-111">Тип</span><span class="sxs-lookup"><span data-stu-id="838dd-111">Type</span></span>|<span data-ttu-id="838dd-112">Описание</span><span class="sxs-lookup"><span data-stu-id="838dd-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="838dd-113">settingInstanceTemplateId</span><span class="sxs-lookup"><span data-stu-id="838dd-113">settingInstanceTemplateId</span></span>|<span data-ttu-id="838dd-114">Строка</span><span class="sxs-lookup"><span data-stu-id="838dd-114">String</span></span>|<span data-ttu-id="838dd-115">Настройка кода шаблона экземпляра, унаследованный от [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="838dd-115">Setting Instance Template Id Inherited from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>|
|<span data-ttu-id="838dd-116">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="838dd-116">settingDefinitionId</span></span>|<span data-ttu-id="838dd-117">Строка</span><span class="sxs-lookup"><span data-stu-id="838dd-117">String</span></span>|<span data-ttu-id="838dd-118">Параметр Определения Id, унаследованный от [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="838dd-118">Setting Definition Id Inherited from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>|
|<span data-ttu-id="838dd-119">isRequired</span><span class="sxs-lookup"><span data-stu-id="838dd-119">isRequired</span></span>|<span data-ttu-id="838dd-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="838dd-120">Boolean</span></span>|<span data-ttu-id="838dd-121">Указывает, должна ли политика указать этот параметр.</span><span class="sxs-lookup"><span data-stu-id="838dd-121">Indicates if a policy must specify this setting.</span></span> <span data-ttu-id="838dd-122">Унаследованный от [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="838dd-122">Inherited from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>|
|<span data-ttu-id="838dd-123">groupSettingValueTemplate</span><span class="sxs-lookup"><span data-stu-id="838dd-123">groupSettingValueTemplate</span></span>|[<span data-ttu-id="838dd-124">deviceManagementConfigurationGroupSettingValueTemplate</span><span class="sxs-lookup"><span data-stu-id="838dd-124">deviceManagementConfigurationGroupSettingValueTemplate</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationgroupsettingvaluetemplate.md)|<span data-ttu-id="838dd-125">Шаблон значения параметра группы</span><span class="sxs-lookup"><span data-stu-id="838dd-125">Group Setting Value Template</span></span>|

## <a name="relationships"></a><span data-ttu-id="838dd-126">Связи</span><span class="sxs-lookup"><span data-stu-id="838dd-126">Relationships</span></span>
<span data-ttu-id="838dd-127">Нет</span><span class="sxs-lookup"><span data-stu-id="838dd-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="838dd-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="838dd-128">JSON Representation</span></span>
<span data-ttu-id="838dd-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="838dd-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationGroupSettingInstanceTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationGroupSettingInstanceTemplate",
  "settingInstanceTemplateId": "String",
  "settingDefinitionId": "String",
  "isRequired": true,
  "groupSettingValueTemplate": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationGroupSettingValueTemplate",
    "children": [
      {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingInstanceTemplate",
        "settingInstanceTemplateId": "String",
        "settingDefinitionId": "String",
        "isRequired": true,
        "simpleSettingValueTemplate": {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueTemplate",
          "settingValueTemplateId": "String",
          "defaultValue": {
            "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueConstantDefaultTemplate",
            "constantValue": "String"
          }
        }
      }
    ],
    "settingValueTemplateId": "String"
  }
}
```




