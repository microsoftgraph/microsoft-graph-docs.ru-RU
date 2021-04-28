---
title: Управление правилами мониторинга развертывания с помощью службы Windows обновления для бизнеса
description: Для развертывания, инициированного службой развертывания, можно использовать правила мониторинга, настраивая оповещения и автоматизированные действия на основе сигналов развертывания.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 7468bef695b704ef40b630e3f0e332e97fb12031
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067739"
---
# <a name="manage-monitoring-rules-for-a-feature-update-deployment-using-the-windows-update-for-business-deployment-service"></a><span data-ttu-id="7b509-103">Управление правилами мониторинга развертывания обновления функций с Windows службы развертывания для бизнеса</span><span class="sxs-lookup"><span data-stu-id="7b509-103">Manage monitoring rules for a feature update deployment using the Windows Update for Business deployment service</span></span>

<span data-ttu-id="7b509-104">Для развертывания, инициированного службой развертывания, можно использовать правило мониторинга для настройки оповещений и автоматизированных действий на основе сигналов развертывания.</span><span class="sxs-lookup"><span data-stu-id="7b509-104">For deployments initiated by the deployment service, you can use a monitoring rule to configure alerts and automated actions based on deployment signals.</span></span>

<span data-ttu-id="7b509-105">Правила мониторинга совместимы с развертыванием обновлений Windows 10 функций.</span><span class="sxs-lookup"><span data-stu-id="7b509-105">Monitoring rules are compatible with deployments of Windows 10 feature updates.</span></span>

> [!NOTE]
> <span data-ttu-id="7b509-106">Если при создании [](/graph/api/resources/windowsupdates-monitoringrule) развертывания не указано правило [мониторинга,](/graph/api/resources/windowsupdates-deployment)создается правило мониторинга по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7b509-106">If you do not specify a [monitoring rule](/graph/api/resources/windowsupdates-monitoringrule) when creating a [deployment](/graph/api/resources/windowsupdates-deployment), a default monitoring rule is created.</span></span> <span data-ttu-id="7b509-107">Это правило мониторинга по умолчанию **имеет** сигнал `rollback` , пороговое значение и  `20` **действие** `alertError` .</span><span class="sxs-lookup"><span data-stu-id="7b509-107">This default monitoring rule has a **signal** of `rollback`, a **threshold** of `20`, and an **action** of `alertError`.</span></span> <span data-ttu-id="7b509-108">В будущем обновлении API это поведение изменится и не будет создано правило мониторинга по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7b509-108">In a future update of the API, this behavior will change and a default monitoring rule will not be created.</span></span>

## <a name="step-1-create-a-monitoring-rule"></a><span data-ttu-id="7b509-109">Шаг 1. Создание правила мониторинга</span><span class="sxs-lookup"><span data-stu-id="7b509-109">Step 1: Create a monitoring rule</span></span>

<span data-ttu-id="7b509-110">Вы можете создать правило [мониторинга для](/graph/api/resources/windowsupdates-monitoringrule) развертывания, настроив [параметры мониторинга.](/graph/api/resources/windowsupdates-monitoringsettings)</span><span class="sxs-lookup"><span data-stu-id="7b509-110">You can create a [monitoring rule](/graph/api/resources/windowsupdates-monitoringrule) for a deployment by configuring the [monitoring settings](/graph/api/resources/windowsupdates-monitoringsettings).</span></span> <span data-ttu-id="7b509-111">Каждое [развертывание](/graph/api/resources/windowsupdates-deployments) может иметь одно правило активного мониторинга одновременно.</span><span class="sxs-lookup"><span data-stu-id="7b509-111">Each [deployment](/graph/api/resources/windowsupdates-deployments) can have one active monitoring rule at a time.</span></span>

<span data-ttu-id="7b509-112">Правила мониторинга состоят из трех компонентов:</span><span class="sxs-lookup"><span data-stu-id="7b509-112">Monitoring rules consist of three components:</span></span>
* <span data-ttu-id="7b509-113">**сигнал.** Тип проблемы обновления, которая должна отслеживаться службой развертывания.</span><span class="sxs-lookup"><span data-stu-id="7b509-113">**signal**: The type of update issue to be monitored by the deployment service.</span></span>
* <span data-ttu-id="7b509-114">**пороговое** значение. Когда этот процент устройств излучает указанный сигнал, запускается правило мониторинга.</span><span class="sxs-lookup"><span data-stu-id="7b509-114">**threshold**: When this percentage of devices emit the specified signal, the monitoring rule is triggered.</span></span>
* <span data-ttu-id="7b509-115">**действие.** Действие, необходимое при запуске правила мониторинга.</span><span class="sxs-lookup"><span data-stu-id="7b509-115">**action**: The action to take when the monitoring rule is triggered.</span></span>

