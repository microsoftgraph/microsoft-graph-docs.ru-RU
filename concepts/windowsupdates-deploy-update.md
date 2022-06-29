---
title: Развертывание обновления компонентов с помощью службы клиентский компонент Центра обновления Windows для бизнеса
description: Выполните следующие действия, чтобы развернуть обновления компонентов Windows на устройствах в клиенте Azure AD с помощью службы клиентский компонент Центра обновления Windows для бизнеса.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 176d4c07348b367bfe02335617ebae3328573907
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437508"
---
# <a name="deploy-a-feature-update-using-the-windows-update-for-business-deployment-service"></a>Развертывание обновления компонентов с помощью службы клиентский компонент Центра обновления Windows для бизнеса

С помощью клиентский компонент Центра обновления Windows развертывания для бизнеса можно развертывать обновления Windows на устройствах в Azure AD клиента. В настоящее время служба развертывания поддерживает [развертывание](windowsupdates-deployments.md) Windows 10 обновлений компонентов и ускоренного обновления системы безопасности. В этом разделе основное внимание уделяется развертываниям обновлений компонентов. Сведения о развертывании ускоренного обновления системы безопасности см. в статье ["Развертывание ускоренного обновления системы безопасности"](windowsupdates-deploy-expedited-update.md).

При развертывании обновления компонентов на устройстве клиентский компонент Центра обновления Windows указанное обновление для устройства, если оно еще не получило обновление. Например, при развертывании Windows 10 версии 20H2 на устройстве, которое зарегистрировано в управлении обновлениями компонентов и в настоящее время используется более ранняя версия Windows 10, устройство обновляется до версии 20H2. Если устройство уже установлено в версии 20H2 или выше, она остается в текущей версии. Если устройство не зарегистрировано в управлении обновлениями компонентов, эта операция не влияет на устройство.

Пока устройство остается зарегистрированным в управлении обновлениями компонентов, оно не получает никаких других обновлений компонентов от клиентский компонент Центра обновления Windows если оно не развернуто явным образом с помощью службы развертывания.

> [!IMPORTANT]
> Используя службу развертывания клиентский компонент Центра обновления Windows для бизнеса для обновления устройств до Windows 11 (путем установки параметра версии развертывания на "Windows 11, версия 21H2"), вы соглашаетесь с тем, что при применении этой операционной системы к устройству (1) применимая лицензия Windows была приобретена в том же объеме.  лицензирование или (2) вы имеете право на привязку организации и принимаете от ее имени соответствующие условия лицензионного соглашения на использование программного обеспечения Майкрософт, которые можно найти здесь: [Условия](https://www.microsoft.com/Useterms) лицензионного соглашения на использование программного обеспечения Майкрософт.

## <a name="prerequisites"></a>Предварительные требования

* Устройства соответствуют [предварительным требованиям для службы развертывания](windowsupdates-concept-overview.md#prerequisites).
* Прежде чем использовать службу развертывания для развертывания обновлений компонентов, устройства должны быть зарегистрированы в службе развертывания для категории обновления компонентов.[](windowsupdates-enroll.md)

## <a name="step-1-optional-get-a-list-of-deployable-updates"></a>Шаг 1. Получение списка развертываемых обновлений (необязательно)

Вы можете запросить каталог служб развертывания, чтобы получить список обновлений, которые можно развернуть на устройствах в качестве содержимого в развертывании.

Ниже приведен пример запроса всех обновлений Windows 10 компонентов, развертываемых службой развертывания.

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

[Развертывание](/graph/api/resources/windowsupdates-deployment) определяет содержимое для развертывания, способ и время развертывания содержимого и целевых устройств. При создании развертывания аудитория развертывания автоматически создается как связь.

Ниже приведен пример создания развертывания обновления компонентов с необязательными параметрами, настроенными [расписанием развертывания](windowsupdates-schedule-deployment.md) и [правилами мониторинга](windowsupdates-manage-monitoring-rules.md). [Меры безопасности](windowsupdates-manage-safeguards.md) применяются по умолчанию. Целевые устройства будут указаны на следующем шаге.

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
        "safeguard": null,
        "userExperience": null
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

После того как всем устройствам, назначенным аудитории развертывания, было изначально предложено обновление, возможно, не все устройства начали или завершили обновление из-за таких факторов, как подключение устройств. Пока развертывание все еще существует, клиентский компонент Центра обновления Windows продолжать предлагать обновление назначенным устройствам при каждом повторном подключении.

