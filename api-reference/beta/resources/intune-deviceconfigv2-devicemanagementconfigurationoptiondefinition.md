---
title: Тип ресурса Девицеманажементконфигуратионоптиондефинитион
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5c8ccb388a8feb43b6be96402d45a5b7a0ae62ed
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242227"
---
# <a name="devicemanagementconfigurationoptiondefinition-resource-type"></a><span data-ttu-id="6cb78-103">Тип ресурса Девицеманажементконфигуратионоптиондефинитион</span><span class="sxs-lookup"><span data-stu-id="6cb78-103">deviceManagementConfigurationOptionDefinition resource type</span></span>

<span data-ttu-id="6cb78-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6cb78-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6cb78-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6cb78-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6cb78-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6cb78-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6cb78-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="6cb78-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="6cb78-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6cb78-108">Properties</span></span>
|<span data-ttu-id="6cb78-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="6cb78-109">Property</span></span>|<span data-ttu-id="6cb78-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6cb78-110">Type</span></span>|<span data-ttu-id="6cb78-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6cb78-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6cb78-112">optionValue</span><span class="sxs-lookup"><span data-stu-id="6cb78-112">optionValue</span></span>|[<span data-ttu-id="6cb78-113">девицеманажементконфигуратионсеттингвалуе</span><span class="sxs-lookup"><span data-stu-id="6cb78-113">deviceManagementConfigurationSettingValue</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)|<span data-ttu-id="6cb78-114">Значение параметра</span><span class="sxs-lookup"><span data-stu-id="6cb78-114">Value of the option</span></span>|
|<span data-ttu-id="6cb78-115">депендентон</span><span class="sxs-lookup"><span data-stu-id="6cb78-115">dependentOn</span></span>|<span data-ttu-id="6cb78-116">Коллекция [девицеманажементконфигуратиондепендентон](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md)</span><span class="sxs-lookup"><span data-stu-id="6cb78-116">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) collection</span></span>|<span data-ttu-id="6cb78-117">Список зависимых параметров для этого параметра</span><span class="sxs-lookup"><span data-stu-id="6cb78-117">List of dependent settings for this option</span></span>|
|<span data-ttu-id="6cb78-118">депендедонби</span><span class="sxs-lookup"><span data-stu-id="6cb78-118">dependedOnBy</span></span>|<span data-ttu-id="6cb78-119">Коллекция [девицеманажементконфигуратионсеттингдепендедонби](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md)</span><span class="sxs-lookup"><span data-stu-id="6cb78-119">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) collection</span></span>|<span data-ttu-id="6cb78-120">Список параметров, которые зависят от этого параметра</span><span class="sxs-lookup"><span data-stu-id="6cb78-120">List of Settings that depends on this option</span></span>|
|<span data-ttu-id="6cb78-121">itemId</span><span class="sxs-lookup"><span data-stu-id="6cb78-121">itemId</span></span>|<span data-ttu-id="6cb78-122">String</span><span class="sxs-lookup"><span data-stu-id="6cb78-122">String</span></span>|<span data-ttu-id="6cb78-123">Идентификатор параметра</span><span class="sxs-lookup"><span data-stu-id="6cb78-123">Identifier of option</span></span>|
|<span data-ttu-id="6cb78-124">description</span><span class="sxs-lookup"><span data-stu-id="6cb78-124">description</span></span>|<span data-ttu-id="6cb78-125">String</span><span class="sxs-lookup"><span data-stu-id="6cb78-125">String</span></span>|<span data-ttu-id="6cb78-126">Описание параметра</span><span class="sxs-lookup"><span data-stu-id="6cb78-126">Description of the option</span></span>|
|<span data-ttu-id="6cb78-127">helpText</span><span class="sxs-lookup"><span data-stu-id="6cb78-127">helpText</span></span>|<span data-ttu-id="6cb78-128">String</span><span class="sxs-lookup"><span data-stu-id="6cb78-128">String</span></span>|<span data-ttu-id="6cb78-129">Текст справки для параметра</span><span class="sxs-lookup"><span data-stu-id="6cb78-129">Help text of the option</span></span>|
|<span data-ttu-id="6cb78-130">name</span><span class="sxs-lookup"><span data-stu-id="6cb78-130">name</span></span>|<span data-ttu-id="6cb78-131">String</span><span class="sxs-lookup"><span data-stu-id="6cb78-131">String</span></span>|<span data-ttu-id="6cb78-132">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="6cb78-132">Name of the option</span></span>|
|<span data-ttu-id="6cb78-133">displayName</span><span class="sxs-lookup"><span data-stu-id="6cb78-133">displayName</span></span>|<span data-ttu-id="6cb78-134">String</span><span class="sxs-lookup"><span data-stu-id="6cb78-134">String</span></span>|<span data-ttu-id="6cb78-135">Понятное имя параметра</span><span class="sxs-lookup"><span data-stu-id="6cb78-135">Friendly name of the option</span></span>|

## <a name="relationships"></a><span data-ttu-id="6cb78-136">Связи</span><span class="sxs-lookup"><span data-stu-id="6cb78-136">Relationships</span></span>
<span data-ttu-id="6cb78-137">Нет</span><span class="sxs-lookup"><span data-stu-id="6cb78-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6cb78-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6cb78-138">JSON Representation</span></span>
<span data-ttu-id="6cb78-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6cb78-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationOptionDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationOptionDefinition",
  "optionValue": {
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
  },
  "dependentOn": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationDependentOn",
      "dependentOn": "String",
      "parentSettingId": "String"
    }
  ],
  "dependedOnBy": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingDependedOnBy",
      "dependedOnBy": "String",
      "required": true
    }
  ],
  "itemId": "String",
  "description": "String",
  "helpText": "String",
  "name": "String",
  "displayName": "String"
}
```




