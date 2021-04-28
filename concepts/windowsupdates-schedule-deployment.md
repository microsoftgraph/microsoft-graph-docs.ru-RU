---
title: Запланировать развертывание с Windows службы обновления для бизнеса
description: При развертывании обновления с помощью службы развертывания можно запланировать развертывание, чтобы устройства получали обновление в будущем.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 461b40ef1e25d6a1943c70456404e7a48bf73d8c
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067734"
---
# <a name="schedule-a-deployment-using-the-windows-update-for-business-deployment-service"></a><span data-ttu-id="276de-103">Запланировать развертывание с Windows службы обновления для бизнеса</span><span class="sxs-lookup"><span data-stu-id="276de-103">Schedule a deployment using the Windows Update for Business deployment service</span></span>

<span data-ttu-id="276de-104">При развертывании обновления с помощью службы развертывания можно запланировать развертывание, чтобы устройства получали обновление в будущем.</span><span class="sxs-lookup"><span data-stu-id="276de-104">When deploying an update using the deployment service, you can schedule the deployment so that devices receive the update at a future date.</span></span>

<span data-ttu-id="276de-105">Функции планирования совместимы с [развертыванием](windowsupdates-deployments.md) обновлений Windows 10 компонентов.</span><span class="sxs-lookup"><span data-stu-id="276de-105">Scheduling features are compatible with [deployments](windowsupdates-deployments.md) of Windows 10 feature updates.</span></span>

## <a name="schedule-a-deployment-to-start-at-a-future-date"></a><span data-ttu-id="276de-106">Запланировать развертывание для начала в будущем</span><span class="sxs-lookup"><span data-stu-id="276de-106">Schedule a deployment to start at a future date</span></span>

<span data-ttu-id="276de-107">Вы можете запланировать развертывание, чтобы начать в будущем, настроив его [параметры развертывания.](/graph/api/resources/windowsupdates-rolloutsettings)</span><span class="sxs-lookup"><span data-stu-id="276de-107">You can schedule a deployment to start at a future date by configuring its [rollout settings](/graph/api/resources/windowsupdates-rolloutsettings).</span></span> <span data-ttu-id="276de-108">В приведенном ниже примере всем устройствам, на которые назначено развертывание, будет предложено обновление 1 июля 2021 г.</span><span class="sxs-lookup"><span data-stu-id="276de-108">In the example below, all devices assigned the deployment will be offered the update on July 1, 2021.</span></span>

