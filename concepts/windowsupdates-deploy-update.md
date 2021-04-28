---
title: Развертывание обновления функций с Windows службы развертывания для бизнеса
description: С помощью Windows обновления для бизнеса можно развернуть обновления Windows на устройствах в клиенте Azure AD.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 92bc4c7b2b5995dd99fbb7ff549610642e4451f6
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067747"
---
# <a name="deploy-a-feature-update-using-the-windows-update-for-business-deployment-service"></a>Развертывание обновления функций с Windows службы развертывания для бизнеса

С помощью Windows обновления для бизнеса можно развернуть Windows на устройствах в клиенте Azure AD. Сегодня служба развертывания поддерживает развертывание [Windows 10](windowsupdates-deployments.md) обновлений функций и ускоренные обновления безопасности. В этом разделе основное внимание уделяется развертыванию обновлений функций. Сведения о развертывании ускоряющихся обновлений безопасности см. в статью [Развертывание ускоренного обновления безопасности.](windowsupdates-deploy-expedited-update.md)

При развертывании обновления функций на устройстве Windows update предлагает указанное обновление устройству, если оно еще не получило обновление. Например, при развертывании Windows 10 версии обновления 20H2 на устройстве, которое зарегистрировано в управлении обновлениями функций и в настоящее время находится на более старой версии Windows 10, устройство обновляется до версии 20H2. Если устройство уже находится на уровне или выше версии 20H2, оно остается на текущей версии. Если устройство не зарегистрировали в управлении обновлениями функций, эта операция не влияет на устройство.

Пока устройство остается зарегистрированным в управлении обновлениями функций, оно не получает других обновлений функций из Windows Update, если явно не развернуто с помощью службы развертывания.

## <a name="prerequisites"></a>Необходимые условия

* Устройства отвечают [необходимым требованиям для службы развертывания.](windowsupdates-concept-overview.md#prerequisites)
* Прежде чем использовать службу развертывания для развертывания обновлений функций, устройства должны быть зарегистрированы в управлении службой развертывания для категории обновления функций. [](windowsupdates-enroll.md)

## <a name="step-1-optional-get-a-list-of-deployable-updates"></a>Шаг 1. (Необязательный) Получить список развертываемых обновлений

Вы можете запрашивать каталог службы развертывания, чтобы получить список обновлений, которые можно развернуть на устройствах в качестве контента в развертывании.

Ниже приведен пример запроса всех обновлений Windows 10, развертываемых службой развертывания.

### <a name="request"></a>Запрос

```http
GET https://graph.microsoft.com/beta/admin/windows/updates/catalog/entries?$filter=isof('microsoft.graph.windowsUpdates.featureUpdateCatalogEntry')
```

### <a name="response"></a>Отклик

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "value": [
        {
            "@odata.type": "#microsoft.graph.windowsUpdates.featureUpdateCatalogEntry",
            "id": "560a186a-1434-4364-8330-deb944b494ff",
            "displayName": "Windows 10, version 20H2",
            "releaseDate": "String (timestamp)",
            "deployableUntilDateTime": "String (timestamp)",
            "version": "20H2"
        },
        {
            "@odata.type": "#microsoft.graph.windowsUpdates.featureUpdateCatalogEntry",
            "id": "5e436dae-56bd-4925-bf8b-acf550e07227",
            "displayName": "Windows 10, version 2004",
            "releaseDate": "String (timestamp)",
            "deployableUntilDateTime": "String (timestamp)",
            "version": "2004"
        }
    ]
}
```

## <a name="step-2-create-a-deployment"></a>Шаг 2. Создание развертывания

[Развертывание](/graph/api/resources/windowsupdates-deployment) указывает содержимое для развертывания, как и когда развертывать контент и целевые устройства. При развертывании аудитория развертывания автоматически создается в качестве связи.

Ниже приведен пример создания развертывания обновления функций с необязательными настройками расписания развертывания и [правил мониторинга.](windowsupdates-manage-monitoring-rules.md) [](windowsupdates-schedule-deployment.md) Целевые устройства указаны на следующем шаге.

> [!NOTE]
> Если при создании [](/graph/api/resources/windowsupdates-monitoringrule) развертывания не указано правило мониторинга, создается правило мониторинга по умолчанию. Это правило мониторинга по умолчанию **имеет** сигнал `rollback` , пороговое значение и  `20` **действие** `alertError` . В будущем обновлении API это поведение изменится и не будет создано правило мониторинга по умолчанию.

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
        "rollout": {
            "devicesPerOffer": 100,
            "durationBetweenOffers": "P7D"
        },
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
        "rollout": {
            "devicesPerOffer": 100,
            "durationBetweenOffers": "P7D",
            "startDateTime": null,
            "endDateTime": null
        },
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
        "userExperience": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```

## <a name="step-3-assign-devices-to-the-deployment-audience"></a>Шаг 3. Назначение устройств аудитории развертывания

После создания развертывания можно назначить устройства аудитории [развертывания.](/graph/api/resources/windowsupdates-deploymentaudience) Устройства могут быть назначены напрямую или с помощью [updatable групп активов.](/graph/api/resources/windowsupdates-updatableassetgroup) После успешного обновления аудитории развертывания Windows update начинает предлагать обновление соответствующим устройствам в соответствии с настройками развертывания.

Устройства автоматически регистрируются в службе при добавлении в собрания участников или исключениях аудитории развертывания (например, объект [azureADDevice](/graph/api/resources/windowsupdates-azureaddevice) автоматически создается, если он еще не существует).

Ниже приведен пример добавления updatable групп активов и устройств Azure AD в качестве членов аудитории развертывания, а также исключение определенного устройства Azure AD.

### <a name="request"></a>Запрос

```http
POST https://graph.microsoft.com/beta/admin/windows/updates/deployments/{deploymentId}/audience/updateAudience
Content-type: application/json

{
    "addMembers": [
        {
            "@odata.type": "#microsoft.graph.windowsUpdates.updatableAssetGroup",
            "id": "String (identifier)"
        },
        {
            "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
            "id": "String (identifier)"
        },
        {
            "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
            "id": "String (identifier)"
        }
    ],
    "addExclusions": [
        {
            "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
            "id": "String (identifier)"
        }
    ]
}
```

### <a name="response"></a>Отклик

```http
HTTP/1.1 202 Accepted
```

## <a name="during-a-deployment"></a>Во время развертывания

Во время развертывания можно приостановить развертывание, обновив его **состояние,** а также обновив членов аудитории и исключения.

## <a name="after-a-deployment"></a>После развертывания

После того как все устройства, заданные аудитории развертывания, были первоначально предложены обновления, возможно, что не все устройства начали или завершили обновление из-за таких факторов, как подключение к устройству. До тех пор, пока развертывание еще существует, Windows update продолжает предлагать обновление для назначенного устройства всякий раз, когда они снова подключены.

