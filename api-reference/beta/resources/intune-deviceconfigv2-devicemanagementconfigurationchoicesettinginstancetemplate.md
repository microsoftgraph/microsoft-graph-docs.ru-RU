---
title: тип ресурса deviceManagementConfigurationChoiceSettingInstanceTemplate
description: Шаблон параметра выбор экземпляра
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 944c9365e8c30444a00c1c087c6680cac80b0fed
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52664939"
---
# <a name="devicemanagementconfigurationchoicesettinginstancetemplate-resource-type"></a><span data-ttu-id="95a8a-103">тип ресурса deviceManagementConfigurationChoiceSettingInstanceTemplate</span><span class="sxs-lookup"><span data-stu-id="95a8a-103">deviceManagementConfigurationChoiceSettingInstanceTemplate resource type</span></span>

<span data-ttu-id="95a8a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95a8a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="95a8a-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95a8a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95a8a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="95a8a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95a8a-107">Шаблон параметра выбор экземпляра</span><span class="sxs-lookup"><span data-stu-id="95a8a-107">Choice Setting Instance Template</span></span>


<span data-ttu-id="95a8a-108">Наследует [от deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="95a8a-108">Inherits from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>

## <a name="properties"></a><span data-ttu-id="95a8a-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="95a8a-109">Properties</span></span>
|<span data-ttu-id="95a8a-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="95a8a-110">Property</span></span>|<span data-ttu-id="95a8a-111">Тип</span><span class="sxs-lookup"><span data-stu-id="95a8a-111">Type</span></span>|<span data-ttu-id="95a8a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="95a8a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95a8a-113">settingInstanceTemplateId</span><span class="sxs-lookup"><span data-stu-id="95a8a-113">settingInstanceTemplateId</span></span>|<span data-ttu-id="95a8a-114">Строка</span><span class="sxs-lookup"><span data-stu-id="95a8a-114">String</span></span>|<span data-ttu-id="95a8a-115">Настройка кода шаблона экземпляра, унаследованный от [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="95a8a-115">Setting Instance Template Id Inherited from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>|
|<span data-ttu-id="95a8a-116">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="95a8a-116">settingDefinitionId</span></span>|<span data-ttu-id="95a8a-117">Строка</span><span class="sxs-lookup"><span data-stu-id="95a8a-117">String</span></span>|<span data-ttu-id="95a8a-118">Параметр Определения Id, унаследованный от [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="95a8a-118">Setting Definition Id Inherited from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>|
|<span data-ttu-id="95a8a-119">isRequired</span><span class="sxs-lookup"><span data-stu-id="95a8a-119">isRequired</span></span>|<span data-ttu-id="95a8a-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="95a8a-120">Boolean</span></span>|<span data-ttu-id="95a8a-121">Указывает, должна ли политика указать этот параметр.</span><span class="sxs-lookup"><span data-stu-id="95a8a-121">Indicates if a policy must specify this setting.</span></span> <span data-ttu-id="95a8a-122">Унаследованный от [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="95a8a-122">Inherited from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>|
|<span data-ttu-id="95a8a-123">choiceSettingValueTemplate</span><span class="sxs-lookup"><span data-stu-id="95a8a-123">choiceSettingValueTemplate</span></span>|[<span data-ttu-id="95a8a-124">deviceManagementConfigurationChoiceSettingValueTemplate</span><span class="sxs-lookup"><span data-stu-id="95a8a-124">deviceManagementConfigurationChoiceSettingValueTemplate</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingvaluetemplate.md)|<span data-ttu-id="95a8a-125">Шаблон параметра параметра выбор</span><span class="sxs-lookup"><span data-stu-id="95a8a-125">Choice Setting Value Template</span></span>|

## <a name="relationships"></a><span data-ttu-id="95a8a-126">Связи</span><span class="sxs-lookup"><span data-stu-id="95a8a-126">Relationships</span></span>
<span data-ttu-id="95a8a-127">Нет</span><span class="sxs-lookup"><span data-stu-id="95a8a-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="95a8a-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="95a8a-128">JSON Representation</span></span>
<span data-ttu-id="95a8a-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="95a8a-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstanceTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationChoiceSettingInstanceTemplate",
  "settingInstanceTemplateId": "String",
  "settingDefinitionId": "String",
  "isRequired": true,
  "choiceSettingValueTemplate": {
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
}
```




