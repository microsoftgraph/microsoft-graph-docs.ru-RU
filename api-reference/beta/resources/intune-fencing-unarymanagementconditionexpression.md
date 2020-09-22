---
title: Тип ресурса Унариманажементкондитионекспрессион
description: Выражение условия управления, вычисляемое с использованием унарной операции.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ecb9c6543a8dbef076822fd09a994a2c7c760272
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48031265"
---
# <a name="unarymanagementconditionexpression-resource-type"></a><span data-ttu-id="ec1e2-103">Тип ресурса Унариманажементкондитионекспрессион</span><span class="sxs-lookup"><span data-stu-id="ec1e2-103">unaryManagementConditionExpression resource type</span></span>

<span data-ttu-id="ec1e2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec1e2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ec1e2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec1e2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ec1e2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ec1e2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec1e2-107">Выражение условия управления, вычисляемое с использованием унарной операции.</span><span class="sxs-lookup"><span data-stu-id="ec1e2-107">A management condition expression that is evaluated using a unary operation.</span></span>


<span data-ttu-id="ec1e2-108">Наследуется от [манажементкондитионекспрессионмодел](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="ec1e2-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ec1e2-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="ec1e2-109">Properties</span></span>
|<span data-ttu-id="ec1e2-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="ec1e2-110">Property</span></span>|<span data-ttu-id="ec1e2-111">Тип</span><span class="sxs-lookup"><span data-stu-id="ec1e2-111">Type</span></span>|<span data-ttu-id="ec1e2-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ec1e2-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec1e2-113">operator</span><span class="sxs-lookup"><span data-stu-id="ec1e2-113">operator</span></span>|[<span data-ttu-id="ec1e2-114">унариманажементкондитионекспрессионоператортипе</span><span class="sxs-lookup"><span data-stu-id="ec1e2-114">unaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-unarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="ec1e2-115">Оператор, используемый в оценке унарной операции.</span><span class="sxs-lookup"><span data-stu-id="ec1e2-115">The operator used in the evaluation of the unary operation.</span></span> <span data-ttu-id="ec1e2-116">Возможные значения: `not` .</span><span class="sxs-lookup"><span data-stu-id="ec1e2-116">Possible values are: `not`.</span></span>|
|<span data-ttu-id="ec1e2-117">начинается</span><span class="sxs-lookup"><span data-stu-id="ec1e2-117">operand</span></span>|[<span data-ttu-id="ec1e2-118">манажементкондитионекспрессионмодел</span><span class="sxs-lookup"><span data-stu-id="ec1e2-118">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="ec1e2-119">Операнд унарной операции.</span><span class="sxs-lookup"><span data-stu-id="ec1e2-119">The operand of the unary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ec1e2-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="ec1e2-120">Relationships</span></span>
<span data-ttu-id="ec1e2-121">Нет</span><span class="sxs-lookup"><span data-stu-id="ec1e2-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ec1e2-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ec1e2-122">JSON Representation</span></span>
<span data-ttu-id="ec1e2-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ec1e2-123">Here is a JSON representation of the resource.</span></span>
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






