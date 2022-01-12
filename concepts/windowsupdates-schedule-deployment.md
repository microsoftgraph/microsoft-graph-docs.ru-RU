---
title: Запланировать развертывание с Windows службы обновления для бизнеса
description: При развертывании обновления с помощью службы развертывания можно запланировать развертывание, чтобы устройства получали обновление в будущем.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 650e35dc8496bcb9e2dbcee33d7dfca58db1615b
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61854830"
---
# <a name="schedule-a-deployment-using-the-windows-update-for-business-deployment-service"></a>Запланировать развертывание с Windows службы обновления для бизнеса

При развертывании обновления с помощью службы развертывания можно запланировать развертывание, чтобы устройства получали обновление в будущем.

Функции планирования совместимы с [развертыванием](windowsupdates-deployments.md) обновлений Windows 10 компонентов.

## <a name="schedule-a-deployment-to-start-at-a-future-date"></a>Запланировать развертывание для начала в будущем

Вы можете запланировать развертывание, чтобы начать в будущем, настроив его [параметры развертывания.](/graph/api/resources/windowsupdates-rolloutsettings) В приведенном ниже примере всем устройствам, на которые назначено развертывание, будет предложено обновление 1 июля 2021 г.

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

## <a name="stage-a-deployment-over-a-period-of-time"></a>Этап развертывания в течение определенного периода времени

Вы также можете запланировать развертывание, чтобы назначенное устройство было предложено обновить в постепенном развертывании, которое будет происходить с течением времени. Обновление предлагается подмесям устройств, заданные развертыванию с регулярными интервалами, при этом общая продолжительность развертывания определяется датой окончания или скоростью предложения. Постепенное развертывание напоминает ряд повторяющихся событий в календаре.

### <a name="example-stage-a-deployment-at-regular-intervals-between-start-and-end-dates"></a>Пример. Поэтапное развертывание с регулярными интервалами между датами начала и окончания

Одним из способов поэтапного развертывания со временем является настройка **endDateTime** развертывания. Всем устройствам, на которые назначено развертывание, будет предложено обновление в окне между **startDateTime** и **endDateTime.** Если **startDateTime** не указан, развертывание начнется сразу же после назначения устройств.

В этом примере вы настраиваете новое развертывание таким образом, чтобы каждую неделю (продолжительность **ДействияBetweenOffers** установлена до семи дней), начиная с 1 июля 2021 г. Всем устройствам предлагается обновление до 1 августа 2021 г.

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


### <a name="example-stage-a-deployment-at-regular-intervals-with-a-specified-number-of-devices-at-each-offer"></a>Пример: поэтапное развертывание с заданным числом устройств в каждом предложении

Другой способ поэтапного развертывания со временем — настроить скорость предложения с помощью `devicesPerOffer` . Устройствам, на которые назначено развертывание, будет предложено обновление в соответствии с указанной скоростью до тех пор, пока все устройства не будут предложены для обновления.

В этом примере вы настраиваете новое развертывание таким образом, чтобы каждую неделю (продолжительность **ДействияBetweenOffers** установлена до семи дней), начиная с 1 июля 2021 г. 100 устройств предлагаются обновления одновременно, пока все устройства не будут предложены обновления.

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
