---
title: тип ресурса deviceManagementConfigurationChoiceSettingValueTemplate
description: Шаблон параметра параметра выбор
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cffa6a685053194b8ff554d101fecd98f6c6456a
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868929"
---
# <a name="devicemanagementconfigurationchoicesettingvaluetemplate-resource-type"></a><span data-ttu-id="3a69d-103">тип ресурса deviceManagementConfigurationChoiceSettingValueTemplate</span><span class="sxs-lookup"><span data-stu-id="3a69d-103">deviceManagementConfigurationChoiceSettingValueTemplate resource type</span></span>

<span data-ttu-id="3a69d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a69d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3a69d-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a69d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3a69d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3a69d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a69d-107">Шаблон параметра параметра выбор</span><span class="sxs-lookup"><span data-stu-id="3a69d-107">Choice Setting Value Template</span></span>

## <a name="properties"></a><span data-ttu-id="3a69d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3a69d-108">Properties</span></span>
|<span data-ttu-id="3a69d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3a69d-109">Property</span></span>|<span data-ttu-id="3a69d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3a69d-110">Type</span></span>|<span data-ttu-id="3a69d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3a69d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a69d-112">defaultValue</span><span class="sxs-lookup"><span data-stu-id="3a69d-112">defaultValue</span></span>|[<span data-ttu-id="3a69d-113">deviceManagementConfigurationChoiceSettingValueDefaultTemplate</span><span class="sxs-lookup"><span data-stu-id="3a69d-113">deviceManagementConfigurationChoiceSettingValueDefaultTemplate</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingvaluedefaulttemplate.md)|<span data-ttu-id="3a69d-114">Шаблон параметра параметра значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="3a69d-114">Choice Setting Value Default Template.</span></span>|
|<span data-ttu-id="3a69d-115">recommendedValueDefinition</span><span class="sxs-lookup"><span data-stu-id="3a69d-115">recommendedValueDefinition</span></span>|[<span data-ttu-id="3a69d-116">deviceManagementConfigurationChoiceSettingValueDefinitionTemplate</span><span class="sxs-lookup"><span data-stu-id="3a69d-116">deviceManagementConfigurationChoiceSettingValueDefinitionTemplate</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingvaluedefinitiontemplate.md)|<span data-ttu-id="3a69d-117">Рекомендуемые переопределения определения.</span><span class="sxs-lookup"><span data-stu-id="3a69d-117">Recommended definition override.</span></span>|
|<span data-ttu-id="3a69d-118">requiredValueDefinition</span><span class="sxs-lookup"><span data-stu-id="3a69d-118">requiredValueDefinition</span></span>|[<span data-ttu-id="3a69d-119">deviceManagementConfigurationChoiceSettingValueDefinitionTemplate</span><span class="sxs-lookup"><span data-stu-id="3a69d-119">deviceManagementConfigurationChoiceSettingValueDefinitionTemplate</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingvaluedefinitiontemplate.md)|<span data-ttu-id="3a69d-120">Обязательное переопределения определения.</span><span class="sxs-lookup"><span data-stu-id="3a69d-120">Required definition override.</span></span>|
|<span data-ttu-id="3a69d-121">settingValueTemplateId</span><span class="sxs-lookup"><span data-stu-id="3a69d-121">settingValueTemplateId</span></span>|<span data-ttu-id="3a69d-122">String</span><span class="sxs-lookup"><span data-stu-id="3a69d-122">String</span></span>|<span data-ttu-id="3a69d-123">Настройка кода шаблона значений</span><span class="sxs-lookup"><span data-stu-id="3a69d-123">Setting Value Template Id</span></span>|

## <a name="relationships"></a><span data-ttu-id="3a69d-124">Связи</span><span class="sxs-lookup"><span data-stu-id="3a69d-124">Relationships</span></span>
<span data-ttu-id="3a69d-125">Нет</span><span class="sxs-lookup"><span data-stu-id="3a69d-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3a69d-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3a69d-126">JSON Representation</span></span>
<span data-ttu-id="3a69d-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3a69d-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValueTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationChoiceSettingValueTemplate",
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
          "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingValueTemplate",
          "settingValueTemplateId": "String"
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
              "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingValueTemplate",
              "settingValueTemplateId": "String"
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
              "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingValueTemplate",
              "settingValueTemplateId": "String"
            }
          }
        ]
      }
    ]
  },
  "settingValueTemplateId": "String"
}
```




