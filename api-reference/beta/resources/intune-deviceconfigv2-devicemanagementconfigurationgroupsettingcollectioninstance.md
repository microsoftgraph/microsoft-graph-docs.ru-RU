---
title: Тип ресурса Девицеманажементконфигуратионграупсеттингколлектионинстанце
description: Экземпляр объекта Граупсеттингколлектион
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 40542c7358838f60bfeb30d8e938062fbbc2c7b0
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242251"
---
# <a name="devicemanagementconfigurationgroupsettingcollectioninstance-resource-type"></a><span data-ttu-id="f8653-103">Тип ресурса Девицеманажементконфигуратионграупсеттингколлектионинстанце</span><span class="sxs-lookup"><span data-stu-id="f8653-103">deviceManagementConfigurationGroupSettingCollectionInstance resource type</span></span>

<span data-ttu-id="f8653-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8653-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f8653-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8653-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f8653-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f8653-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8653-107">Экземпляр объекта Граупсеттингколлектион</span><span class="sxs-lookup"><span data-stu-id="f8653-107">Instance of a GroupSettingCollection</span></span>


<span data-ttu-id="f8653-108">Наследуется от [девицеманажементконфигуратионсеттингинстанце](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="f8653-108">Inherits from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f8653-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="f8653-109">Properties</span></span>
|<span data-ttu-id="f8653-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="f8653-110">Property</span></span>|<span data-ttu-id="f8653-111">Тип</span><span class="sxs-lookup"><span data-stu-id="f8653-111">Type</span></span>|<span data-ttu-id="f8653-112">Описание</span><span class="sxs-lookup"><span data-stu-id="f8653-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8653-113">сеттингдефинитионид</span><span class="sxs-lookup"><span data-stu-id="f8653-113">settingDefinitionId</span></span>|<span data-ttu-id="f8653-114">String</span><span class="sxs-lookup"><span data-stu-id="f8653-114">String</span></span>|<span data-ttu-id="f8653-115">Параметр ID определения, наследуемый от [девицеманажементконфигуратионсеттингинстанце](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="f8653-115">Setting Definition Id Inherited from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>|
|<span data-ttu-id="f8653-116">граупсеттингколлектионвалуе</span><span class="sxs-lookup"><span data-stu-id="f8653-116">groupSettingCollectionValue</span></span>|<span data-ttu-id="f8653-117">Коллекция [девицеманажементконфигуратионграупсеттингвалуе](../resources/intune-deviceconfigv2-devicemanagementconfigurationgroupsettingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="f8653-117">[deviceManagementConfigurationGroupSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationgroupsettingvalue.md) collection</span></span>|<span data-ttu-id="f8653-118">Коллекция значений GroupSetting</span><span class="sxs-lookup"><span data-stu-id="f8653-118">A collection of GroupSetting values</span></span>|

## <a name="relationships"></a><span data-ttu-id="f8653-119">Связи</span><span class="sxs-lookup"><span data-stu-id="f8653-119">Relationships</span></span>
<span data-ttu-id="f8653-120">Нет</span><span class="sxs-lookup"><span data-stu-id="f8653-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f8653-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f8653-121">JSON Representation</span></span>
<span data-ttu-id="f8653-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f8653-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationGroupSettingCollectionInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationGroupSettingCollectionInstance",
  "settingDefinitionId": "String",
  "groupSettingCollectionValue": [
    {
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
  ]
}
```




