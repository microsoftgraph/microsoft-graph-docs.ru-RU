---
title: Тип ресурса Девицеманажементконфигуратионграупсеттингинстанце
description: Экземпляр объекта GroupSetting
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bb5105acb3e975811400bd9784803c97db0c5370
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242248"
---
# <a name="devicemanagementconfigurationgroupsettinginstance-resource-type"></a><span data-ttu-id="dc390-103">Тип ресурса Девицеманажементконфигуратионграупсеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="dc390-103">deviceManagementConfigurationGroupSettingInstance resource type</span></span>

<span data-ttu-id="dc390-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc390-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dc390-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc390-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dc390-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dc390-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc390-107">Экземпляр объекта GroupSetting</span><span class="sxs-lookup"><span data-stu-id="dc390-107">Instance of a GroupSetting</span></span>


<span data-ttu-id="dc390-108">Наследуется от [девицеманажементконфигуратионсеттингинстанце](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="dc390-108">Inherits from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>

## <a name="properties"></a><span data-ttu-id="dc390-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="dc390-109">Properties</span></span>
|<span data-ttu-id="dc390-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="dc390-110">Property</span></span>|<span data-ttu-id="dc390-111">Тип</span><span class="sxs-lookup"><span data-stu-id="dc390-111">Type</span></span>|<span data-ttu-id="dc390-112">Описание</span><span class="sxs-lookup"><span data-stu-id="dc390-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc390-113">сеттингдефинитионид</span><span class="sxs-lookup"><span data-stu-id="dc390-113">settingDefinitionId</span></span>|<span data-ttu-id="dc390-114">String</span><span class="sxs-lookup"><span data-stu-id="dc390-114">String</span></span>|<span data-ttu-id="dc390-115">Параметр ID определения, наследуемый от [девицеманажементконфигуратионсеттингинстанце](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="dc390-115">Setting Definition Id Inherited from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>|
|<span data-ttu-id="dc390-116">граупсеттингвалуе</span><span class="sxs-lookup"><span data-stu-id="dc390-116">groupSettingValue</span></span>|[<span data-ttu-id="dc390-117">девицеманажементконфигуратионграупсеттингвалуе</span><span class="sxs-lookup"><span data-stu-id="dc390-117">deviceManagementConfigurationGroupSettingValue</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationgroupsettingvalue.md)|<span data-ttu-id="dc390-118">Значение GroupSetting</span><span class="sxs-lookup"><span data-stu-id="dc390-118">GroupSetting value</span></span>|

## <a name="relationships"></a><span data-ttu-id="dc390-119">Связи</span><span class="sxs-lookup"><span data-stu-id="dc390-119">Relationships</span></span>
<span data-ttu-id="dc390-120">Нет</span><span class="sxs-lookup"><span data-stu-id="dc390-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dc390-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dc390-121">JSON Representation</span></span>
<span data-ttu-id="dc390-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dc390-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationGroupSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationGroupSettingInstance",
  "settingDefinitionId": "String",
  "groupSettingValue": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationGroupSettingValue",
    "children": [
      {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
        "settingDefinitionId": "String",
        "choiceSettingValue": {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
          "value": "String",
          "children": [
            {
              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
              "settingDefinitionId": "String",
              "choiceSettingValue": {
                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                "value": "String",
                "children": [
                  {
                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                    "settingDefinitionId": "String",
                    "choiceSettingValue": {
                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                      "value": "String",
                      "children": [
                        {
                          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                          "settingDefinitionId": "String",
                          "choiceSettingValue": {
                            "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                            "value": "String",
                            "children": [
                              {
                                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                "settingDefinitionId": "String",
                                "choiceSettingValue": {
                                  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                  "value": "String",
                                  "children": [
                                    {
                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                      "settingDefinitionId": "String",
                                      "choiceSettingValue": {
                                        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                        "value": "String",
                                        "children": [
                                          {
                                            "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                            "settingDefinitionId": "String",
                                            "choiceSettingValue": {
                                              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                              "value": "String",
                                              "children": [
                                                {
                                                  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                  "settingDefinitionId": "String",
                                                  "choiceSettingValue": {
                                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                    "value": "String",
                                                    "children": [
                                                      {
                                                        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                        "settingDefinitionId": "String",
                                                        "choiceSettingValue": {
                                                          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                          "value": "String",
                                                          "children": [
                                                            {
                                                              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                              "settingDefinitionId": "String",
                                                              "choiceSettingValue": {
                                                                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                                "value": "String",
                                                                "children": [
                                                                  {
                                                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                                    "settingDefinitionId": "String",
                                                                    "choiceSettingValue": {
                                                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                                      "value": "String",
                                                                      "children": null
                                                                    }
                                                                  }
                                                                ]
                                                              }
                                                            }
                                                          ]
                                                        }
                                                      }
                                                    ]
                                                  }
                                                }
                                              ]
                                            }
                                          }
                                        ]
                                      }
                                    }
                                  ]
                                }
                              }
                            ]
                          }
                        }
                      ]
                    }
                  }
                ]
              }
            }
          ]
        }
      }
    ]
  }
}
```