### <a name="request"></a><span data-ttu-id="276de-109">Запрос</span><span class="sxs-lookup"><span data-stu-id="276de-109">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="276de-110">Отклик</span><span class="sxs-lookup"><span data-stu-id="276de-110">Response</span></span>

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
        "userExperience": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```

## <a name="stage-a-deployment-over-a-period-of-time"></a><span data-ttu-id="276de-111">Этап развертывания в течение определенного периода времени</span><span class="sxs-lookup"><span data-stu-id="276de-111">Stage a deployment over a period of time</span></span>

<span data-ttu-id="276de-112">Вы также можете запланировать развертывание, чтобы назначенное устройство было предложено обновить в постепенном развертывании, которое будет происходить с течением времени.</span><span class="sxs-lookup"><span data-stu-id="276de-112">You can also schedule a deployment so that assigned devices are offered the update in a gradual rollout that is staged over time.</span></span> <span data-ttu-id="276de-113">Обновление предлагается подмесям устройств, заданные развертыванию с регулярными интервалами, при этом общая продолжительность развертывания определяется датой окончания или скоростью предложения.</span><span class="sxs-lookup"><span data-stu-id="276de-113">The update is offered to subsets of devices assigned to the deployment at regular intervals, with the total duration of the rollout determined by either an end date or offering rate.</span></span> <span data-ttu-id="276de-114">Можно думать о постепенном выкатке, как о повторяющейся серии событий календаря.</span><span class="sxs-lookup"><span data-stu-id="276de-114">You can think of a gradual rollout as similar to a recurring calendar event series.</span></span>

### <a name="example-stage-a-deployment-at-regular-intervals-between-start-and-end-dates"></a><span data-ttu-id="276de-115">Пример. Поэтапное развертывание с регулярными интервалами между датами начала и окончания</span><span class="sxs-lookup"><span data-stu-id="276de-115">Example: Stage a deployment at regular intervals between start and end dates</span></span>

<span data-ttu-id="276de-116">Одним из способов поэтапного развертывания со временем является настройка **endDateTime** развертывания.</span><span class="sxs-lookup"><span data-stu-id="276de-116">One way to stage a deployment over time is to set the **endDateTime** of the deployment.</span></span> <span data-ttu-id="276de-117">Всем устройствам, на которые назначено развертывание, будет предложено обновление в окне между **startDateTime** и **endDateTime.**</span><span class="sxs-lookup"><span data-stu-id="276de-117">All devices assigned to the deployment will be offered the update within the window between the **startDateTime** and **endDateTime**.</span></span> <span data-ttu-id="276de-118">Если **startDateTime** не указан, развертывание начнется сразу же после назначения устройств.</span><span class="sxs-lookup"><span data-stu-id="276de-118">If the **startDateTime** is not specified, then the deployment will begin as soon as devices are assigned.</span></span>


<span data-ttu-id="276de-119">В этом примере вы настраиваете новое развертывание таким образом, чтобы каждую неделю (продолжительность **ДействияBetweenOffers** установлена до семи дней), начиная с 1 июля 2021 г.</span><span class="sxs-lookup"><span data-stu-id="276de-119">In this example, you configure a new deployment so that a new set of devices is offered the update every week (**durationBetweenOffers** set to seven days), starting on July 1, 2021.</span></span> <span data-ttu-id="276de-120">Всем устройствам предлагается обновление до 1 августа 2021 г.</span><span class="sxs-lookup"><span data-stu-id="276de-120">All devices are offered the update before August 1, 2021.</span></span>

#### <a name="request"></a><span data-ttu-id="276de-121">Запрос</span><span class="sxs-lookup"><span data-stu-id="276de-121">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="276de-122">Отклик</span><span class="sxs-lookup"><span data-stu-id="276de-122">Response</span></span>

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
        "userExperience": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```


### <a name="example-stage-a-deployment-at-regular-intervals-with-a-specified-number-of-devices-at-each-offer"></a><span data-ttu-id="276de-123">Пример: поэтапное развертывание с заданным числом устройств в каждом предложении</span><span class="sxs-lookup"><span data-stu-id="276de-123">Example: Stage a deployment at regular intervals with a specified number of devices at each offer</span></span>

<span data-ttu-id="276de-124">Другой способ поэтапного развертывания со временем — настроить скорость предложения с помощью `devicesPerOffer` .</span><span class="sxs-lookup"><span data-stu-id="276de-124">Another way to stage a deployment over time is to configure the offering rate using `devicesPerOffer`.</span></span> <span data-ttu-id="276de-125">Устройствам, на которые назначено развертывание, будет предложено обновление в соответствии с указанной скоростью до тех пор, пока все устройства не будут предложены для обновления.</span><span class="sxs-lookup"><span data-stu-id="276de-125">Devices assigned to the deployment will be offered the update according to the specified rate until all devices have been offered the update.</span></span>

<span data-ttu-id="276de-126">В этом примере вы настраиваете новое развертывание таким образом, чтобы каждую неделю (продолжительность **ДействияBetweenOffers** установлена до семи дней), начиная с 1 июля 2021 г.</span><span class="sxs-lookup"><span data-stu-id="276de-126">In this example, you configure a new deployment so that a new set of devices is offered the update every week (**durationBetweenOffers** set to seven days), starting on July 1, 2021.</span></span> <span data-ttu-id="276de-127">100 устройств предлагаются обновления одновременно, пока все устройства не будут предложены обновления.</span><span class="sxs-lookup"><span data-stu-id="276de-127">100 devices are offered the update at a time until all devices have been offered the update.</span></span>

#### <a name="request"></a><span data-ttu-id="276de-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="276de-128">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="276de-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="276de-129">Response</span></span>

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
        "userExperience": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```