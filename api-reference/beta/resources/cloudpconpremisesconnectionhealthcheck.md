---
title: Тип ресурса cloudPcOnPremisesConnectionHealthCheck
description: Результат проверки состояния локального подключения на облачном компьютере.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 32b57750400e1fb71dc8cc173b364fba76cd36ec
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2021
ms.locfileid: "50033983"
---
# <a name="cloudpconpremisesconnectionhealthcheck-resource-type"></a>Тип ресурса cloudPcOnPremisesConnectionHealthCheck

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Результат проверки состояния локального подключения на облачном компьютере.

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[RunHealthChecks cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-runhealthcheck.md)|Нет|Запустите проверки состояния [cloudPcOnPremisesConnection.](../resources/cloudpconpremisesconnection.md)|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Отображаемая фамилия для этого элемента проверки состояния.|
|status|[cloudPcOnPremisesConnectionStatus](../resources/cloudpconpremisesconnection.md#cloudpconpremisesconnectionstatus-values)|Состояние элемента проверки состояния. Возможные значения: `pending`, `running`, `passed`, `failed`, `unknownFutureValue`. Только для чтения.|
|startDateTime|DateTimeOffset|Время начала проверки состояния. Только для чтения.|
|endDateTime|DateTimeOffset|Время окончания элемента проверки состояния. Только для чтения.|
|errorType|[cloudPcOnPremisesConnectionHealthCheckErrorType](#cloudpconpremisesconnectionhealthcheckerrortype-values)|Тип ошибки, которая произошла во время этой проверки.|
|recommendedAction|String|Рекомендуемое действие для устранения соответствующей ошибки.|
|additionalDetails|String|Дополнительные сведения о проверке состояния или рекомендуемом действии.|

### <a name="cloudpconpremisesconnectionhealthcheckerrortype-values"></a>значения cloudPcOnPremisesConnectionHealthCheckErrorType

|Member|Описание|
|:---|:---|
|dnsCheckFqdnNotFound|Сбой проверки DNS, так как полное доменное имя не найдено. Повторно введите полное доменное имя.|
|dnsCheckUnknownError|Не удалось проверить DNS из-за неизвестной ошибки. Обратитесь в службу поддержки клиентов.|
|adJoinCheckFqdnNotFound|Сбой проверки пользования активным доменом из-за того, что не найдено полное доменное имя. Повторно введите полное доменное имя.|
|adJoinCheckIncorrectCredentials|Сбой проверки пользования активным доменом из-за неправильных учетных данных домена. Обновите имя пользователя и пароль.|
|adJoinCheckOrganizationalUnitNotFound|Сбой проверки присоединить активный домен из-за того, что указанное подразделение не найдено. Повторно введите подразделение.|
|adJoinCheckOrganizationalUnitIncorrectFormat|При проверке пользования активным доменом не удалось использовать неправильный формат указанного подразделения. Пример формата: "OU=OU1,OU=OU2,OU=OU3,DC=DC1".|
|adJoinCheckUnknownError|Сбой проверки присоединить активный домен из-за неизвестной ошибки. Обратитесь в службу поддержки клиентов.|
|endpointConnectivityCheckUrlNotWhitelisted|Не удалось проверить возможность подключения к конечной точке, так как URL-адреса не находятся в списке адресов в параметрах сетевого брандмауэра. Добавьте URL-адреса в список разрешаний для параметров сетевого брандмауэра. Сведения [об URL-адресах см.](/azure/virtual-desktop/safe-url-list) в обязательном списке URL-адресов.|
|endpointConnectivityCheckUnknownError|Не удалось проверить возможность подключения к конечной точке из-за неизвестной ошибки. Обратитесь в службу поддержки клиентов.|
|aadConnectivityCheckUnknownError|Не удалось проверить подключение Azure Active Directory из-за неизвестной ошибки. Обратитесь в службу поддержки клиентов.|
|resourceAvailabilityCheckNoSubnetIP|Не удалось проверить доступность ресурсов, так как в подсети нет доступных IP-адресов. Освободите некоторые из них или измените их на другую подсеть и повторить попытку.|
|resourceAvailabilityCheckSubscriptionDisabled|Не удалось проверить доступность ресурсов из-за отключенной подписки Azure. Please re-enable the subscription.|
|resourceAvailabilityCheckUnknownError|Не удалось проверить доступность ресурсов из-за неизвестной ошибки. Обратитесь в службу поддержки клиентов.|
|permissionCheckNoSubscriptionReaderRole|У директора-службы облачного ПК нет разрешений на чтение для указанной подписки Azure. Обратитесь к владельцу подписки, чтобы добавить назначение роли читателя в подписке Azure для основного компьютера-службы Cloud PC.|
|permissionCheckNoResourceGroupOwnerRole|У директора-службы облачного ПК нет разрешений владельца для указанной группы ресурсов. Обратитесь к владельцу подписки, чтобы добавить назначение роли владельца в группу ресурсов для основного службы Cloud PC.|
|permissionCheckNoVNetContributorRole|У участника-службы облачного ПК нет разрешений на сетевой участник в указанной виртуальной сети. Обратитесь к владельцу подписки, чтобы добавить назначение роли сетевого участника для участника-службы Cloud PC. |
|permissionCheckUnknownError|Не удалось проверить разрешения из-за неизвестной ошибки. Обратитесь в службу поддержки клиентов.|
|internalServerUnknownError|Не удалось проверить состояние системы из-за неизвестной внутренней ошибки сервера. Обратитесь в службу поддержки клиентов.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcOnPremisesConnectionHealthCheck"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcOnPremisesConnectionHealthCheck",
  "displayName": "String",
  "status": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "errorType": "String",
  "recommendedAction": "String",
  "additionalDetails": "String"
}
```
