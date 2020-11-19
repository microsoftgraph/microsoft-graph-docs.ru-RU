---
title: Тип ресурса Девицеманажементконфигуратионсеттинг
description: Установка экземпляра в политике
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3767f7a9e21b72175f6df40dca78a0b2c0600b58
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242219"
---
# <a name="devicemanagementconfigurationsetting-resource-type"></a>Тип ресурса Девицеманажементконфигуратионсеттинг

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Установка экземпляра в политике

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицеманажементконфигуратионсеттингс](../api/intune-deviceconfigv2-devicemanagementconfigurationsetting-list.md)|Коллекция [девицеманажементконфигуратионсеттинг](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md)|Список свойств и связей объектов [девицеманажементконфигуратионсеттинг](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) .|
|[Получение Девицеманажементконфигуратионсеттинг](../api/intune-deviceconfigv2-devicemanagementconfigurationsetting-get.md)|[девицеманажементконфигуратионсеттинг](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md)|Чтение свойств и связей объекта [девицеманажементконфигуратионсеттинг](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) .|
|[Создание Девицеманажементконфигуратионсеттинг](../api/intune-deviceconfigv2-devicemanagementconfigurationsetting-create.md)|[девицеманажементконфигуратионсеттинг](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md)|Создание нового объекта [девицеманажементконфигуратионсеттинг](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) .|
|[Удаление Девицеманажементконфигуратионсеттинг](../api/intune-deviceconfigv2-devicemanagementconfigurationsetting-delete.md)|Нет|Удаляет объект [девицеманажементконфигуратионсеттинг](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md).|
|[Обновление Девицеманажементконфигуратионсеттинг](../api/intune-deviceconfigv2-devicemanagementconfigurationsetting-update.md)|[девицеманажементконфигуратионсеттинг](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md)|Обновление свойств объекта [девицеманажементконфигуратионсеттинг](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ этого параметра в политике, которая содержит его. Создается автоматически.|
|сеттингинстанце|[девицеманажементконфигуратионсеттингинстанце](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)|Установка экземпляра|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|сеттингдефинитионс|Коллекция [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|Список определений связанных параметров|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSetting",
  "id": "String (identifier)",
  "settingInstance": {
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
                                                                  "children": [
                                                                    {
                                                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                                      "settingDefinitionId": null,
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
}
```