<span data-ttu-id="7b509-116">Ниже приведен пример создания правила мониторинга для развертывания одновременно с созданием развертывания.</span><span class="sxs-lookup"><span data-stu-id="7b509-116">Below is an example of creating a monitoring rule for a deployment at the same time as creating the deployment.</span></span>

### <a name="request"></a><span data-ttu-id="7b509-117">Запрос</span><span class="sxs-lookup"><span data-stu-id="7b509-117">Request</span></span>

```http
POST https://graph.microsoft.com/beta/admin/windows/updates/deployments
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
    "content": {
        "@odata.type": "microsoft.graph.windowsUpdates.featureUpdateReference",
        "version": "20H2"
    },
    "settings": {
        "@odata.type": "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
        "monitoring": {
            "monitoringRules": [
                {
                    "@odata.type": "#microsoft.graph.windowsUpdates.monitoringRule",
                    "signal": "rollback",
                    "threshold": 5,
                    "action": "pauseDeployment"
                }
            ]
        }
    }
}
```

### <a name="response"></a><span data-ttu-id="7b509-118">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b509-118">Response</span></span>

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
    "id": "b5171742-1742-b517-4217-17b5421717b5",
    "state": {
        "@odata.type": "microsoft.graph.windowsUpdates.deploymentState",
        "value": "offering",
        "reasons": [
            {
                "@odata.type": "microsoft.graph.windowsUpdates.deploymentStateReason",
                "value": "offeringByRequest"
            }
        ],
        "requestedValue": "none",
        "effectiveSinceDate": "String (timestamp)"
    },
    "content": {
        "@odata.type": "microsoft.graph.windowsUpdates.featureUpdateReference",
        "version": "20H2"
    },
    "settings": {
        "@odata.type": "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
        "monitoring": {
            "monitoringRules": [
                {
                    "@odata.type": "#microsoft.graph.windowsUpdates.monitoringRule",
                    "signal": "rollback",
                    "threshold": 5,
                    "action": "pauseDeployment"
                }
            ]
        },
        "rollout": null,
        "userExperience": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```

## <a name="step-2-unpause-a-deployment-that-was-paused-by-a-monitoring-rule"></a><span data-ttu-id="7b509-119">Шаг 2. Приостановка развертывания, приостановленного правилом мониторинга</span><span class="sxs-lookup"><span data-stu-id="7b509-119">Step 2: Unpause a deployment that was paused by a monitoring rule</span></span>
<span data-ttu-id="7b509-120">Когда запускается правило мониторинга, оно предоставляет возможность исследовать проблемы обновления, которые могли привести к его применении.</span><span class="sxs-lookup"><span data-stu-id="7b509-120">When a monitoring rule triggers, it provides the opportunity to investigate update issues that may have lead to it being applied.</span></span> <span data-ttu-id="7b509-121">После расследования может потребоваться возобновить развертывание.</span><span class="sxs-lookup"><span data-stu-id="7b509-121">After investigation, you may wish to resume the deployment.</span></span> <span data-ttu-id="7b509-122">Это можно сделать двумя способами: удалить правило мониторинга или обновить пороговое значение правила мониторинга.</span><span class="sxs-lookup"><span data-stu-id="7b509-122">There are two ways to do so: removing the monitoring rule or updating the monitoring rule threshold.</span></span>

### <a name="example-resume-deployment-by-removing-a-monitoring-rule"></a><span data-ttu-id="7b509-123">Пример. Возобновление развертывания путем удаления правила мониторинга</span><span class="sxs-lookup"><span data-stu-id="7b509-123">Example: Resume deployment by removing a monitoring rule</span></span>
<span data-ttu-id="7b509-124">Когда запускается правило мониторинга, приостанавлив которое запускается развертывание, одним из способов возобновления развертывания является удаление правила.</span><span class="sxs-lookup"><span data-stu-id="7b509-124">When a monitoring rule that pauses the deployment is triggered, one way to resume the deployment is to remove the rule.</span></span>

<span data-ttu-id="7b509-125">Ниже приведен пример повторного развертывания путем удаления правила.</span><span class="sxs-lookup"><span data-stu-id="7b509-125">Below is an example of resuming the deployment by removing the rule.</span></span>

#### <a name="request"></a><span data-ttu-id="7b509-126">Запрос</span><span class="sxs-lookup"><span data-stu-id="7b509-126">Request</span></span>

``` http
PATCH https://graph.microsoft.com/beta/admin/windows/updates/deployments/b5171742-1742-b517-4217-17b5421717b5
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
    "settings": {
        "@odata.type": "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
        "monitoring": {
            "monitoringRules": []
        }
    }
}
```

#### <a name="response"></a><span data-ttu-id="7b509-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b509-127">Response</span></span>

``` http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
    "id": "b5171742-1742-b517-4217-17b5421717b5",
    "state": {
        "@odata.type": "microsoft.graph.windowsUpdates.deploymentState",
        "value": "offering",
        "reasons": [
            {
                "@odata.type": "microsoft.graph.windowsUpdates.deploymentStateReason",
                "value": "offeringByRequest"
            }
        ],
        "requestedValue": "none",
        "effectiveSinceDate": "String (timestamp)"
    },
    "content": {
        "@odata.type": "microsoft.graph.windowsUpdates.featureUpdateReference",
        "version": "20H2"
    },
    "settings": {
        "@odata.type": "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
        "monitoring": {
            "monitoringRules": []
        },
        "rollout": null,
        "userExperience": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```

### <a name="example-resume-deployment-by-updating-a-monitoring-rule-threshold"></a><span data-ttu-id="7b509-128">Пример: Возобновление развертывания путем обновления порогового значения правил мониторинга</span><span class="sxs-lookup"><span data-stu-id="7b509-128">Example: Resume deployment by updating a monitoring rule threshold</span></span>
<span data-ttu-id="7b509-129">Еще один способ возобновить развертывание — изменить пороговое значение соответствующего правила мониторинга.</span><span class="sxs-lookup"><span data-stu-id="7b509-129">Another way to resume the deployment is to change the threshold of the relevant monitoring rule.</span></span> <span data-ttu-id="7b509-130">После того, как будет достигнут новый порог, действие (в этом `pauseDeployment` случае) будет активировало еще раз.</span><span class="sxs-lookup"><span data-stu-id="7b509-130">When the new threshold is reached, the action (in this case, `pauseDeployment`) will be triggered again.</span></span> 

<span data-ttu-id="7b509-131">Ниже приведен пример повторного развертывания путем изменения порогового значения правила мониторинга.</span><span class="sxs-lookup"><span data-stu-id="7b509-131">Below is an example of resuming the deployment by changing the monitoring rule threshold.</span></span> <span data-ttu-id="7b509-132">В этом примере также показано, как изменить любое существующее правило мониторинга, даже если его пороговое значение еще не установлено, а также как создать правило мониторинга в развертывании, которое не имеет его.</span><span class="sxs-lookup"><span data-stu-id="7b509-132">This example also illustrates how to edit any existing monitoring rule, even if its threshold has not yet been met, as well as how to create a monitoring rule on a deployment that does not have one.</span></span>

#### <a name="request"></a><span data-ttu-id="7b509-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="7b509-133">Request</span></span>

``` http
PATCH https://graph.microsoft.com/beta/admin/windows/updates/deployments/b5171742-1742-b517-4217-17b5421717b5
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
    "settings": {
        "@odata.type": "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
        "monitoring": {
            "monitoringRules": [
                {
                    "@odata.type": "#microsoft.graph.windowsUpdates.monitoringRule",
                    "signal": "rollback",
                    "threshold": 10,
                    "action": "pauseDeployment"
                }
            ]
        }
    }
}
```

#### <a name="response"></a><span data-ttu-id="7b509-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b509-134">Response</span></span>

``` http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
    "id": "b5171742-1742-b517-4217-17b5421717b5",
    "state": {
        "@odata.type": "microsoft.graph.windowsUpdates.deploymentState",
        "value": "offering",
        "reasons": [
            {
                "@odata.type": "microsoft.graph.windowsUpdates.deploymentStateReason",
                "value": "offeringByRequest"
            }
        ],
        "requestedValue": "none",
        "effectiveSinceDate": "String (timestamp)"
    },
    "content": {
        "@odata.type": "microsoft.graph.windowsUpdates.featureUpdateReference",
        "version": "20H2"
    },
    "settings": {
        "@odata.type": "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
        "monitoring": {
            "monitoringRules": [
                {
                    "@odata.type": "#microsoft.graph.windowsUpdates.monitoringRule",
                    "signal": "rollback",
                    "threshold": 10,
                    "action": "pauseDeployment"
                }
            ]
        },
        "rollout": null,
        "userExperience": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```