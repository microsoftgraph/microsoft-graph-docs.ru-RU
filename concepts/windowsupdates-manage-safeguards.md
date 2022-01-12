---
title: Управление гарантиями с помощью службы Windows обновления для бизнеса
description: При развертывании обновлений в службе развертывания служба автоматически защищает развертывание, не мешая устройствам с известными или вероятными вопросами предлагать обновление Windows Update.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: ff3d8c594087253db85fb943bd34fe9478f45bb9
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61855521"
---
# <a name="manage-safeguards-using-the-windows-update-for-business-deployment-service"></a>Управление гарантиями с помощью службы Windows обновления для бизнеса

При развертывании обновлений в службе развертывания служба автоматически защищает развертывание, не мешая устройствам с известными или вероятными вопросами предлагать обновление Windows Update.

Гарантии совместимы с [развертыванием обновлений](windowsupdates-deployments.md) Windows 11 Windows 10 функций. Средства защиты от известных проблем доступны для развертывания обновлений 11 Windows и Windows 10, а средства защиты от вероятных проблем доступны для развертывания Windows 11.

## <a name="apply-all-safeguards"></a>Применение всех гарантий

По умолчанию служба развертывания применяет все применимые гарантии к устройствам в развертывании. Чтобы воспользоваться преимуществами защиты, не нужно указывать какие-либо дополнительные средства при создании развертывания.

В следующем примере показано, как создать развертывание со всеми применяемыми гарантиями.

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

Можно отказаться от защиты от вероятных проблем в развертывании, настроив [параметры защиты.](/graph/api/resources/windowsupdates-safeguardsettings) При необходимости вы также можете отказаться от сохранения для известных проблем с помощью политики [отключения гарантий.](/windows/deployment/update/safeguard-opt-out)

В следующем примере показано, как создать развертывание без защиты от вероятных проблем. Указав **safeguardProfile** для  категории в списке профилей защиты, которые необходимо отключить, развертывание настраивается, чтобы предложить обновление устройству, даже если у него может быть проблема с `likelyIssues` обновлением.

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
