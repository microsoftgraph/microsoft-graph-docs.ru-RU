---
title: Развертывание ускоренного обновления системы безопасности с помощью службы клиентский компонент Центра обновления Windows для бизнеса
description: Выполните следующие действия, чтобы развернуть ускоренное обновление системы безопасности Windows на устройствах в клиенте Azure AD в случае экстренного реагирования с помощью службы развертывания клиентский компонент Центра обновления Windows для бизнеса.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: c0c8d0389c2d152ebc4323639c0b8494927f89e7
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66444217"
---
# <a name="deploy-an-expedited-security-update-using-the-windows-update-for-business-deployment-service"></a>Развертывание ускоренного обновления системы безопасности с помощью службы клиентский компонент Центра обновления Windows для бизнеса

С помощью клиентский компонент Центра обновления Windows развертывания для бизнеса можно развертывать обновления Windows на устройствах в Azure AD клиента. В настоящее время служба развертывания поддерживает [развертывание](windowsupdates-deployments.md) Windows 10 обновлений компонентов и ускоренного обновления системы безопасности. В этом разделе основное внимание уделяется развертыванию ускоренного обновления системы безопасности. Сведения о развертывании обновлений компонентов см. в разделе ["Развертывание обновления компонентов"](windowsupdates-deploy-update.md).

Ускорение обновления системы безопасности переопределяет клиентский компонент Центра обновления Windows для бизнеса, чтобы обновление устанавливались как можно быстрее. Это может быть полезно, когда возникают критические события безопасности, и вам нужно развертывать последние обновления более быстро, чем обычно. Тем не менее, хотя это может помочь достичь целей соответствия для определенного обновления безопасности, оно не предназначено для использования каждый месяц. Вместо этого рекомендуется использовать [крайние сроки соответствия для обновлений](/windows/deployment/update/wufb-compliancedeadlines).

При развертывании ускоренного обновления системы безопасности на устройстве клиентский компонент Центра обновления Windows предлагает последнее применимое обновление для устройства, если оно еще не получило обновление с указанной датой выпуска. Например, если развернуть обновление Windows 10 безопасности, выпущенное 13 апреля 2021 г., на устройстве, которое в настоящее время не имеет обновления, устройство получит ускоренное обновление. Если устройство уже имеет указанное или более позднее обновление, оно не получает ускоренное обновление.

Ускоренные обновления для системы безопасности также обладают следующими характеристиками.

* Обновление начинается сразу, а не ожидает следующей регулярной проверки наличия обновлений, которая выполняется каждые 22 часа по умолчанию.
* Обновление скачивается и устанавливается максимально быстро.
* Процесс обновления переопределяет настроенные параметры политики устройства, например дни до принудительной перезагрузки устройства. После установки ускоренного обновления устройство возвращается к текущим параметрам политики.

## <a name="prerequisites"></a>Предварительные требования

* Устройства соответствуют [предварительным требованиям для службы развертывания](windowsupdates-concept-overview.md#prerequisites).
* Устройства установили обновление, описанное в статье ["KB4023057 — обновление](https://support.microsoft.com/topic/kb4023057-update-for-windows-10-update-service-components-fccad0ca-dc10-2e46-9ed1-7e392450fb3a) для компонентов Windows 10 обновления (или более поздней версии)".

## <a name="step-1-optional-get-a-list-of-expeditable-updates"></a>Шаг 1. Получение списка ускоряемых обновлений (необязательно)

Вы можете запросить каталог служб развертывания, чтобы получить список обновлений, которые можно ускорить на устройствах в качестве содержимого в развертывании.

Обновления системы безопасности представлены типом [qualityUpdateCatalogEntry](/graph/api/resources/windowsupdates-qualityupdatecatalogentry) с **qualityUpdateClassification** .`security` Все Windows 10 исправления, которые классифицируются как обновления безопасности, можно ускорить и пометить с помощью свойства **isExpeditable** `true` для их идентификации.

Ниже приведен пример запроса всех обновлений Windows 10 безопасности, которые могут быть развернуты службой развертывания в качестве ускоренного обновления. Корпорация Майкрософт рекомендует показывать только три последних обновления, поэтому пример включает в себя `$top=3`.

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

[Развертывание](/graph/api/resources/windowsupdates-deployment) определяет содержимое для развертывания, способ и время развертывания содержимого и целевых устройств. Для исправлений содержимое указывается с использованием целевой даты соответствия. При создании развертывания аудитория развертывания автоматически создается как связь.

При развертывании ускоренного обновления системы безопасности на устройстве клиентский компонент Центра обновления Windows предлагает обновление, которое переводит устройство выше заданного минимального уровня соответствия. В зависимости от того, когда каждое устройство сканирует и обновляется, некоторые устройства могут получать более новые обновления (например, если имеется более новое обновление безопасности, чем обновление, соответствующее требуемого минимальному уровню соответствия), но все устройства соответствуют указанному стандарту соответствия обновлений безопасности. Такое поведение при предложении последнего применимого обновления, означаемое свойством **equivalentContent**`latestSecurity`, заданным значением по умолчанию, помогает обеспечить безопасность устройств и не позволяет устройству получать ускоренное обновление, за которым следует другое регулярное обновление всего несколько дней спустя.

Вы можете настроить льготный период перезапуска устройства с помощью свойства **daysUntilForcedReboot** в параметрах пользовательского интерфейса развертывания.[](/graph/api/resources/windowsupdates-userexperiencesettings) Льготный период задает период времени после установки, в течение которого пользователь может управлять временем перезапуска устройства. Если устройство не было перезапущено к истечении льготного периода, оно перезапускается автоматически.

Ниже приведен пример создания развертывания для ускоренного обновления качества. Целевые устройства будут указаны на следующем шаге.

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

После создания развертывания можно назначить устройства [аудитории развертывания](/graph/api/resources/windowsupdates-deploymentaudience). После успешного обновления аудитории развертывания клиентский компонент Центра обновления Windows предлагать обновление соответствующим устройствам в соответствии с параметрами развертывания.

Устройства автоматически регистрируются в службе при добавлении в коллекции элементов или исключений аудитории развертывания (то есть объект [azureADDevice](/graph/api/resources/windowsupdates-azureaddevice) создается автоматически, если он еще не существует).

В следующем примере показано, как Azure AD устройств в качестве участников аудитории развертывания.

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

Во время развертывания можно приостановить развертывание, обновив его **состояние, а** также обновив участников аудитории и исключения.

## <a name="after-a-deployment"></a>После развертывания

После того как всем устройствам, назначенным аудитории развертывания, было изначально предложено обновление, возможно, не все устройства начали или завершили обновление из-за таких факторов, как подключение устройств. Пока развертывание по-прежнему существует, оно продолжает клиентский компонент Центра обновления Windows предлагать обновление назначенным устройствам при каждом повторном подключении.
