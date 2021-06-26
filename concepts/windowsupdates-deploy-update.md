---
title: Развертывание обновления функций с Windows службы развертывания для бизнеса
description: С помощью Windows обновления для бизнеса можно развернуть обновления Windows на устройствах в клиенте Azure AD.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 2022294dc9467c2854642ac255169aa867ac162e
ms.sourcegitcommit: 0ca0a1e2810701c2392e5c685e984fbfb6785579
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2021
ms.locfileid: "53151603"
---
# <a name="deploy-a-feature-update-using-the-windows-update-for-business-deployment-service"></a><span data-ttu-id="a83be-103">Развертывание обновления функций с Windows службы развертывания для бизнеса</span><span class="sxs-lookup"><span data-stu-id="a83be-103">Deploy a feature update using the Windows Update for Business deployment service</span></span>

<span data-ttu-id="a83be-104">С помощью Windows обновления для бизнеса можно развернуть Windows на устройствах в клиенте Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a83be-104">With the Windows Update for Business deployment service, you can deploy Windows updates to devices in an Azure AD tenant.</span></span> <span data-ttu-id="a83be-105">Сегодня служба развертывания поддерживает развертывание [Windows 10](windowsupdates-deployments.md) обновлений функций и ускоренные обновления безопасности.</span><span class="sxs-lookup"><span data-stu-id="a83be-105">Today, the deployment service supports [deployments](windowsupdates-deployments.md) of Windows 10 feature updates and expedited security updates.</span></span> <span data-ttu-id="a83be-106">В этом разделе основное внимание уделяется развертыванию обновлений функций.</span><span class="sxs-lookup"><span data-stu-id="a83be-106">This topic focuses on deployments of feature updates.</span></span> <span data-ttu-id="a83be-107">Сведения о развертывании ускоряющихся обновлений безопасности см. в статью [Развертывание ускоренного обновления безопасности.](windowsupdates-deploy-expedited-update.md)</span><span class="sxs-lookup"><span data-stu-id="a83be-107">For information on deploying expedited security updates, see [Deploy an expedited security update](windowsupdates-deploy-expedited-update.md).</span></span>

<span data-ttu-id="a83be-108">При развертывании обновления функций на устройстве Windows update предлагает указанное обновление устройству, если оно еще не получило обновление.</span><span class="sxs-lookup"><span data-stu-id="a83be-108">When you deploy a feature update to a device, Windows Update offers the specified update to the device if it has not yet received the update.</span></span> <span data-ttu-id="a83be-109">Например, при развертывании Windows 10 версии обновления 20H2 на устройстве, которое зарегистрировано в управлении обновлениями функций и в настоящее время находится на более старой версии Windows 10, устройство обновляется до версии 20H2.</span><span class="sxs-lookup"><span data-stu-id="a83be-109">For example, if you deploy Windows 10 feature update version 20H2 to a device that is enrolled in feature update management and is currently on an older version of Windows 10, the device updates to version 20H2.</span></span> <span data-ttu-id="a83be-110">Если устройство уже находится на уровне или выше версии 20H2, оно остается на текущей версии.</span><span class="sxs-lookup"><span data-stu-id="a83be-110">If the device is already at or above version 20H2, it stays on its current version.</span></span> <span data-ttu-id="a83be-111">Если устройство не зарегистрировали в управлении обновлениями функций, эта операция не влияет на устройство.</span><span class="sxs-lookup"><span data-stu-id="a83be-111">If the device is not enrolled in feature update management, the device is not affected by this operation.</span></span>

<span data-ttu-id="a83be-112">Пока устройство остается зарегистрированным в управлении обновлениями функций, оно не получает других обновлений функций из Windows Update, если явно не развернуто с помощью службы развертывания.</span><span class="sxs-lookup"><span data-stu-id="a83be-112">As long as a device remains enrolled in feature update management, the device does not receive any other feature updates from Windows Update unless explicitly deployed using the deployment service.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a83be-113">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="a83be-113">Prerequisites</span></span>

