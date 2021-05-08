---
title: тип ресурса cloudPcOnPremisesConnectionHealthCheck
description: Результат проверки состояния локального подключения облачного КОМПЬЮТЕРА.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: adc215b32635476320913b2d14aac33ec6ccfc95
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241151"
---
# <a name="cloudpconpremisesconnectionhealthcheck-resource-type"></a>тип ресурса cloudPcOnPremisesConnectionHealthCheck

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Результат проверки состояния локального подключения облачного КОМПЬЮТЕРА.

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[RunHealthChecks cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-runhealthcheck.md)|Нет|Запустите проверки состояния [здоровья cloudPcOnPremisesConnection.](../resources/cloudpconpremisesconnection.md)|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Имя отображения этого элемента проверки состояния.|
|status|[cloudPcOnPremisesConnectionStatus](../resources/cloudpconpremisesconnection.md#cloudpconpremisesconnectionstatus-values)|Состояние элемента проверки состояния. Возможные значения: `pending`, `running`, `passed`, `failed`, `unknownFutureValue`. Только для чтения.|
|startDateTime|DateTimeOffset|Время начала элемента проверки состояния. Только для чтения.|
|endDateTime|DateTimeOffset|Конечное время проверки состояния элемента. Только для чтения.|
|errorType|[cloudPcOnPremisesConnectionHealthCheckErrorType](#cloudpconpremisesconnectionhealthcheckerrortype-values)|Тип ошибки, которая произошла во время проверки состояния.|
|recommendedAction|Строка|Рекомендуемое действие для устранения соответствующей ошибки.|
|additionalDetails|Строка|Дополнительные сведения о проверке состояния здоровья или рекомендуемом действии.|

### <a name="cloudpconpremisesconnectionhealthcheckerrortype-values"></a>значения cloudPcOnPremisesConnectionHealthCheckErrorType

|Member|Описание|
|:---|:---|
|dnsCheckFqdnNotFound|Проверка DNS не удалась, так как полностью квалифицированное доменное имя не было найдено. Повторно введите полное доменное имя.|
|dnsCheckUnknownError|Проверка DNS не удалось из-за неизвестной ошибки. Обратитесь в службу поддержки клиентов.|
|adJoinCheckFqdnNotFound|Проверка активного присоединиться к домену не удалась, так как полностью квалифицированное доменное имя не было найдено. Повторно введите полное доменное имя.|
|adJoinCheckIncorrectCredentials|Проверка активного входа в домен не удалось, так как учетные данные домена некорректны. Пожалуйста, обнови имя пользователя и пароль.|
|adJoinCheckOrganizationalUnitNotFound|Проверка активного присоединяться к домену не удалась, так как указанное организационное подразделение не было найдено. Повторно введите подразделение организации.|
|adJoinCheckOrganizationalUnitIncorrectFormat|Проверка активного присоединяться к домену не удалось beccause формат указанного организационного подразделения является неправильным. Пример формата: "OU=OU1,OU=OU2,OU=OU3,DC=DC1".|
|adJoinCheckAccessDenied|Проверка присоединений к активному домену не удалась, так как доступ отказано, когда пользователи, не администраторы которых были делегированы, пытаются присоединиться к объектам компьютера к контроллеру домена. Назначьте клиенту правильное разрешение присоединиться к объекту компьютера в домене. Необходимые разрешения: создание объектов компьютера, удаление объектов компьютера.|
|adJoinCheckUnknownError|Проверка активного присоединяться к домену не удалось из-за неизвестной ошибки. Обратитесь в службу поддержки клиентов.|
|endpointConnectivityCheckUrlNotWhitelisted|Проверка подключения конечной точки не удалась, так как URL-адреса не находятся в списке допуска в параметрах сетевого брандмауэра. Добавьте URL-адреса в список допуска для параметров сетевого брандмауэра. Сведения [об URL-адресе см.](/azure/virtual-desktop/safe-url-list) в обязательном списке URL-адресов.|
|endpointConnectivityCheckUnknownError|Проверка подключения конечной точки не удалось из-за неизвестной ошибки. Обратитесь в службу поддержки клиентов.|
|aadConnectivityCheckUnknownError|Проверка Azure Active Directory подключения не удалось из-за неизвестной ошибки. Обратитесь в службу поддержки клиентов.|
|resourceAvailabilityCheckNoSubnetIP|Проверка доступности ресурсов не удалась из-за того, что в подсети не было доступных IP-адресов. Пожалуйста, освободите некоторые или измените другую подсеть и повторно.|
|resourceAvailabilityCheckSubscriptionDisabled|Проверка доступности ресурсов не удалось из-за отключенной подписки Azure. Пожалуйста, повторно ввяйте подписку.|
|resourceAvailabilityCheckUnknownError|Проверка доступности ресурсов не удалось из-за неизвестной ошибки. Обратитесь в службу поддержки клиентов.|
|permissionCheckNoSubscriptionReaderRole|Cloud PC службы не имеет разрешений на чтение в указанной подписке Azure. Обратитесь к владельцу подписки, чтобы добавить назначение ролей читателя в подписке Azure для Cloud PC службы.|
|permissionCheckNoResourceGroupOwnerRole|Cloud PC не имеет разрешений владельца в указанной группе ресурсов. Обратитесь к владельцу подписки, чтобы добавить назначение роли владельца в группе ресурсов для Cloud PC службы.|
|permissionCheckNoVNetContributorRole|Cloud PC службы не имеет разрешений на сетевой вкладчик в указанной виртуальной сети. Обратитесь к владельцу подписки, чтобы добавить назначение роли вкладчика сети для Cloud PC службы. |
|permissionCheckUnknownError|Проверка разрешений не удалась из-за неизвестной ошибки. Обратитесь в службу поддержки клиентов.|
|internalServerUnknownError|Проверка состояния не удалось из-за неизвестной ошибки внутреннего сервера. Обратитесь в службу поддержки клиентов.|

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
