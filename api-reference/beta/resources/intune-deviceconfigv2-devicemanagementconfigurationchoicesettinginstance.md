---
title: Тип ресурса Девицеманажементконфигуратиончоицесеттингинстанце
description: Установка экземпляра в политике
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 591c99a1089a9a01acb6b4ded72439f98d3afbb1
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242263"
---
# <a name="devicemanagementconfigurationchoicesettinginstance-resource-type"></a><span data-ttu-id="b036b-103">Тип ресурса Девицеманажементконфигуратиончоицесеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="b036b-103">deviceManagementConfigurationChoiceSettingInstance resource type</span></span>

<span data-ttu-id="b036b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b036b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b036b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b036b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b036b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b036b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b036b-107">Установка экземпляра в политике</span><span class="sxs-lookup"><span data-stu-id="b036b-107">Setting instance within policy</span></span>


<span data-ttu-id="b036b-108">Наследуется от [девицеманажементконфигуратионсеттингинстанце](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="b036b-108">Inherits from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b036b-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="b036b-109">Properties</span></span>
|<span data-ttu-id="b036b-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="b036b-110">Property</span></span>|<span data-ttu-id="b036b-111">Тип</span><span class="sxs-lookup"><span data-stu-id="b036b-111">Type</span></span>|<span data-ttu-id="b036b-112">Описание</span><span class="sxs-lookup"><span data-stu-id="b036b-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b036b-113">сеттингдефинитионид</span><span class="sxs-lookup"><span data-stu-id="b036b-113">settingDefinitionId</span></span>|<span data-ttu-id="b036b-114">String</span><span class="sxs-lookup"><span data-stu-id="b036b-114">String</span></span>|<span data-ttu-id="b036b-115">Параметр ID определения, наследуемый от [девицеманажементконфигуратионсеттингинстанце](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="b036b-115">Setting Definition Id Inherited from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>|
|<span data-ttu-id="b036b-116">чоицесеттингвалуе</span><span class="sxs-lookup"><span data-stu-id="b036b-116">choiceSettingValue</span></span>|[<span data-ttu-id="b036b-117">девицеманажементконфигуратиончоицесеттингвалуе</span><span class="sxs-lookup"><span data-stu-id="b036b-117">deviceManagementConfigurationChoiceSettingValue</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingvalue.md)|<span data-ttu-id="b036b-118">Значение параметра Choice</span><span class="sxs-lookup"><span data-stu-id="b036b-118">Choice setting value</span></span>|

## <a name="relationships"></a><span data-ttu-id="b036b-119">Связи</span><span class="sxs-lookup"><span data-stu-id="b036b-119">Relationships</span></span>
<span data-ttu-id="b036b-120">Нет</span><span class="sxs-lookup"><span data-stu-id="b036b-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b036b-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b036b-121">JSON Representation</span></span>
<span data-ttu-id="b036b-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b036b-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
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
                                                                "children": [
                                                                  {
                                                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                                    "settingDefinitionId": "String",
                                                                    "choiceSettingValue": null
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




