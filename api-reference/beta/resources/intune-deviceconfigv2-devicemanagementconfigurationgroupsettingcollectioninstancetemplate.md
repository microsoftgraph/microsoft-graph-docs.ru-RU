---
title: тип ресурса deviceManagementConfigurationGroupSettingCollectionInstanceTemplate
description: Шаблон экземпляра экземпляра коллекции параметров группы
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0c5433edec34908e7b10e6212387b442e76edcd6
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666564"
---
# <a name="devicemanagementconfigurationgroupsettingcollectioninstancetemplate-resource-type"></a><span data-ttu-id="c55c7-103">тип ресурса deviceManagementConfigurationGroupSettingCollectionInstanceTemplate</span><span class="sxs-lookup"><span data-stu-id="c55c7-103">deviceManagementConfigurationGroupSettingCollectionInstanceTemplate resource type</span></span>

<span data-ttu-id="c55c7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c55c7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c55c7-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c55c7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c55c7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c55c7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c55c7-107">Шаблон экземпляра экземпляра коллекции параметров группы</span><span class="sxs-lookup"><span data-stu-id="c55c7-107">Group Setting Collection Instance Template</span></span>


<span data-ttu-id="c55c7-108">Наследует [от deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="c55c7-108">Inherits from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c55c7-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="c55c7-109">Properties</span></span>
|<span data-ttu-id="c55c7-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="c55c7-110">Property</span></span>|<span data-ttu-id="c55c7-111">Тип</span><span class="sxs-lookup"><span data-stu-id="c55c7-111">Type</span></span>|<span data-ttu-id="c55c7-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c55c7-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c55c7-113">settingInstanceTemplateId</span><span class="sxs-lookup"><span data-stu-id="c55c7-113">settingInstanceTemplateId</span></span>|<span data-ttu-id="c55c7-114">Строка</span><span class="sxs-lookup"><span data-stu-id="c55c7-114">String</span></span>|<span data-ttu-id="c55c7-115">Настройка кода шаблона экземпляра, унаследованный от [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="c55c7-115">Setting Instance Template Id Inherited from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>|
|<span data-ttu-id="c55c7-116">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="c55c7-116">settingDefinitionId</span></span>|<span data-ttu-id="c55c7-117">Строка</span><span class="sxs-lookup"><span data-stu-id="c55c7-117">String</span></span>|<span data-ttu-id="c55c7-118">Параметр Определения Id, унаследованный от [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="c55c7-118">Setting Definition Id Inherited from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>|
|<span data-ttu-id="c55c7-119">isRequired</span><span class="sxs-lookup"><span data-stu-id="c55c7-119">isRequired</span></span>|<span data-ttu-id="c55c7-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="c55c7-120">Boolean</span></span>|<span data-ttu-id="c55c7-121">Указывает, должна ли политика указать этот параметр.</span><span class="sxs-lookup"><span data-stu-id="c55c7-121">Indicates if a policy must specify this setting.</span></span> <span data-ttu-id="c55c7-122">Унаследованный от [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="c55c7-122">Inherited from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>|
|<span data-ttu-id="c55c7-123">groupSettingCollectionValueTemplate</span><span class="sxs-lookup"><span data-stu-id="c55c7-123">groupSettingCollectionValueTemplate</span></span>|<span data-ttu-id="c55c7-124">[коллекция deviceManagementConfigurationGroupSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationgroupsettingvaluetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="c55c7-124">[deviceManagementConfigurationGroupSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationgroupsettingvaluetemplate.md) collection</span></span>|<span data-ttu-id="c55c7-125">Шаблон значения коллекции параметров группы</span><span class="sxs-lookup"><span data-stu-id="c55c7-125">Group Setting Collection Value Template</span></span>|
|<span data-ttu-id="c55c7-126">allowUnmanagedValues</span><span class="sxs-lookup"><span data-stu-id="c55c7-126">allowUnmanagedValues</span></span>|<span data-ttu-id="c55c7-127">Логический</span><span class="sxs-lookup"><span data-stu-id="c55c7-127">Boolean</span></span>|<span data-ttu-id="c55c7-128">Связанная политика может при добавлении значений, которые не присутствуют в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="c55c7-128">Linked policy may append values which are not present in the template.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c55c7-129">Связи</span><span class="sxs-lookup"><span data-stu-id="c55c7-129">Relationships</span></span>
<span data-ttu-id="c55c7-130">Нет</span><span class="sxs-lookup"><span data-stu-id="c55c7-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c55c7-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c55c7-131">JSON Representation</span></span>
<span data-ttu-id="c55c7-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c55c7-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationGroupSettingCollectionInstanceTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationGroupSettingCollectionInstanceTemplate",
  "settingInstanceTemplateId": "String",
  "settingDefinitionId": "String",
  "isRequired": true,
  "groupSettingCollectionValueTemplate": [
    {
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
  ],
  "allowUnmanagedValues": true
}
```




