---
title: Развертывание ускоренного обновления безопасности с Windows службы развертывания для бизнеса
description: С помощью службы Windows обновления для бизнеса можно развернуть ускоренные обновления Windows безопасности на устройствах в клиенте Azure AD в случае возникновения чрезвычайной ситуации и необходимо немедленно развернуть обновление безопасности.
author: Alice-at-Microsoft
ms.localizationpriority: medium
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 855f123fbd81d19f17dca6e436586365a0b221a5
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60688628"
---
# <a name="deploy-an-expedited-security-update-using-the-windows-update-for-business-deployment-service"></a>Развертывание ускоренного обновления безопасности с Windows службы развертывания для бизнеса

С помощью Windows обновления для бизнеса можно развернуть Windows на устройствах в клиенте Azure AD. Сегодня служба развертывания поддерживает развертывание [Windows 10](windowsupdates-deployments.md) обновлений функций и ускоренные обновления безопасности. В этом разделе основное внимание уделяется развертыванию ускоряемого обновления безопасности. Сведения о развертывании обновлений функций см. в дополнительных [сведениях о развертывании обновления функций.](windowsupdates-deploy-update.md)

Ускорение обновления безопасности переопределяет Windows политики отсрочки для бизнеса, чтобы обновление было установлено как можно быстрее. Это может быть полезно при критически важных событиях безопасности, и вам необходимо развертывать последние обновления быстрее, чем обычно. Однако, хотя это может помочь достичь целей соответствия требованиям в отношении определенного обновления безопасности, оно не предназначено для использования каждый месяц. Вместо этого рассмотрите возможность использования [сроков соответствия требованиям для обновлений.](/windows/deployment/update/wufb-compliancedeadlines)

При развертывании ускоренного обновления безопасности на устройстве Windows update предлагает последнее применимое обновление для устройства, если оно еще не получило обновление с указанной датой выпуска. Например, при развертывании обновления Windows 10 безопасности, выпущенного 13 апреля 2021 г. на устройстве, которое в настоящее время не имеет обновления, устройство получает ускоренное обновление. Если устройство уже имеет указанное обновление или более новое, оно не получает ускоренного обновления.

Ускоренные обновления безопасности также имеют следующие характеристики:

* Обновление начинается сразу, а не ожидает следующего регулярного сканирования обновлений, которое происходит раз в 22 часа по умолчанию.
* Обновление загружается и устанавливается как можно быстрее.
* Процесс обновления переопределяет настроенные параметры политики устройства, например дни, пока устройство не будет вынуждено перезапуститься. После установки ускоренного обновления устройство возвращается в текущие параметры политики.

## <a name="prerequisites"></a>Предварительные требования

* Устройства отвечают [необходимым требованиям для службы развертывания.](windowsupdates-concept-overview.md#prerequisites)
* Устройства установили обновление, описанное в [KB4023057 .](https://support.microsoft.com/topic/kb4023057-update-for-windows-10-update-service-components-fccad0ca-dc10-2e46-9ed1-7e392450fb3a) Обновление для компонентов службы Windows 10 обновления (или более новых).

## <a name="step-1-optional-get-a-list-of-expeditable-updates"></a>Шаг 1. (Необязательный) Получить список оперативных обновлений

Вы можете запрашивать каталог службы развертывания, чтобы получить список обновлений, которые можно ускорить на устройствах в качестве контента в развертывании.

Обновления безопасности представляются [типом qualityUpdateCatalogEntry](/graph/api/resources/windowsupdates-qualityupdatecatalogentry) с **qualityUpdateClassification** `security` . Все Windows 10 обновления качества, классифицируемые как обновления безопасности, могут быть ускорены и помечены свойством **isExpeditable** для `true` их идентификации.

Ниже приведен пример запроса всех обновлений Windows 10 безопасности, которые могут быть развернуты службой развертывания в качестве ускоряющих обновлений. Корпорация Майкрософт рекомендует показывать только три наиболее актуальных обновления, поэтому в пример входит `$top=3` .

### <a name="request"></a>Запрос

```http
GET https://graph.microsoft.com/beta/admin/windows/updates/catalog/entries?$top=3&$filter=isof('microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry') and microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry/isExpeditable eq true&$orderby=releaseDateTime desc
```

### <a name="response"></a>Отклик

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

## <a name="step-2-create-a-deployment"></a>Шаг 2. Создание развертывания

[Развертывание](/graph/api/resources/windowsupdates-deployment) указывает содержимое для развертывания, как и когда развертывать контент и целевые устройства. Для обновления качества контент указывается с помощью целевой даты соответствия требованиям. При развертывании аудитория развертывания автоматически создается в качестве связи.

При развертывании ускоренного обновления безопасности на устройстве Windows update предлагает обновление, которое приводит устройство выше установленного минимального уровня соответствия требованиям. В зависимости от того, когда каждое устройство сканирует и обновляется, некоторые устройства могут получать более новые обновления (например, если имеется более новое обновление безопасности, чем обновление, соответствующее необходимому минимальному уровню соответствия требованиям), но все устройства соответствуют указанному стандарту соответствия требованиям безопасности. Такое поведение при предложении последнего применимого обновления, на которое указывает эквивалент **свойстваContent,** задающий значение по умолчанию, помогает обеспечить безопасность устройств и не позволяет устройству получать ускоренное обновление, за которым следует еще одно регулярное обновление всего несколько дней `latestSecurity` спустя.

Вы можете настроить период отсрочки перезапуска устройства с помощью свойств [](/graph/api/resources/windowsupdates-userexperiencesettings) **daysUntilForcedReboot** в параметрах пользовательского интерфейса развертывания. Период льготы задает время после установки, которое пользователь может контролировать при перезапуске устройства. Если устройство не перезапустилось к истечении срока действия льготного периода, оно перезапускает автоматически.

Ниже приведен пример создания развертывания для ускоренного обновления качества. Целевые устройства указаны на следующем шаге.

### <a name="request"></a>Запрос

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
        "rollout": null,
        "safeguard": null
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
}
```

## <a name="step-3-assign-devices-to-the-deployment-audience"></a>Шаг 3. Назначение устройств аудитории развертывания

После создания развертывания можно назначить устройства аудитории [развертывания.](/graph/api/resources/windowsupdates-deploymentaudience) После успешного обновления аудитории развертывания Windows update начинает предлагать обновление соответствующим устройствам в соответствии с настройками развертывания.

Устройства автоматически регистрируются в службе при добавлении в коллекции участников или исключений аудитории развертывания (то есть объект [azureADDevice](/graph/api/resources/windowsupdates-azureaddevice) автоматически создается, если он еще не существует).

В следующем примере показано, как добавлять устройства Azure AD в качестве участников аудитории развертывания.

### <a name="request"></a>Запрос

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

### <a name="response"></a>Отклик

```http
HTTP/1.1 202 Accepted
```

## <a name="during-a-deployment"></a>Во время развертывания

Во время развертывания можно приостановить развертывание, обновив его **состояние,** а также обновив членов аудитории и исключения.

## <a name="after-a-deployment"></a>После развертывания

После того как все устройства, заданные аудитории развертывания, были первоначально предложены обновления, возможно, что не все устройства начали или завершили обновление из-за таких факторов, как подключение к устройству. До тех пор, пока развертывание все еще существует, он по-прежнему Windows обновления предлагает обновление для назначенного устройства при повторном подключении.
