---
title: Управление мерами безопасности с помощью клиентский компонент Центра обновления Windows развертывания для бизнеса
description: При развертывании обновлений с клиентский компонент Центра обновления Windows развертывания для бизнеса оно автоматически запрещает устройствам с проблемой предлагать обновление.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 5373fe27415bbfd552303e7d154be131bdf76e11
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437445"
---
# <a name="manage-safeguards-using-the-windows-update-for-business-deployment-service"></a>Управление мерами безопасности с помощью клиентский компонент Центра обновления Windows развертывания для бизнеса

При развертывании обновлений с помощью службы развертывания служба автоматически защищает развертывания, не позволяя устройствам с известными или вероятными неполадками предлагать обновление клиентский компонент Центра обновления Windows.

Меры безопасности совместимы с [развертываниями Windows 11](windowsupdates-deployments.md) и Windows 10 компонентов. Меры защиты от известных проблем доступны для развертываний обновлений компонентов Windows 11 и Windows 10, а меры защиты от вероятных проблем доступны для развертываний Windows 11.

## <a name="apply-all-safeguards"></a>Применение всех мер безопасности

По умолчанию служба развертывания применяет все применимые меры безопасности к устройствам в развертывании. Чтобы воспользоваться преимуществами мер безопасности, не нужно указывать дополнительные параметры при создании развертывания.

В следующем примере показано, как создать развертывание со всеми примененными мерами безопасности.

### <a name="request"></a>Запрос

```http
POST https://graph.microsoft.com/beta/admin/windows/updates/deployments
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
    "content": {
        "@odata.type": "microsoft.graph.windowsUpdates.featureUpdateReference",
        "version": "20H2"
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
    "settings": null,
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```

## <a name="opt-out-of-safeguards-against-likely-issues"></a>Отключение защиты от вероятных проблем

Вы можете отказаться от мер защиты от вероятных проблем в развертывании, настроив [параметры защиты](/graph/api/resources/windowsupdates-safeguardsettings). При необходимости вы также можете отказаться от удержаний для известных проблем с помощью политики [отключения мер безопасности](/windows/deployment/update/safeguard-opt-out).

В следующем примере показано, как создать развертывание без защиты от вероятных проблем. Указав **параметр safeguardProfile**  `likelyIssues` для категории в списке профилей защиты для отключения, вы настраиваете развертывание, чтобы предложить обновление устройству, даже если, скорее всего, возникает проблема с обновлением.

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
        "safeguard": {
            "disabledSafeguardProfiles": [
                {
                    "category": "likelyIssues"
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
        "monitoring": null,
        "rollout": null,
        "userExperience": null,
        "safeguard": {
            "disabledSafeguardProfiles": [
                {
                    "@odata.type": "#microsoft.graph.windowsUpdates.safeguardProfile",
                    "category": "likelyIssues"
                }
            ]
        }
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```
