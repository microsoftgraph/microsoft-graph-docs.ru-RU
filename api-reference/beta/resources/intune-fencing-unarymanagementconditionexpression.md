---
title: тип ресурса unaryManagementConditionExpression
description: Выражение состояния управления, которое оценивается с помощью безоценной операции.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2a3aa2c001c08e3d315e65fd0d7911d4f557c3becab7a4a9be4a2826c2313375
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54152994"
---
# <a name="unarymanagementconditionexpression-resource-type"></a>тип ресурса unaryManagementConditionExpression

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Выражение состояния управления, которое оценивается с помощью безоценной операции.


Наследует от [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|operator|[unaryManagementConditionExpressionOperatorType](../resources/intune-fencing-unarymanagementconditionexpressionoperatortype.md)|Оператор, используемый при оценке безоценной операции. Возможные значения: `not` .|
|operand|[managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)|Операнд операции без операции.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.unaryManagementConditionExpression"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unaryManagementConditionExpression",
  "operator": "String",
  "operand": {
    "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
    "operator": "String",
    "firstOperand": {
      "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
      "operator": "String",
      "firstOperand": {
        "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
        "operator": "String",
        "firstOperand": {
          "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
          "operator": "String",
          "firstOperand": {
            "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
            "operator": "String",
            "firstOperand": {
              "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
              "operator": "String",
              "firstOperand": {
                "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                "operator": "String",
                "firstOperand": {
                  "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                  "operator": "String",
                  "firstOperand": {
                    "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                    "operator": "String",
                    "firstOperand": {
                      "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                      "operator": "String",
                      "firstOperand": {
                        "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                        "operator": "String",
                        "firstOperand": {
                          "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                          "operator": null,
                          "firstOperand": null,
                          "secondOperand": {
                            "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                            "operator": null,
                            "firstOperand": null,
                            "secondOperand": {
                              "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                              "operator": null,
                              "firstOperand": null,
                              "secondOperand": {
                                "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                                "operator": null,
                                "firstOperand": null,
                                "secondOperand": {
                                  "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                                  "operator": null,
                                  "firstOperand": null,
                                  "secondOperand": {
                                    "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                                    "operator": null,
                                    "firstOperand": null,
                                    "secondOperand": {
                                      "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                                      "operator": null,
                                      "firstOperand": null,
                                      "secondOperand": {
                                        "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                                        "operator": null,
                                        "firstOperand": null,
                                        "secondOperand": {
                                          "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                                          "operator": null,
                                          "firstOperand": null,
                                          "secondOperand": {
                                            "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                                            "operator": null,
                                            "firstOperand": null,
                                            "secondOperand": {
                                              "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                                              "operator": null,
                                              "firstOperand": null,
                                              "secondOperand": {
                                                "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                                                "operator": null,
                                                "firstOperand": null,
                                                "secondOperand": null
                                              }
                                            }
                                          }
                                        }
                                      }
                                    }
                                  }
                                }
                              }
                            }
                          }
                        },
                        "secondOperand": null
                      },
                      "secondOperand": null
                    },
                    "secondOperand": null
                  },
                  "secondOperand": null
                },
                "secondOperand": null
              },
              "secondOperand": null
            },
            "secondOperand": null
          },
          "secondOperand": null
        },
        "secondOperand": null
      },
      "secondOperand": null
    },
    "secondOperand": null
  }
}
```




