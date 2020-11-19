---
title: Тип ресурса Девицеманажементконфигуратиончоицесеттингколлектионинстанце
description: Установка экземпляра в политике
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c184daa530de199afc5240b42cbcb1d8204f96df
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242267"
---
# <a name="devicemanagementconfigurationchoicesettingcollectioninstance-resource-type"></a><span data-ttu-id="8cc0d-103">Тип ресурса Девицеманажементконфигуратиончоицесеттингколлектионинстанце</span><span class="sxs-lookup"><span data-stu-id="8cc0d-103">deviceManagementConfigurationChoiceSettingCollectionInstance resource type</span></span>

<span data-ttu-id="8cc0d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8cc0d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8cc0d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8cc0d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8cc0d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8cc0d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8cc0d-107">Установка экземпляра в политике</span><span class="sxs-lookup"><span data-stu-id="8cc0d-107">Setting instance within policy</span></span>


<span data-ttu-id="8cc0d-108">Наследуется от [девицеманажементконфигуратионсеттингинстанце](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="8cc0d-108">Inherits from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8cc0d-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="8cc0d-109">Properties</span></span>
|<span data-ttu-id="8cc0d-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="8cc0d-110">Property</span></span>|<span data-ttu-id="8cc0d-111">Тип</span><span class="sxs-lookup"><span data-stu-id="8cc0d-111">Type</span></span>|<span data-ttu-id="8cc0d-112">Описание</span><span class="sxs-lookup"><span data-stu-id="8cc0d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8cc0d-113">сеттингдефинитионид</span><span class="sxs-lookup"><span data-stu-id="8cc0d-113">settingDefinitionId</span></span>|<span data-ttu-id="8cc0d-114">String</span><span class="sxs-lookup"><span data-stu-id="8cc0d-114">String</span></span>|<span data-ttu-id="8cc0d-115">Параметр ID определения, наследуемый от [девицеманажементконфигуратионсеттингинстанце](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="8cc0d-115">Setting Definition Id Inherited from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>|
|<span data-ttu-id="8cc0d-116">чоицесеттингколлектионвалуе</span><span class="sxs-lookup"><span data-stu-id="8cc0d-116">choiceSettingCollectionValue</span></span>|<span data-ttu-id="8cc0d-117">Коллекция [девицеманажементконфигуратиончоицесеттингвалуе](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="8cc0d-117">[deviceManagementConfigurationChoiceSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingvalue.md) collection</span></span>|<span data-ttu-id="8cc0d-118">Значение коллекции параметров Choice</span><span class="sxs-lookup"><span data-stu-id="8cc0d-118">Choice setting collection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="8cc0d-119">Связи</span><span class="sxs-lookup"><span data-stu-id="8cc0d-119">Relationships</span></span>
<span data-ttu-id="8cc0d-120">Нет</span><span class="sxs-lookup"><span data-stu-id="8cc0d-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8cc0d-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8cc0d-121">JSON Representation</span></span>
<span data-ttu-id="8cc0d-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8cc0d-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingCollectionInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationChoiceSettingCollectionInstance",
  "settingDefinitionId": "String",
  "choiceSettingCollectionValue": [
    {
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
                                                                  "children": [
                                                                    {
                                                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                                      "settingDefinitionId": "String",
                                                                      "choiceSettingValue": {
                                                                        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                                        "value": null,
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




