---
title: Тип ресурса Девицеманажементконфигуратионграупсеттингвалуе
description: Значение GroupSetting
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a4c21b07f2e180f7c12a8f0df8e208f14a67cb6b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242236"
---
# <a name="devicemanagementconfigurationgroupsettingvalue-resource-type"></a><span data-ttu-id="57ea0-103">Тип ресурса Девицеманажементконфигуратионграупсеттингвалуе</span><span class="sxs-lookup"><span data-stu-id="57ea0-103">deviceManagementConfigurationGroupSettingValue resource type</span></span>

<span data-ttu-id="57ea0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57ea0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="57ea0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57ea0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57ea0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="57ea0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57ea0-107">Значение GroupSetting</span><span class="sxs-lookup"><span data-stu-id="57ea0-107">Value of the GroupSetting</span></span>


<span data-ttu-id="57ea0-108">Наследуется от [девицеманажементконфигуратионсеттингвалуе](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="57ea0-108">Inherits from [deviceManagementConfigurationSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)</span></span>

## <a name="properties"></a><span data-ttu-id="57ea0-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="57ea0-109">Properties</span></span>
|<span data-ttu-id="57ea0-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="57ea0-110">Property</span></span>|<span data-ttu-id="57ea0-111">Тип</span><span class="sxs-lookup"><span data-stu-id="57ea0-111">Type</span></span>|<span data-ttu-id="57ea0-112">Описание</span><span class="sxs-lookup"><span data-stu-id="57ea0-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57ea0-113">children</span><span class="sxs-lookup"><span data-stu-id="57ea0-113">children</span></span>|<span data-ttu-id="57ea0-114">Коллекция [девицеманажементконфигуратионсеттингинстанце](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="57ea0-114">[deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md) collection</span></span>|<span data-ttu-id="57ea0-115">Коллекция экземпляров дочерних параметров, содержащихся в этом GroupSetting</span><span class="sxs-lookup"><span data-stu-id="57ea0-115">Collection of child setting instances contained within this GroupSetting</span></span>|

## <a name="relationships"></a><span data-ttu-id="57ea0-116">Связи</span><span class="sxs-lookup"><span data-stu-id="57ea0-116">Relationships</span></span>
<span data-ttu-id="57ea0-117">Нет</span><span class="sxs-lookup"><span data-stu-id="57ea0-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="57ea0-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="57ea0-118">JSON Representation</span></span>
<span data-ttu-id="57ea0-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="57ea0-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationGroupSettingValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationGroupSettingValue",
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
```




