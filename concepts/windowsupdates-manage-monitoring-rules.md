---
title: Управление правилами мониторинга развертывания с помощью службы Windows обновления для бизнеса
description: Для развертывания, инициированного службой развертывания, можно использовать правила мониторинга, настраивая оповещения и автоматизированные действия на основе сигналов развертывания.
author: Alice-at-Microsoft
ms.localizationpriority: medium
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 1e4f0538a9e7a5d47b070514685a11860a86ac35
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59117531"
---
# <a name="manage-monitoring-rules-for-a-feature-update-deployment-using-the-windows-update-for-business-deployment-service"></a>Управление правилами мониторинга развертывания обновления функций с Windows службы развертывания для бизнеса

Для развертывания, инициированного службой развертывания, можно использовать правило мониторинга для настройки оповещений и автоматизированных действий на основе сигналов развертывания.

Правила мониторинга совместимы с развертыванием обновлений Windows 10 функций.

> [!NOTE]
> Если при создании [](/graph/api/resources/windowsupdates-monitoringrule) развертывания не указано правило [мониторинга,](/graph/api/resources/windowsupdates-deployment)создается правило мониторинга по умолчанию. Это правило мониторинга по умолчанию **имеет** сигнал `rollback` , пороговое значение и  `20` **действие** `alertError` . В будущем обновлении API это поведение изменится и не будет создано правило мониторинга по умолчанию.

## <a name="step-1-create-a-monitoring-rule"></a>Шаг 1. Создание правила мониторинга

Вы можете создать правило [мониторинга для](/graph/api/resources/windowsupdates-monitoringrule) развертывания, настроив [параметры мониторинга.](/graph/api/resources/windowsupdates-monitoringsettings) Каждое [развертывание](/graph/api/resources/windowsupdates-deployments) может иметь одно правило активного мониторинга одновременно.

Правила мониторинга состоят из трех компонентов:
* **сигнал.** Тип проблемы обновления, которая должна отслеживаться службой развертывания.
* **пороговое** значение. Когда этот процент устройств излучает указанный сигнал, запускается правило мониторинга.
* **действие.** Действие, необходимое при запуске правила мониторинга.

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
        "userExperience": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```

## <a name="step-2-unpause-a-deployment-that-was-paused-by-a-monitoring-rule"></a>Шаг 2. Приостановка развертывания, приостановленного правилом мониторинга
Когда запускается правило мониторинга, оно предоставляет возможность исследовать проблемы обновления, которые могли привести к его применении. После расследования может потребоваться возобновить развертывание. Это можно сделать двумя способами: удалить правило мониторинга или обновить пороговое значение правила мониторинга.

### <a name="example-resume-deployment-by-removing-a-monitoring-rule"></a>Пример. Возобновление развертывания путем удаления правила мониторинга
Когда запускается правило мониторинга, приостанавлив которое запускается развертывание, одним из способов возобновления развертывания является удаление правила.

Ниже приведен пример повторного развертывания путем удаления правила.

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
        "userExperience": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```

### <a name="example-resume-deployment-by-updating-a-monitoring-rule-threshold"></a>Пример: Возобновление развертывания путем обновления порогового значения правил мониторинга
Еще один способ возобновить развертывание — изменить пороговое значение соответствующего правила мониторинга. После того, как будет достигнут новый порог, действие (в этом `pauseDeployment` случае) будет активировало еще раз. 

Ниже приведен пример повторного развертывания путем изменения порогового значения правила мониторинга. В этом примере также показано, как изменить любое существующее правило мониторинга, даже если его пороговое значение еще не установлено, а также как создать правило мониторинга в развертывании, которое не имеет его.

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
        "userExperience": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```
