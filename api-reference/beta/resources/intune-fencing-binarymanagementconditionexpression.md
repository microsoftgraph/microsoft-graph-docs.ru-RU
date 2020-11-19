---
title: Тип ресурса Бинариманажементкондитионекспрессион
description: Выражение условия управления, вычисляемое с помощью бинарной операции.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b7f8efa0bba16a9567258449e42b5d3e8ed28dab
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49299087"
---
# <a name="binarymanagementconditionexpression-resource-type"></a><span data-ttu-id="8c8dd-103">Тип ресурса Бинариманажементкондитионекспрессион</span><span class="sxs-lookup"><span data-stu-id="8c8dd-103">binaryManagementConditionExpression resource type</span></span>

<span data-ttu-id="8c8dd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c8dd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8c8dd-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c8dd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c8dd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8c8dd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c8dd-107">Выражение условия управления, вычисляемое с помощью бинарной операции.</span><span class="sxs-lookup"><span data-stu-id="8c8dd-107">A management condition expression that is evaluated using a binary operation.</span></span>


<span data-ttu-id="8c8dd-108">Наследуется от [манажементкондитионекспрессионмодел](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="8c8dd-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8c8dd-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="8c8dd-109">Properties</span></span>
|<span data-ttu-id="8c8dd-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="8c8dd-110">Property</span></span>|<span data-ttu-id="8c8dd-111">Тип</span><span class="sxs-lookup"><span data-stu-id="8c8dd-111">Type</span></span>|<span data-ttu-id="8c8dd-112">Описание</span><span class="sxs-lookup"><span data-stu-id="8c8dd-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c8dd-113">operator</span><span class="sxs-lookup"><span data-stu-id="8c8dd-113">operator</span></span>|[<span data-ttu-id="8c8dd-114">бинариманажементкондитионекспрессионоператортипе</span><span class="sxs-lookup"><span data-stu-id="8c8dd-114">binaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-binarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="8c8dd-115">Оператор, используемый для оценки бинарной операции.</span><span class="sxs-lookup"><span data-stu-id="8c8dd-115">The operator used in the evaluation of the binary operation.</span></span> <span data-ttu-id="8c8dd-116">Возможные значения: `or`, `and`.</span><span class="sxs-lookup"><span data-stu-id="8c8dd-116">Possible values are: `or`, `and`.</span></span>|
|<span data-ttu-id="8c8dd-117">фирстоперанд</span><span class="sxs-lookup"><span data-stu-id="8c8dd-117">firstOperand</span></span>|[<span data-ttu-id="8c8dd-118">манажементкондитионекспрессионмодел</span><span class="sxs-lookup"><span data-stu-id="8c8dd-118">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="8c8dd-119">Первый операнд бинарной операции.</span><span class="sxs-lookup"><span data-stu-id="8c8dd-119">The first operand of the binary operation.</span></span>|
|<span data-ttu-id="8c8dd-120">секондоперанд</span><span class="sxs-lookup"><span data-stu-id="8c8dd-120">secondOperand</span></span>|[<span data-ttu-id="8c8dd-121">манажементкондитионекспрессионмодел</span><span class="sxs-lookup"><span data-stu-id="8c8dd-121">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="8c8dd-122">Второй операнд бинарной операции.</span><span class="sxs-lookup"><span data-stu-id="8c8dd-122">The second operand of the binary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c8dd-123">Связи</span><span class="sxs-lookup"><span data-stu-id="8c8dd-123">Relationships</span></span>
<span data-ttu-id="8c8dd-124">Нет</span><span class="sxs-lookup"><span data-stu-id="8c8dd-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8c8dd-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8c8dd-125">JSON Representation</span></span>
<span data-ttu-id="8c8dd-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8c8dd-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.binaryManagementConditionExpression"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.binaryManagementConditionExpression",
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
                        "operator": "String",
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
  "secondOperand": {
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




