---
title: Управление правилами мониторинга с помощью клиентский компонент Центра обновления Windows развертывания для бизнеса
description: Используйте службу клиентский компонент Центра обновления Windows для бизнеса, чтобы создать правило мониторинга или возобновить развертывания, приостановленные правилом мониторинга.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 30f2c9cd2d219710fda5beba6862e9f15c7c94d6
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437452"
---
# <a name="manage-monitoring-rules-using-the-windows-update-for-business-deployment-service"></a>Управление правилами мониторинга с помощью клиентский компонент Центра обновления Windows развертывания для бизнеса

Для развертываний, инициированных службой развертывания, можно использовать правило мониторинга для настройки оповещений и автоматических действий на основе сигналов развертывания.

Правила мониторинга совместимы с развертываниями Windows 10 компонентов.

## <a name="step-1-create-a-monitoring-rule"></a>Шаг 1. Создание правила мониторинга

Вы можете создать правило [мониторинга для](/graph/api/resources/windowsupdates-monitoringrule) развертывания, настроив [параметры мониторинга](/graph/api/resources/windowsupdates-monitoringsettings). [Каждое развертывание](/graph/api/resources/windowsupdates-deployments) может иметь одно активное правило мониторинга за раз.

Правила мониторинга состоят из трех компонентов:
* **signal**: тип проблемы обновления, отслеживаемой службой развертывания.
* **threshold**: When this percentage of devices emit the specified signal, the monitoring rule is triggered.
* **действие**: действие, выполняемые при активации правила мониторинга.

Ниже приведен пример создания правила мониторинга для развертывания одновременно с созданием развертывания.

### <a name="request"></a>Запрос

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
                    "signal": "rollback",
                    "threshold": 5,
                    "action": "pauseDeployment"
                }
            ]
        }
    }
}
```

### <a name="response"></a>Отклик

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
        "userExperience": null,
        "safeguard": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```

## <a name="step-2-resume-a-deployment-that-was-paused-by-a-monitoring-rule"></a>Шаг 2. Возобновление развертывания, приостановленного правилом мониторинга
Когда правило мониторинга активируется, оно предоставляет возможность исследовать проблемы обновления, которые могли привести к его применении. После изучения может потребоваться возобновить развертывание. Это можно сделать двумя способами: удалить правило мониторинга или обновить пороговое значение правила мониторинга.

### <a name="example-resume-deployment-by-removing-a-monitoring-rule"></a>Пример. Возобновление развертывания путем удаления правила мониторинга
При активации правила мониторинга, которое приостанавливать развертывание, одним из способов возобновления развертывания является удаление правила.

Ниже приведен пример возобновления развертывания путем удаления правила.

#### <a name="request"></a>Запрос

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

#### <a name="response"></a>Отклик

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
        "userExperience": null,
        "safeguard": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```

### <a name="example-resume-deployment-by-updating-a-monitoring-rule-threshold"></a>Пример. Возобновление развертывания путем обновления порогового значения правила мониторинга
Еще один способ возобновить развертывание — изменить пороговое значение соответствующего правила мониторинга. Когда будет достигнуто новое пороговое значение, действие (в `pauseDeployment`данном случае) будет активироваться снова. 

Ниже приведен пример возобновления развертывания путем изменения порогового значения правила мониторинга. В этом примере также показано, как изменить любое существующее правило мониторинга, даже если его пороговое значение еще не достигнуто, а также как создать правило мониторинга в развертывании, в котором его нет.

#### <a name="request"></a>Запрос

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
                    "signal": "rollback",
                    "threshold": 10,
                    "action": "pauseDeployment"
                }
            ]
        }
    }
}
```

#### <a name="response"></a>Отклик

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
        "userExperience": null,
        "safeguard": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```
