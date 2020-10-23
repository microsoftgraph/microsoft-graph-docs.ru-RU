---
title: Тип ресурса Унариманажементкондитионекспрессион
description: Выражение условия управления, вычисляемое с использованием унарной операции.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e940331176c52f8e8da848793088a1388f977339
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728090"
---
# <a name="unarymanagementconditionexpression-resource-type"></a><span data-ttu-id="91e62-103">Тип ресурса Унариманажементкондитионекспрессион</span><span class="sxs-lookup"><span data-stu-id="91e62-103">unaryManagementConditionExpression resource type</span></span>

<span data-ttu-id="91e62-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91e62-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="91e62-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91e62-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="91e62-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="91e62-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91e62-107">Выражение условия управления, вычисляемое с использованием унарной операции.</span><span class="sxs-lookup"><span data-stu-id="91e62-107">A management condition expression that is evaluated using a unary operation.</span></span>


<span data-ttu-id="91e62-108">Наследуется от [манажементкондитионекспрессионмодел](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="91e62-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="91e62-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="91e62-109">Properties</span></span>
|<span data-ttu-id="91e62-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="91e62-110">Property</span></span>|<span data-ttu-id="91e62-111">Тип</span><span class="sxs-lookup"><span data-stu-id="91e62-111">Type</span></span>|<span data-ttu-id="91e62-112">Описание</span><span class="sxs-lookup"><span data-stu-id="91e62-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91e62-113">operator</span><span class="sxs-lookup"><span data-stu-id="91e62-113">operator</span></span>|[<span data-ttu-id="91e62-114">унариманажементкондитионекспрессионоператортипе</span><span class="sxs-lookup"><span data-stu-id="91e62-114">unaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-unarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="91e62-115">Оператор, используемый в оценке унарной операции.</span><span class="sxs-lookup"><span data-stu-id="91e62-115">The operator used in the evaluation of the unary operation.</span></span> <span data-ttu-id="91e62-116">Возможные значения: `not` .</span><span class="sxs-lookup"><span data-stu-id="91e62-116">Possible values are: `not`.</span></span>|
|<span data-ttu-id="91e62-117">начинается</span><span class="sxs-lookup"><span data-stu-id="91e62-117">operand</span></span>|[<span data-ttu-id="91e62-118">манажементкондитионекспрессионмодел</span><span class="sxs-lookup"><span data-stu-id="91e62-118">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="91e62-119">Операнд унарной операции.</span><span class="sxs-lookup"><span data-stu-id="91e62-119">The operand of the unary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="91e62-120">Связи</span><span class="sxs-lookup"><span data-stu-id="91e62-120">Relationships</span></span>
<span data-ttu-id="91e62-121">Нет</span><span class="sxs-lookup"><span data-stu-id="91e62-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="91e62-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="91e62-122">JSON Representation</span></span>
<span data-ttu-id="91e62-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="91e62-123">Here is a JSON representation of the resource.</span></span>
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