* <span data-ttu-id="a83be-114">Устройства отвечают [необходимым требованиям для службы развертывания.](windowsupdates-concept-overview.md#prerequisites)</span><span class="sxs-lookup"><span data-stu-id="a83be-114">Devices meet the [prerequisites for the deployment service](windowsupdates-concept-overview.md#prerequisites).</span></span>
* <span data-ttu-id="a83be-115">Прежде чем использовать службу развертывания для развертывания обновлений функций, устройства должны быть зарегистрированы в управлении службой развертывания для категории обновления функций. [](windowsupdates-enroll.md)</span><span class="sxs-lookup"><span data-stu-id="a83be-115">Before you can use the deployment service to deploy feature updates, devices must be [enrolled in management](windowsupdates-enroll.md) by the deployment service for the feature update category.</span></span>

## <a name="step-1-optional-get-a-list-of-deployable-updates"></a><span data-ttu-id="a83be-116">Шаг 1. (Необязательный) Получить список развертываемых обновлений</span><span class="sxs-lookup"><span data-stu-id="a83be-116">Step 1: (Optional) Get a list of deployable updates</span></span>

<span data-ttu-id="a83be-117">Вы можете запрашивать каталог службы развертывания, чтобы получить список обновлений, которые можно развернуть на устройствах в качестве контента в развертывании.</span><span class="sxs-lookup"><span data-stu-id="a83be-117">You can query the deployment service catalog to get a list of updates that can be deployed to devices as content in a deployment.</span></span>

<span data-ttu-id="a83be-118">Ниже приведен пример запроса всех обновлений Windows 10, развертываемых службой развертывания.</span><span class="sxs-lookup"><span data-stu-id="a83be-118">Below is an example of querying for all Windows 10 feature updates that are deployable by the deployment service.</span></span>

### <a name="request"></a><span data-ttu-id="a83be-119">Запрос</span><span class="sxs-lookup"><span data-stu-id="a83be-119">Request</span></span>

```http
GET https://graph.microsoft.com/beta/admin/windows/updates/catalog/entries?$filter=isof('microsoft.graph.windowsUpdates.featureUpdateCatalogEntry')
```

### <a name="response"></a><span data-ttu-id="a83be-120">Отклик</span><span class="sxs-lookup"><span data-stu-id="a83be-120">Response</span></span>

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

## <a name="step-2-create-a-deployment"></a><span data-ttu-id="a83be-121">Шаг 2. Создание развертывания</span><span class="sxs-lookup"><span data-stu-id="a83be-121">Step 2: Create a deployment</span></span>

<span data-ttu-id="a83be-122">[Развертывание](/graph/api/resources/windowsupdates-deployment) указывает содержимое для развертывания, как и когда развертывать контент и целевые устройства.</span><span class="sxs-lookup"><span data-stu-id="a83be-122">A [deployment](/graph/api/resources/windowsupdates-deployment) specifies content to deploy, how and when to deploy the content, and the targeted devices.</span></span> <span data-ttu-id="a83be-123">При развертывании аудитория развертывания автоматически создается в качестве связи.</span><span class="sxs-lookup"><span data-stu-id="a83be-123">When a deployment is created, a deployment audience is automatically created as a relationship.</span></span>

<span data-ttu-id="a83be-124">Ниже приведен пример создания развертывания обновления функций с необязательными настройками расписания развертывания и [правил мониторинга.](windowsupdates-manage-monitoring-rules.md) [](windowsupdates-schedule-deployment.md)</span><span class="sxs-lookup"><span data-stu-id="a83be-124">Below is an example of creating a deployment of a feature update, with optional settings configuring the [deployment schedule](windowsupdates-schedule-deployment.md) and [monitoring rules](windowsupdates-manage-monitoring-rules.md).</span></span> <span data-ttu-id="a83be-125">Целевые устройства указаны на следующем шаге.</span><span class="sxs-lookup"><span data-stu-id="a83be-125">The targeted devices are specified in the next step.</span></span>

> [!NOTE]
> <span data-ttu-id="a83be-126">Если при создании [](/graph/api/resources/windowsupdates-monitoringrule) развертывания не указано правило мониторинга, создается правило мониторинга по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a83be-126">If you do not specify a [monitoring rule](/graph/api/resources/windowsupdates-monitoringrule) when creating a deployment, a default monitoring rule is created.</span></span> <span data-ttu-id="a83be-127">Это правило мониторинга по умолчанию **имеет** сигнал `rollback` , пороговое значение и  `20` **действие** `alertError` .</span><span class="sxs-lookup"><span data-stu-id="a83be-127">This default monitoring rule has a **signal** of `rollback`, a **threshold** of `20`, and an **action** of `alertError`.</span></span> <span data-ttu-id="a83be-128">В будущем обновлении API это поведение изменится и не будет создано правило мониторинга по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a83be-128">In a future update of the API, this behavior will change and a default monitoring rule will not be created.</span></span>

### <a name="request"></a><span data-ttu-id="a83be-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="a83be-129">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="a83be-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="a83be-130">Response</span></span>

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

## <a name="step-3-assign-devices-to-the-deployment-audience"></a><span data-ttu-id="a83be-131">Шаг 3. Назначение устройств аудитории развертывания</span><span class="sxs-lookup"><span data-stu-id="a83be-131">Step 3: Assign devices to the deployment audience</span></span>

<span data-ttu-id="a83be-132">После создания развертывания можно назначить устройства аудитории [развертывания.](/graph/api/resources/windowsupdates-deploymentaudience)</span><span class="sxs-lookup"><span data-stu-id="a83be-132">After a deployment is created, you can assign devices to the [deployment audience](/graph/api/resources/windowsupdates-deploymentaudience).</span></span> <span data-ttu-id="a83be-133">После успешного обновления аудитории развертывания Windows update начинает предлагать обновление соответствующим устройствам в соответствии с настройками развертывания.</span><span class="sxs-lookup"><span data-stu-id="a83be-133">After the deployment audience is successfully updated, Windows Update starts offering the update to the relevant devices according to the deployment settings.</span></span>

<span data-ttu-id="a83be-134">Устройства автоматически регистрируются в службе при добавлении в коллекции участников или исключений аудитории развертывания (то есть объект [azureADDevice](/graph/api/resources/windowsupdates-azureaddevice) автоматически создается, если он еще не существует).</span><span class="sxs-lookup"><span data-stu-id="a83be-134">Devices are automatically registered with the service when added to the members or exclusions collections of a deployment audience (that is, an [azureADDevice](/graph/api/resources/windowsupdates-azureaddevice) object is automatically created if it does not already exist).</span></span>

<span data-ttu-id="a83be-135">В следующем примере показано, как добавлять устройства Azure AD в качестве участников аудитории развертывания.</span><span class="sxs-lookup"><span data-stu-id="a83be-135">The follwoing example shows how to add Azure AD devices as members of the deployment audience.</span></span>

### <a name="request"></a><span data-ttu-id="a83be-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="a83be-136">Request</span></span>

```http
POST https://graph.microsoft.com/beta/admin/windows/updates/deployments/{deploymentId}/audience/updateAudience
Content-type: application/json

{
    "addMembers": [
        {
            "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
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
    ]
}
```

### <a name="response"></a><span data-ttu-id="a83be-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="a83be-137">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

## <a name="during-a-deployment"></a><span data-ttu-id="a83be-138">Во время развертывания</span><span class="sxs-lookup"><span data-stu-id="a83be-138">During a deployment</span></span>

<span data-ttu-id="a83be-139">Во время развертывания можно приостановить развертывание, обновив его **состояние,** а также обновив членов аудитории и исключения.</span><span class="sxs-lookup"><span data-stu-id="a83be-139">While a deployment is in progress, you can pause the deployment by updating its **state**, as well as update its audience members and exclusions.</span></span>

## <a name="after-a-deployment"></a><span data-ttu-id="a83be-140">После развертывания</span><span class="sxs-lookup"><span data-stu-id="a83be-140">After a deployment</span></span>

<span data-ttu-id="a83be-141">После того как все устройства, заданные аудитории развертывания, были первоначально предложены обновления, возможно, что не все устройства начали или завершили обновление из-за таких факторов, как подключение к устройству.</span><span class="sxs-lookup"><span data-stu-id="a83be-141">After all devices assigned to a deployment audience have been initially offered the update, it is possible that not all devices have started or completed the update, due to factors like device connectivity.</span></span> <span data-ttu-id="a83be-142">До тех пор, пока развертывание еще существует, Windows update продолжает предлагать обновление для назначенного устройства всякий раз, когда они снова подключены.</span><span class="sxs-lookup"><span data-stu-id="a83be-142">As long as the deployment still exists, Windows Update continues to offer the update to the assigned devices whenever they reconnect.</span></span>

