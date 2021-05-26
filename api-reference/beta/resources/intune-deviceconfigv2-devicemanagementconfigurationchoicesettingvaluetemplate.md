---
title: тип ресурса deviceManagementConfigurationChoiceSettingValueTemplate
description: Шаблон параметра параметра выбор
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 10d446532e0664c6d83d16d223c0a8e0d966aeb4
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666578"
---
# <a name="devicemanagementconfigurationchoicesettingvaluetemplate-resource-type"></a><span data-ttu-id="d70f8-103">тип ресурса deviceManagementConfigurationChoiceSettingValueTemplate</span><span class="sxs-lookup"><span data-stu-id="d70f8-103">deviceManagementConfigurationChoiceSettingValueTemplate resource type</span></span>

<span data-ttu-id="d70f8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d70f8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d70f8-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d70f8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d70f8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d70f8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d70f8-107">Шаблон параметра параметра выбор</span><span class="sxs-lookup"><span data-stu-id="d70f8-107">Choice Setting Value Template</span></span>

## <a name="properties"></a><span data-ttu-id="d70f8-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d70f8-108">Properties</span></span>
|<span data-ttu-id="d70f8-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d70f8-109">Property</span></span>|<span data-ttu-id="d70f8-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d70f8-110">Type</span></span>|<span data-ttu-id="d70f8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d70f8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d70f8-112">defaultValue</span><span class="sxs-lookup"><span data-stu-id="d70f8-112">defaultValue</span></span>|[<span data-ttu-id="d70f8-113">deviceManagementConfigurationChoiceSettingValueDefaultTemplate</span><span class="sxs-lookup"><span data-stu-id="d70f8-113">deviceManagementConfigurationChoiceSettingValueDefaultTemplate</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingvaluedefaulttemplate.md)|<span data-ttu-id="d70f8-114">Шаблон параметра параметра значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="d70f8-114">Choice Setting Value Default Template.</span></span>|
|<span data-ttu-id="d70f8-115">recommendedValueDefinition</span><span class="sxs-lookup"><span data-stu-id="d70f8-115">recommendedValueDefinition</span></span>|[<span data-ttu-id="d70f8-116">deviceManagementConfigurationChoiceSettingValueDefinitionTemplate</span><span class="sxs-lookup"><span data-stu-id="d70f8-116">deviceManagementConfigurationChoiceSettingValueDefinitionTemplate</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingvaluedefinitiontemplate.md)|<span data-ttu-id="d70f8-117">Рекомендуемые переопределения определения.</span><span class="sxs-lookup"><span data-stu-id="d70f8-117">Recommended definition override.</span></span>|
|<span data-ttu-id="d70f8-118">requiredValueDefinition</span><span class="sxs-lookup"><span data-stu-id="d70f8-118">requiredValueDefinition</span></span>|[<span data-ttu-id="d70f8-119">deviceManagementConfigurationChoiceSettingValueDefinitionTemplate</span><span class="sxs-lookup"><span data-stu-id="d70f8-119">deviceManagementConfigurationChoiceSettingValueDefinitionTemplate</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingvaluedefinitiontemplate.md)|<span data-ttu-id="d70f8-120">Обязательное переопределения определения.</span><span class="sxs-lookup"><span data-stu-id="d70f8-120">Required definition override.</span></span>|
|<span data-ttu-id="d70f8-121">settingValueTemplateId</span><span class="sxs-lookup"><span data-stu-id="d70f8-121">settingValueTemplateId</span></span>|<span data-ttu-id="d70f8-122">Строка</span><span class="sxs-lookup"><span data-stu-id="d70f8-122">String</span></span>|<span data-ttu-id="d70f8-123">Настройка кода шаблона значений</span><span class="sxs-lookup"><span data-stu-id="d70f8-123">Setting Value Template Id</span></span>|

## <a name="relationships"></a><span data-ttu-id="d70f8-124">Связи</span><span class="sxs-lookup"><span data-stu-id="d70f8-124">Relationships</span></span>
<span data-ttu-id="d70f8-125">Нет</span><span class="sxs-lookup"><span data-stu-id="d70f8-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d70f8-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d70f8-126">JSON Representation</span></span>
<span data-ttu-id="d70f8-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d70f8-127">Here is a JSON representation of the resource.</span></span>
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
```




