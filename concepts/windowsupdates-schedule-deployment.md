---
title: Планирование развертывания с помощью службы клиентский компонент Центра обновления Windows для бизнеса
description: При развертывании обновления можно запланировать развертывание, чтобы устройства получили обновление позже с помощью службы клиентский компонент Центра обновления Windows для бизнеса.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 60d505eb5fab2ef003bb04762b6cccf3974e4f25
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437389"
---
# <a name="schedule-a-deployment-using-the-windows-update-for-business-deployment-service"></a>Планирование развертывания с помощью службы клиентский компонент Центра обновления Windows для бизнеса

При развертывании обновления с помощью службы развертывания можно запланировать развертывание, чтобы устройства получили обновление в будущем.

Функции планирования совместимы с [развертываниями](windowsupdates-deployments.md) Windows 10 компонентов.

## <a name="schedule-a-deployment-to-start-at-a-future-date"></a>Планирование развертывания на будущий день

Вы можете запланировать развертывание на будущую дату, настроив его [параметры развертывания](/graph/api/resources/windowsupdates-rolloutsettings). В приведенном ниже примере всем устройствам, назначенным развертыванию, будет предложено обновление 1 июля 2021 г.

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
            "startDateTime": "2021-07-01T17:00:00Z",
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
            "startDateTime": "2021-07-01T17:00:00Z",
            "endDateTime": null,
            "durationBetweenOffers": "P1D",
            "devicesPerOffer": null
        },
        "monitoring": null,
        "userExperience": null,
        "safeguard": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```

## <a name="stage-a-deployment-over-a-period-of-time"></a>Подготовка развертывания в течение определенного периода времени

Вы также можете запланировать развертывание таким образом, чтобы назначенным устройствам было предложено обновление в постепенном развертывании, которое со временем выполняется поэтапно. Обновление предлагается подмножествам устройств, назначенных развертыванию, через регулярные интервалы, с общей длительностью развертывания, определяемой датой окончания или частотой предложения. Постепенное развертывание напоминает ряд повторяющихся событий в календаре.

### <a name="example-stage-a-deployment-at-regular-intervals-between-start-and-end-dates"></a>Пример. Подготовка развертывания с регулярными интервалами между датами начала и окончания

Один из способов промежуточного развертывания с течением времени — задать **endDateTime** развертывания. Всем устройствам, назначенным для развертывания, будет предложено обновление в течение периода между **startDateTime** **и endDateTime**. Если **параметр startDateTime** не указан, развертывание начнется сразу после назначения устройств.

В этом примере вы настраиваете новое развертывание таким образом, чтобы новый набор устройств обновлялись каждую неделю (для **параметра durationBetweenOffers** задано семь дней), начиная с 1 июля 2021 г. Всем устройствам предлагается обновление до 1 августа 2021 г.

#### <a name="request"></a>Запрос

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
            "startDateTime": "2021-07-01T17:00:00Z",
            "endDateTime": "2021-08-01T17:00:00Z",
            "durationBetweenOffers": "P7D"
        }
    }
}
```

#### <a name="response"></a>Отклик

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
            "startDateTime": "2021-07-01T17:00:00Z",
            "endDateTime": "2021-08-01T17:00:00Z",
            "durationBetweenOffers": "P7D",
            "devicesPerOffer": null
        },
        "monitoring": null,
        "userExperience": null,
        "safeguard": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```


### <a name="example-stage-a-deployment-at-regular-intervals-with-a-specified-number-of-devices-at-each-offer"></a>Пример. Регулярное поэтапное развертывание с указанным количеством устройств в каждом предложении

Еще один способ упределить развертывание с течением времени — настроить ставку предложения с помощью `devicesPerOffer`. Устройства, назначенные развертыванию, будут предлагаться в соответствии с указанной скоростью до тех пор, пока все устройства не будут предлагать обновление.

В этом примере вы настраиваете новое развертывание таким образом, чтобы новый набор устройств обновлялись каждую неделю (для **параметра durationBetweenOffers** задано семь дней), начиная с 1 июля 2021 г. Обновление предлагается 100 устройствам одновременно, пока не будет предложено обновление для всех устройств.

#### <a name="request"></a>Запрос

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
            "startDateTime": "2020-07-01T17:00:00Z",
            "devicesPerOffer": 100,
            "durationBetweenOffers": "P7D"
        }
    }
}
```

#### <a name="response"></a>Отклик

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
            "startDateTime": "2020-07-01T17:00:00Z",
            "devicesPerOffer": 100,
            "durationBetweenOffers": "P7D",
            "endDateTime": null
        },
        "monitoring": null,
        "userExperience": null,
        "safeguard": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```
