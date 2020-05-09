---
title: Тип ресурса Унариманажементкондитионекспрессион
description: Выражение условия управления, вычисляемое с использованием унарной операции.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d4e6d3081574a1aaacb0ad336f200ed0e9337b23
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44177424"
---
# <a name="unarymanagementconditionexpression-resource-type"></a><span data-ttu-id="bbd47-103">Тип ресурса Унариманажементкондитионекспрессион</span><span class="sxs-lookup"><span data-stu-id="bbd47-103">unaryManagementConditionExpression resource type</span></span>

<span data-ttu-id="bbd47-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bbd47-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bbd47-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bbd47-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bbd47-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bbd47-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bbd47-107">Выражение условия управления, вычисляемое с использованием унарной операции.</span><span class="sxs-lookup"><span data-stu-id="bbd47-107">A management condition expression that is evaluated using a unary operation.</span></span>


<span data-ttu-id="bbd47-108">Наследуется от [манажементкондитионекспрессионмодел](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="bbd47-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bbd47-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="bbd47-109">Properties</span></span>
|<span data-ttu-id="bbd47-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="bbd47-110">Property</span></span>|<span data-ttu-id="bbd47-111">Тип</span><span class="sxs-lookup"><span data-stu-id="bbd47-111">Type</span></span>|<span data-ttu-id="bbd47-112">Описание</span><span class="sxs-lookup"><span data-stu-id="bbd47-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bbd47-113">operator</span><span class="sxs-lookup"><span data-stu-id="bbd47-113">operator</span></span>|[<span data-ttu-id="bbd47-114">унариманажементкондитионекспрессионоператортипе</span><span class="sxs-lookup"><span data-stu-id="bbd47-114">unaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-unarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="bbd47-115">Оператор, используемый в оценке унарной операции.</span><span class="sxs-lookup"><span data-stu-id="bbd47-115">The operator used in the evaluation of the unary operation.</span></span> <span data-ttu-id="bbd47-116">Возможные значения: `not`.</span><span class="sxs-lookup"><span data-stu-id="bbd47-116">Possible values are: `not`.</span></span>|
|<span data-ttu-id="bbd47-117">начинается</span><span class="sxs-lookup"><span data-stu-id="bbd47-117">operand</span></span>|[<span data-ttu-id="bbd47-118">манажементкондитионекспрессионмодел</span><span class="sxs-lookup"><span data-stu-id="bbd47-118">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="bbd47-119">Операнд унарной операции.</span><span class="sxs-lookup"><span data-stu-id="bbd47-119">The operand of the unary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bbd47-120">Связи</span><span class="sxs-lookup"><span data-stu-id="bbd47-120">Relationships</span></span>
<span data-ttu-id="bbd47-121">Нет</span><span class="sxs-lookup"><span data-stu-id="bbd47-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bbd47-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bbd47-122">JSON Representation</span></span>
<span data-ttu-id="bbd47-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bbd47-123">Here is a JSON representation of the resource.</span></span>
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



