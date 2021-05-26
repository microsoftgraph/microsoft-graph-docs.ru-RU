---
title: тип ресурса deviceManagementConfigurationChoiceSettingCollectionInstanceTemplate
description: Шаблон экземпляра параметра выбор коллекции
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9f8741ab5b771325935512a179d837864a2a5b3b
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666256"
---
# <a name="devicemanagementconfigurationchoicesettingcollectioninstancetemplate-resource-type"></a><span data-ttu-id="5786e-103">тип ресурса deviceManagementConfigurationChoiceSettingCollectionInstanceTemplate</span><span class="sxs-lookup"><span data-stu-id="5786e-103">deviceManagementConfigurationChoiceSettingCollectionInstanceTemplate resource type</span></span>

<span data-ttu-id="5786e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5786e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5786e-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5786e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5786e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5786e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5786e-107">Шаблон экземпляра параметра выбор коллекции</span><span class="sxs-lookup"><span data-stu-id="5786e-107">Choice Setting Collection Instance Template</span></span>


<span data-ttu-id="5786e-108">Наследует [от deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="5786e-108">Inherits from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5786e-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="5786e-109">Properties</span></span>
|<span data-ttu-id="5786e-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="5786e-110">Property</span></span>|<span data-ttu-id="5786e-111">Тип</span><span class="sxs-lookup"><span data-stu-id="5786e-111">Type</span></span>|<span data-ttu-id="5786e-112">Описание</span><span class="sxs-lookup"><span data-stu-id="5786e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5786e-113">settingInstanceTemplateId</span><span class="sxs-lookup"><span data-stu-id="5786e-113">settingInstanceTemplateId</span></span>|<span data-ttu-id="5786e-114">Строка</span><span class="sxs-lookup"><span data-stu-id="5786e-114">String</span></span>|<span data-ttu-id="5786e-115">Настройка кода шаблона экземпляра, унаследованный от [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="5786e-115">Setting Instance Template Id Inherited from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>|
|<span data-ttu-id="5786e-116">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="5786e-116">settingDefinitionId</span></span>|<span data-ttu-id="5786e-117">Строка</span><span class="sxs-lookup"><span data-stu-id="5786e-117">String</span></span>|<span data-ttu-id="5786e-118">Параметр Определения Id, унаследованный от [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="5786e-118">Setting Definition Id Inherited from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>|
|<span data-ttu-id="5786e-119">isRequired</span><span class="sxs-lookup"><span data-stu-id="5786e-119">isRequired</span></span>|<span data-ttu-id="5786e-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="5786e-120">Boolean</span></span>|<span data-ttu-id="5786e-121">Указывает, должна ли политика указать этот параметр.</span><span class="sxs-lookup"><span data-stu-id="5786e-121">Indicates if a policy must specify this setting.</span></span> <span data-ttu-id="5786e-122">Унаследованный от [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="5786e-122">Inherited from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>|
|<span data-ttu-id="5786e-123">choiceSettingCollectionValueTemplate</span><span class="sxs-lookup"><span data-stu-id="5786e-123">choiceSettingCollectionValueTemplate</span></span>|<span data-ttu-id="5786e-124">[коллекция deviceManagementConfigurationChoiceSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingvaluetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="5786e-124">[deviceManagementConfigurationChoiceSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingvaluetemplate.md) collection</span></span>|<span data-ttu-id="5786e-125">Шаблон значения параметра выбор коллекции</span><span class="sxs-lookup"><span data-stu-id="5786e-125">Choice Setting Collection Value Template</span></span>|
|<span data-ttu-id="5786e-126">allowUnmanagedValues</span><span class="sxs-lookup"><span data-stu-id="5786e-126">allowUnmanagedValues</span></span>|<span data-ttu-id="5786e-127">Логический</span><span class="sxs-lookup"><span data-stu-id="5786e-127">Boolean</span></span>|<span data-ttu-id="5786e-128">Связанная политика может при добавлении значений, которые не присутствуют в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="5786e-128">Linked policy may append values which are not present in the template.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5786e-129">Связи</span><span class="sxs-lookup"><span data-stu-id="5786e-129">Relationships</span></span>
<span data-ttu-id="5786e-130">Нет</span><span class="sxs-lookup"><span data-stu-id="5786e-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5786e-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5786e-131">JSON Representation</span></span>
<span data-ttu-id="5786e-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5786e-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingCollectionInstanceTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationChoiceSettingCollectionInstanceTemplate",
  "settingInstanceTemplateId": "String",
  "settingDefinitionId": "String",
  "isRequired": true,
  "choiceSettingCollectionValueTemplate": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValueTemplate",
      "defaultValue": {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValueConstantDefaultTemplate",
        "settingDefinitionOptionId": "String",
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
        ]
      },
      "recommendedValueDefinition": {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValueDefinitionTemplate",
        "allowedOptions": [
          {
            "@odata.type": "microsoft.graph.deviceManagementConfigurationOptionDefinitionTemplate",
            "itemId": "String",
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
            ]
          }
        ]
      },
      "requiredValueDefinition": {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValueDefinitionTemplate",
        "allowedOptions": [
          {
            "@odata.type": "microsoft.graph.deviceManagementConfigurationOptionDefinitionTemplate",
            "itemId": "String",
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
            ]
          }
        ]
      },
      "settingValueTemplateId": "String"
    }
  ],
  "allowUnmanagedValues": true
}
```




