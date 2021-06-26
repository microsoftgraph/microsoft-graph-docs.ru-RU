---
title: Развертывание ускоренного обновления безопасности с Windows службы развертывания для бизнеса
description: С помощью службы Windows обновления для бизнеса можно развернуть ускоренные обновления Windows безопасности на устройствах в клиенте Azure AD в случае возникновения чрезвычайной ситуации и необходимо немедленно развернуть обновление безопасности.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 58dfdb7a260d2381b05332914fe71f9948c87e17
ms.sourcegitcommit: 0ca0a1e2810701c2392e5c685e984fbfb6785579
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2021
ms.locfileid: "53151596"
---
# <a name="deploy-an-expedited-security-update-using-the-windows-update-for-business-deployment-service"></a><span data-ttu-id="008ab-103">Развертывание ускоренного обновления безопасности с Windows службы развертывания для бизнеса</span><span class="sxs-lookup"><span data-stu-id="008ab-103">Deploy an expedited security update using the Windows Update for Business deployment service</span></span>

<span data-ttu-id="008ab-104">С помощью Windows обновления для бизнеса можно развернуть Windows на устройствах в клиенте Azure AD.</span><span class="sxs-lookup"><span data-stu-id="008ab-104">With the Windows Update for Business deployment service, you can deploy Windows updates to devices in an Azure AD tenant.</span></span> <span data-ttu-id="008ab-105">Сегодня служба развертывания поддерживает развертывание [Windows 10](windowsupdates-deployments.md) обновлений функций и ускоренные обновления безопасности.</span><span class="sxs-lookup"><span data-stu-id="008ab-105">Today, the deployment service supports [deployments](windowsupdates-deployments.md) of Windows 10 feature updates and expedited security updates.</span></span> <span data-ttu-id="008ab-106">В этом разделе основное внимание уделяется развертыванию ускоряемого обновления безопасности.</span><span class="sxs-lookup"><span data-stu-id="008ab-106">This topic focuses on deployments of expedited security updates.</span></span> <span data-ttu-id="008ab-107">Сведения о развертывании обновлений функций см. в дополнительных [сведениях о развертывании обновления функций.](windowsupdates-deploy-update.md)</span><span class="sxs-lookup"><span data-stu-id="008ab-107">For information on deploying feature updates, see [Deploy a feature update](windowsupdates-deploy-update.md).</span></span>

