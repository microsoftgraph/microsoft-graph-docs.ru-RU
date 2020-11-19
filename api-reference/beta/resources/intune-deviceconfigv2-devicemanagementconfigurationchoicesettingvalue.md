---
title: Тип ресурса Девицеманажементконфигуратиончоицесеттингвалуе
description: Значение параметра
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d7b57e1cb62feb48073207275c249796a2474294
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242260"
---
# <a name="devicemanagementconfigurationchoicesettingvalue-resource-type"></a><span data-ttu-id="e2ca4-103">Тип ресурса Девицеманажементконфигуратиончоицесеттингвалуе</span><span class="sxs-lookup"><span data-stu-id="e2ca4-103">deviceManagementConfigurationChoiceSettingValue resource type</span></span>

<span data-ttu-id="e2ca4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2ca4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e2ca4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2ca4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2ca4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e2ca4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2ca4-107">Значение параметра</span><span class="sxs-lookup"><span data-stu-id="e2ca4-107">Setting value</span></span>


<span data-ttu-id="e2ca4-108">Наследуется от [девицеманажементконфигуратионсеттингвалуе](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="e2ca4-108">Inherits from [deviceManagementConfigurationSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e2ca4-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="e2ca4-109">Properties</span></span>
|<span data-ttu-id="e2ca4-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="e2ca4-110">Property</span></span>|<span data-ttu-id="e2ca4-111">Тип</span><span class="sxs-lookup"><span data-stu-id="e2ca4-111">Type</span></span>|<span data-ttu-id="e2ca4-112">Описание</span><span class="sxs-lookup"><span data-stu-id="e2ca4-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2ca4-113">значение</span><span class="sxs-lookup"><span data-stu-id="e2ca4-113">value</span></span>|<span data-ttu-id="e2ca4-114">String</span><span class="sxs-lookup"><span data-stu-id="e2ca4-114">String</span></span>|<span data-ttu-id="e2ca4-115">Значение параметра Choice: Оптиондефинитион ItemId.</span><span class="sxs-lookup"><span data-stu-id="e2ca4-115">Choice setting value: an OptionDefinition ItemId.</span></span>|
|<span data-ttu-id="e2ca4-116">children</span><span class="sxs-lookup"><span data-stu-id="e2ca4-116">children</span></span>|<span data-ttu-id="e2ca4-117">Коллекция [девицеманажементконфигуратионсеттингинстанце](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="e2ca4-117">[deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md) collection</span></span>|<span data-ttu-id="e2ca4-118">Параметры дочернего элемента.</span><span class="sxs-lookup"><span data-stu-id="e2ca4-118">Child settings.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2ca4-119">Связи</span><span class="sxs-lookup"><span data-stu-id="e2ca4-119">Relationships</span></span>
<span data-ttu-id="e2ca4-120">Нет</span><span class="sxs-lookup"><span data-stu-id="e2ca4-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e2ca4-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e2ca4-121">JSON Representation</span></span>
<span data-ttu-id="e2ca4-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e2ca4-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
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




