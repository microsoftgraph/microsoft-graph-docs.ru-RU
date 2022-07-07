---
title: Тип ресурса deviceManagementReusablePolicySetting
description: Модель графа для повторно используемого параметра
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 14d464d334432eda7c779bb80d636c7b9be3416d
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2022
ms.locfileid: "66670837"
---
# <a name="devicemanagementreusablepolicysetting-resource-type"></a>Тип ресурса deviceManagementReusablePolicySetting

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Модель графа для повторно используемого параметра

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление deviceManagementReusablePolicySettings](../api/intune-deviceconfigv2-devicemanagementreusablepolicysetting-list.md)|[Коллекция deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md)|Список свойств и связей объектов [deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md) .|
|[Получение объекта deviceManagementReusablePolicySetting](../api/intune-deviceconfigv2-devicemanagementreusablepolicysetting-get.md)|[deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md)|Чтение свойств и связей объекта [deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md) .|
|[Создание объекта deviceManagementReusablePolicySetting](../api/intune-deviceconfigv2-devicemanagementreusablepolicysetting-create.md)|[deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md)|Создайте объект [deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md) .|
|[Удаление объекта deviceManagementReusablePolicySetting](../api/intune-deviceconfigv2-devicemanagementreusablepolicysetting-delete.md)|Нет|Удаляет [объект deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md).|
|[Обновление объекта deviceManagementReusablePolicySetting](../api/intune-deviceconfigv2-devicemanagementreusablepolicysetting-update.md)|[deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md)|Обновление свойств объекта [deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md) .|
|[Действие клонирования](../api/intune-deviceconfigv2-devicemanagementreusablepolicysetting-clone.md)|[deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|созданный системой идентификатор многократно используемого параметра.|
|displayName|String|отображаемое имя параметра многократного использования, предоставленное пользователем.|
|description|String|многократно используемое описание параметра, предоставленное пользователем.|
|settingDefinitionId|String|идентификатор определения параметра, связанный с этим повторно используемым параметром.|
|settingInstance|[deviceManagementConfigurationSettingInstance](../resources/intune-shared-devicemanagementconfigurationsettinginstance.md)|Повторно используемый экземпляр конфигурации параметров|
|createdDateTime|DateTimeOffset|многократно используемые параметры даты и времени создания. Это свойство доступно только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения параметра многократного использования. Это свойство доступно только для чтения.|
|version|Int32|номер версии для параметра многократного использования. Допустимые значения от 0 до 2147483647. Это свойство доступно только для чтения.|
|referencingConfigurationPolicyCount|Int32|число политик конфигурации, ссылаемых на текущий параметр многократного использования. Допустимые значения от 0 до 2147483647. Это свойство доступно только для чтения.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|referencingConfigurationPolicies|[Коллекция deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md)|политики конфигурации, ссылаясь на текущий параметр многократного использования. Это свойство доступно только для чтения.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementReusablePolicySetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementReusablePolicySetting",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "settingDefinitionId": "String",
  "settingInstance": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
    "settingDefinitionId": "String",
    "settingInstanceTemplateReference": {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
      "settingInstanceTemplateId": "String"
    },
    "choiceSettingValue": {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
      "settingValueTemplateReference": {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
        "settingValueTemplateId": "String",
        "useTemplateDefault": true
      },
      "value": "String",
      "children": [
        {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
          "settingDefinitionId": "String",
          "settingInstanceTemplateReference": {
            "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
            "settingInstanceTemplateId": "String"
          },
          "choiceSettingValue": {
            "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
            "settingValueTemplateReference": {
              "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
              "settingValueTemplateId": "String",
              "useTemplateDefault": true
            },
            "value": "String",
            "children": [
              {
                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                "settingDefinitionId": "String",
                "settingInstanceTemplateReference": {
                  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
                  "settingInstanceTemplateId": "String"
                },
                "choiceSettingValue": {
                  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                  "settingValueTemplateReference": {
                    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
                    "settingValueTemplateId": "String",
                    "useTemplateDefault": true
                  },
                  "value": "String",
                  "children": [
                    {
                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                      "settingDefinitionId": "String",
                      "settingInstanceTemplateReference": {
                        "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
                        "settingInstanceTemplateId": "String"
                      },
                      "choiceSettingValue": {
                        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                        "settingValueTemplateReference": {
                          "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
                          "settingValueTemplateId": "String",
                          "useTemplateDefault": true
                        },
                        "value": "String",
                        "children": [
                          {
                            "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                            "settingDefinitionId": "String",
                            "settingInstanceTemplateReference": {
                              "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
                              "settingInstanceTemplateId": "String"
                            },
                            "choiceSettingValue": {
                              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                              "settingValueTemplateReference": {
                                "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
                                "settingValueTemplateId": "String",
                                "useTemplateDefault": true
                              },
                              "value": "String",
                              "children": [
                                {
                                  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                  "settingDefinitionId": "String",
                                  "settingInstanceTemplateReference": {
                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
                                    "settingInstanceTemplateId": "String"
                                  },
                                  "choiceSettingValue": {
                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                    "settingValueTemplateReference": {
                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
                                      "settingValueTemplateId": "String",
                                      "useTemplateDefault": true
                                    },
                                    "value": "String",
                                    "children": [
                                      {
                                        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                        "settingDefinitionId": "String",
                                        "settingInstanceTemplateReference": {
                                          "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
                                          "settingInstanceTemplateId": "String"
                                        },
                                        "choiceSettingValue": {
                                          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                          "settingValueTemplateReference": {
                                            "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
                                            "settingValueTemplateId": "String",
                                            "useTemplateDefault": true
                                          },
                                          "value": "String",
                                          "children": [
                                            {
                                              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                              "settingDefinitionId": "String",
                                              "settingInstanceTemplateReference": {
                                                "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
                                                "settingInstanceTemplateId": "String"
                                              },
                                              "choiceSettingValue": {
                                                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                "settingValueTemplateReference": {
                                                  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
                                                  "settingValueTemplateId": "String",
                                                  "useTemplateDefault": true
                                                },
                                                "value": "String",
                                                "children": [
                                                  {
                                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                    "settingDefinitionId": "String",
                                                    "settingInstanceTemplateReference": {
                                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
                                                      "settingInstanceTemplateId": "String"
                                                    },
                                                    "choiceSettingValue": {
                                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                      "settingValueTemplateReference": {
                                                        "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
                                                        "settingValueTemplateId": "String",
                                                        "useTemplateDefault": true
                                                      },
                                                      "value": "String",
                                                      "children": [
                                                        {
                                                          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                          "settingDefinitionId": "String",
                                                          "settingInstanceTemplateReference": {
                                                            "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
                                                            "settingInstanceTemplateId": "String"
                                                          },
                                                          "choiceSettingValue": {
                                                            "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                            "settingValueTemplateReference": {
                                                              "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
                                                              "settingValueTemplateId": "String",
                                                              "useTemplateDefault": true
                                                            },
                                                            "value": "String",
                                                            "children": [
                                                              {
                                                                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                                "settingDefinitionId": "String",
                                                                "settingInstanceTemplateReference": {
                                                                  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
                                                                  "settingInstanceTemplateId": "String"
                                                                },
                                                                "choiceSettingValue": {
                                                                  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                                  "settingValueTemplateReference": {
                                                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
                                                                    "settingValueTemplateId": "String",
                                                                    "useTemplateDefault": true
                                                                  },
                                                                  "value": "String",
                                                                  "children": [
                                                                    {
                                                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                                      "settingDefinitionId": null,
                                                                      "settingInstanceTemplateReference": null,
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
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": 1024,
  "referencingConfigurationPolicyCount": 1024
}
```