<span data-ttu-id="008ab-108">Ускорение обновления безопасности переопределяет Windows политики отсрочки для бизнеса, чтобы обновление было установлено как можно быстрее.</span><span class="sxs-lookup"><span data-stu-id="008ab-108">Expediting a security update overrides Windows Update for Business deferral policies so that the update is installed as quickly as possible.</span></span> <span data-ttu-id="008ab-109">Это может быть полезно при критически важных событиях безопасности, и вам необходимо развертывать последние обновления быстрее, чем обычно.</span><span class="sxs-lookup"><span data-stu-id="008ab-109">It can be useful when critical security events arise and you need to deploy the latest updates more rapidly than normal.</span></span> <span data-ttu-id="008ab-110">Однако, хотя это может помочь достичь целей соответствия требованиям в отношении определенного обновления безопасности, оно не предназначено для использования каждый месяц.</span><span class="sxs-lookup"><span data-stu-id="008ab-110">However, while it can help to achieve compliance targets against a specific security update, it is not designed to be used every month.</span></span> <span data-ttu-id="008ab-111">Вместо этого рассмотрите возможность использования [сроков соответствия требованиям для обновлений.](https://docs.microsoft.com/windows/deployment/update/wufb-compliancedeadlines)</span><span class="sxs-lookup"><span data-stu-id="008ab-111">Instead, consider using [compliance deadlines for updates](https://docs.microsoft.com/windows/deployment/update/wufb-compliancedeadlines).</span></span>

<span data-ttu-id="008ab-112">При развертывании ускоренного обновления безопасности на устройстве Windows update предлагает последнее применимое обновление для устройства, если оно еще не получило обновление с указанной датой выпуска.</span><span class="sxs-lookup"><span data-stu-id="008ab-112">When you deploy an expedited security update to a device, Windows Update offers the latest applicable update to the device if it has not yet received the update with the specified release date.</span></span> <span data-ttu-id="008ab-113">Например, при развертывании обновления Windows 10 безопасности, выпущенного 13 апреля 2021 г. на устройстве, которое в настоящее время не имеет обновления, устройство получает ускоренное обновление.</span><span class="sxs-lookup"><span data-stu-id="008ab-113">For example, if you deploy the Windows 10 security update released on April 13, 2021 to a device that does not currently have the update, the device receives an expedited update.</span></span> <span data-ttu-id="008ab-114">Если устройство уже имеет указанное обновление или более новое, оно не получает ускоренного обновления.</span><span class="sxs-lookup"><span data-stu-id="008ab-114">If the device already has the specified update or newer, it does not receive an expedited update.</span></span>

<span data-ttu-id="008ab-115">Ускоренные обновления безопасности также имеют следующие характеристики:</span><span class="sxs-lookup"><span data-stu-id="008ab-115">Expedited security updates also have the following characteristics:</span></span>

* <span data-ttu-id="008ab-116">Обновление начинается сразу, а не ожидает следующего регулярного сканирования обновлений, которое происходит раз в 22 часа по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="008ab-116">The update starts right away rather than waiting for the next regular update scan, which occurs once every 22 hours by default.</span></span>
* <span data-ttu-id="008ab-117">Обновление загружается и устанавливается как можно быстрее.</span><span class="sxs-lookup"><span data-stu-id="008ab-117">The update downloads and installs as quickly as possible.</span></span>
* <span data-ttu-id="008ab-118">Процесс обновления переопределяет настроенные параметры политики устройства, например дни, пока устройство не будет вынуждено перезапуститься.</span><span class="sxs-lookup"><span data-stu-id="008ab-118">The update process overrides configured device policy settings, such as days until the device is forced to restart.</span></span> <span data-ttu-id="008ab-119">После установки ускоренного обновления устройство возвращается в текущие параметры политики.</span><span class="sxs-lookup"><span data-stu-id="008ab-119">After the expedited update is installed, the device returns to the current policy settings.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="008ab-120">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="008ab-120">Prerequisites</span></span>

* <span data-ttu-id="008ab-121">Устройства отвечают [необходимым требованиям для службы развертывания.](windowsupdates-concept-overview.md#prerequisites)</span><span class="sxs-lookup"><span data-stu-id="008ab-121">Devices meet the [prerequisites for the deployment service](windowsupdates-concept-overview.md#prerequisites).</span></span>
* <span data-ttu-id="008ab-122">Устройства установили обновление, описанное в [KB4023057 .](https://support.microsoft.com/topic/kb4023057-update-for-windows-10-update-service-components-fccad0ca-dc10-2e46-9ed1-7e392450fb3a) Обновление для компонентов службы Windows 10 обновления (или более новых).</span><span class="sxs-lookup"><span data-stu-id="008ab-122">Devices have installed the update described in [KB4023057 - Update for Windows 10 Update Service components](https://support.microsoft.com/topic/kb4023057-update-for-windows-10-update-service-components-fccad0ca-dc10-2e46-9ed1-7e392450fb3a) (or newer).</span></span>

## <a name="step-1-optional-get-a-list-of-expeditable-updates"></a><span data-ttu-id="008ab-123">Шаг 1. (Необязательный) Получить список оперативных обновлений</span><span class="sxs-lookup"><span data-stu-id="008ab-123">Step 1: (Optional) Get a list of expeditable updates</span></span>

<span data-ttu-id="008ab-124">Вы можете запрашивать каталог службы развертывания, чтобы получить список обновлений, которые можно ускорить на устройствах в качестве контента в развертывании.</span><span class="sxs-lookup"><span data-stu-id="008ab-124">You can query the deployment service catalog to get a list of updates that can be expedited to devices as content in a deployment.</span></span>

<span data-ttu-id="008ab-125">Обновления безопасности представляются [типом qualityUpdateCatalogEntry](/graph/api/resources/windowsupdates-qualityupdatecatalogentry) с **qualityUpdateClassification** `security` .</span><span class="sxs-lookup"><span data-stu-id="008ab-125">Security updates are represented by the [qualityUpdateCatalogEntry](/graph/api/resources/windowsupdates-qualityupdatecatalogentry) type, with a **qualityUpdateClassification** of `security`.</span></span> <span data-ttu-id="008ab-126">Все Windows 10 обновления качества, классифицируемые как обновления безопасности, могут быть ускорены и помечены свойством **isExpeditable** для `true` их идентификации.</span><span class="sxs-lookup"><span data-stu-id="008ab-126">All Windows 10 quality updates that are classified as security updates can be expedited and are tagged with the **isExpeditable** property set to `true` to identify them.</span></span>

<span data-ttu-id="008ab-127">Ниже приведен пример запроса всех обновлений Windows 10 безопасности, которые могут быть развернуты службой развертывания в качестве ускоряющих обновлений.</span><span class="sxs-lookup"><span data-stu-id="008ab-127">Below is an example of querying for all Windows 10 security updates that can be deployed as expedited updates by the deployment service.</span></span> <span data-ttu-id="008ab-128">Корпорация Майкрософт рекомендует показывать только три наиболее актуальных обновления, поэтому в пример входит `$top=3` .</span><span class="sxs-lookup"><span data-stu-id="008ab-128">Microsoft recommends to only show the three most current updates, so the example includes `$top=3`.</span></span>

### <a name="request"></a><span data-ttu-id="008ab-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="008ab-129">Request</span></span>

```http
GET https://graph.microsoft.com/beta/admin/windows/updates/catalog/entries?$top=3&$filter=isof('microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry') and microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry/isExpeditable eq true&$orderby=releaseDateTime desc
```

### <a name="response"></a><span data-ttu-id="008ab-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="008ab-130">Response</span></span>

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "value": [
        {
            "@odata.type": "#microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry",
            "id": "bd9554dc-2737-4e3c-b794-fa2b8b3f4a30",
            "displayName": "MM/DD/YYYY - YYYY.MM B Security Updates for Windows 10",
            "releaseDateTime": "String (timestamp)",
            "deployableUntilDateTime": null,
            "isExpeditable": true,
            "qualityUpdateClassification": "security"
        },
        {
            "@odata.type": "#microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry",
            "id": "68860630-c2d0-4dd2-8c4b-9b9737ee5081",
            "displayName": "MM/DD/YYYY - YYYY.MM B Security Updates for Windows 10",
            "releaseDateTime": "String (timestamp)",
            "deployableUntilDateTime": null,
            "isExpeditable": true,
            "qualityUpdateClassification": "security"
        },
        {
            "@odata.type": "#microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry",
            "id": "aa336b13-db33-4d94-89ea-90e43e4ad30b",
            "displayName": "MM/DD/YYYY - YYYY.MM B Security Updates for Windows 10",
            "releaseDateTime": "String (timestamp)",
            "deployableUntilDateTime": null,
            "isExpeditable": true,
            "qualityUpdateClassification": "security"
        }
    ]
}
```

## <a name="step-2-create-a-deployment"></a><span data-ttu-id="008ab-131">Шаг 2. Создание развертывания</span><span class="sxs-lookup"><span data-stu-id="008ab-131">Step 2: Create a deployment</span></span>

> [!NOTE]
> <span data-ttu-id="008ab-132">При первом развертывании ускоренного обновления безопасности в клиенте при настройке службы для организации может возникнуть задержка на один день.</span><span class="sxs-lookup"><span data-stu-id="008ab-132">The first time you deploy an expedited security update in your tenant, you may experience up to a one-day delay while the service is configured for your organization.</span></span> <span data-ttu-id="008ab-133">Эта задержка не применяется к последующим развертываниям или развертываниям обновлений функций и будет устранена в будущем обновлении.</span><span class="sxs-lookup"><span data-stu-id="008ab-133">This delay does not apply to subsequent deployments or deployments of feature updates, and will be addressed in a future update.</span></span>

<span data-ttu-id="008ab-134">[Развертывание](/graph/api/resources/windowsupdates-deployment) указывает содержимое для развертывания, как и когда развертывать контент и целевые устройства.</span><span class="sxs-lookup"><span data-stu-id="008ab-134">A [deployment](/graph/api/resources/windowsupdates-deployment) specifies content to deploy, how and when to deploy the content, and the targeted devices.</span></span> <span data-ttu-id="008ab-135">Для обновления качества контент указывается с помощью целевой даты соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="008ab-135">For quality updates, the content is specified using a target compliance date.</span></span> <span data-ttu-id="008ab-136">При развертывании аудитория развертывания автоматически создается в качестве связи.</span><span class="sxs-lookup"><span data-stu-id="008ab-136">When a deployment is created, a deployment audience is automatically created as a relationship.</span></span>

<span data-ttu-id="008ab-137">При развертывании ускоренного обновления безопасности на устройстве Windows update предлагает обновление, которое приводит устройство выше установленного минимального уровня соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="008ab-137">When you deploy an expedited security update to a device, Windows Update offers an update that brings the device above the minimum compliance level specified.</span></span> <span data-ttu-id="008ab-138">В зависимости от того, когда каждое устройство сканирует и обновляется, некоторые устройства могут получать более новые обновления (например, если имеется более новое обновление безопасности, чем обновление, соответствующее необходимому минимальному уровню соответствия требованиям), но все устройства соответствуют указанному стандарту соответствия требованиям безопасности.</span><span class="sxs-lookup"><span data-stu-id="008ab-138">Depending on when each device scans and updates, some devices may receive newer updates (e.g. if there is a newer security update than the one corresponding to the desired minimum compliance level), but all devices meet the specified security update compliance standard.</span></span> <span data-ttu-id="008ab-139">Такое поведение при предложении последнего применимого обновления, на которое указывает эквивалент **свойстваContent,** задающий значение по умолчанию, помогает обеспечить безопасность устройств и не позволяет устройству получать ускоренное обновление, за которым следует еще одно регулярное обновление всего несколько дней `latestSecurity` спустя.</span><span class="sxs-lookup"><span data-stu-id="008ab-139">This behavior of offering the latest applicable update, indicated by the property **equivalentContent** being set to the default value `latestSecurity`, helps keep devices as secure as possible and prevents a device from receiving an expedited update followed by another regular update just days later.</span></span>

<span data-ttu-id="008ab-140">Вы можете настроить период отсрочки перезапуска устройства с помощью свойств [](/graph/api/resources/windowsupdates-userexperiencesettings) **daysUntilForcedReboot** в параметрах пользовательского интерфейса развертывания.</span><span class="sxs-lookup"><span data-stu-id="008ab-140">You can configure the device restart grace period using the property **daysUntilForcedReboot** in the [user experience settings](/graph/api/resources/windowsupdates-userexperiencesettings) of the deployment.</span></span> <span data-ttu-id="008ab-141">Период льготы задает время после установки, которое пользователь может контролировать при перезапуске устройства.</span><span class="sxs-lookup"><span data-stu-id="008ab-141">The grace period sets the amount of time after installation that the user can control the timing of when the device restarts.</span></span> <span data-ttu-id="008ab-142">Если устройство не перезапустилось к истечении срока действия льготного периода, оно перезапускает автоматически.</span><span class="sxs-lookup"><span data-stu-id="008ab-142">If the device has not restarted by the time the grace period expires, it restarts automatically.</span></span>

<span data-ttu-id="008ab-143">Ниже приведен пример создания развертывания для ускоренного обновления качества.</span><span class="sxs-lookup"><span data-stu-id="008ab-143">Below is an example of creating a deployment for an expedited quality update.</span></span> <span data-ttu-id="008ab-144">Целевые устройства указаны на следующем шаге.</span><span class="sxs-lookup"><span data-stu-id="008ab-144">The targeted devices are specified in the next step.</span></span>

### <a name="request"></a><span data-ttu-id="008ab-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="008ab-145">Request</span></span>

```http
POST https://graph.microsoft.com/beta/admin/windows/updates/deployments
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
    "content": {
        "@odata.type": "microsoft.graph.windowsUpdates.expeditedQualityUpdateReference",
        "releaseDate": "YYYY-MM-DD"
    },
    "settings": {
        "@odata.type": "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
        "userExperience": {
            "daysUntilForcedReboot": 2
        }
    }
}
```

### <a name="response"></a><span data-ttu-id="008ab-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="008ab-146">Response</span></span>

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
        "@odata.type": "microsoft.graph.windowsUpdates.expeditedQualityUpdateReference",
        "releaseDate": "YYYY-MM-DDT00:00:00Z",
        "classification": "security",
        "equivalentContent": "latestSecurity"
    },
    "settings": {
        "@odata.type": "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
        "userExperience": {
            "daysUntilForcedReboot": 2
        },
        "monitoring": null,
        "rollout": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```

## <a name="step-3-assign-devices-to-the-deployment-audience"></a><span data-ttu-id="008ab-147">Шаг 3. Назначение устройств аудитории развертывания</span><span class="sxs-lookup"><span data-stu-id="008ab-147">Step 3: Assign devices to the deployment audience</span></span>

<span data-ttu-id="008ab-148">После создания развертывания можно назначить устройства аудитории [развертывания.](/graph/api/resources/windowsupdates-deploymentaudience)</span><span class="sxs-lookup"><span data-stu-id="008ab-148">After a deployment is created, you can assign devices to the [deployment audience](/graph/api/resources/windowsupdates-deploymentaudience).</span></span> <span data-ttu-id="008ab-149">После успешного обновления аудитории развертывания Windows update начинает предлагать обновление соответствующим устройствам в соответствии с настройками развертывания.</span><span class="sxs-lookup"><span data-stu-id="008ab-149">When the deployment audience is successfully updated, Windows Update starts offering the update to the relevant devices according to the deployment settings.</span></span>

<span data-ttu-id="008ab-150">Устройства автоматически регистрируются в службе при добавлении в коллекции участников или исключений аудитории развертывания (то есть объект [azureADDevice](/graph/api/resources/windowsupdates-azureaddevice) автоматически создается, если он еще не существует).</span><span class="sxs-lookup"><span data-stu-id="008ab-150">Devices are automatically registered with the service when added to the members or exclusions collections of a deployment audience (that is, an [azureADDevice](/graph/api/resources/windowsupdates-azureaddevice) object is automatically created if it does not already exist).</span></span>

<span data-ttu-id="008ab-151">В следующем примере показано, как добавлять устройства Azure AD в качестве участников аудитории развертывания.</span><span class="sxs-lookup"><span data-stu-id="008ab-151">The following example shows how to add Azure AD devices as members of the deployment audience.</span></span>

### <a name="request"></a><span data-ttu-id="008ab-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="008ab-152">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="008ab-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="008ab-153">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

## <a name="during-a-deployment"></a><span data-ttu-id="008ab-154">Во время развертывания</span><span class="sxs-lookup"><span data-stu-id="008ab-154">During a deployment</span></span>

<span data-ttu-id="008ab-155">Во время развертывания можно приостановить развертывание, обновив его **состояние,** а также обновив членов аудитории и исключения.</span><span class="sxs-lookup"><span data-stu-id="008ab-155">While a deployment is in progress, you can pause the deployment by updating its **state**, as well as update its audience members and exclusions.</span></span>

## <a name="after-a-deployment"></a><span data-ttu-id="008ab-156">После развертывания</span><span class="sxs-lookup"><span data-stu-id="008ab-156">After a deployment</span></span>

<span data-ttu-id="008ab-157">После того как все устройства, заданные аудитории развертывания, были первоначально предложены обновления, возможно, что не все устройства начали или завершили обновление из-за таких факторов, как подключение к устройству.</span><span class="sxs-lookup"><span data-stu-id="008ab-157">After all devices assigned to a deployment audience have been initially offered the update, it is possible that not all devices have started or completed the update, due to factors like device connectivity.</span></span> <span data-ttu-id="008ab-158">До тех пор, пока развертывание все еще существует, он по-прежнему Windows обновления предлагает обновление для назначенного устройства при повторном подключении.</span><span class="sxs-lookup"><span data-stu-id="008ab-158">As long as the deployment still exists, it continues to make sure that Windows Update is offering the update to the assigned devices whenever they reconnect.</span></span>
