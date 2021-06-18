---
title: тип ресурса cloudPcOnPremisesConnectionHealthCheck
description: Результат проверки состояния локального подключения облачного КОМПЬЮТЕРА.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 0323ee64056df1019cc2a8f6e2bd004ffec223b7
ms.sourcegitcommit: 2d0daa446c7b37ced1d214e0c6e18e2b8243bb09
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2021
ms.locfileid: "53010202"
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
|displayName|String|Имя отображения этого элемента проверки состояния.|
|status|[cloudPcOnPremisesConnectionStatus](../resources/cloudpconpremisesconnection.md#cloudpconpremisesconnectionstatus-values)|Состояние элемента проверки состояния. Возможные значения: `pending`, `running`, `passed`, `failed`, `unknownFutureValue`. Только для чтения.|
|startDateTime|DateTimeOffset|Время начала элемента проверки состояния. Только для чтения.|
|endDateTime|DateTimeOffset|Конечное время проверки состояния элемента. Только для чтения.|
|errorType|[cloudPcOnPremisesConnectionHealthCheckErrorType](#cloudpconpremisesconnectionhealthcheckerrortype-values)|Тип ошибки, которая произошла во время проверки состояния.|
|recommendedAction|String|Рекомендуемое действие для устранения соответствующей ошибки.|
|additionalDetails|String|Дополнительные сведения о проверке состояния здоровья или рекомендуемом действии.|

### <a name="cloudpconpremisesconnectionhealthcheckerrortype-values"></a>значения cloudPcOnPremisesConnectionHealthCheckErrorType

|Member|Описание|
|:---|:---|
|dnsCheckFqdnNotFound|Проверка DNS не удалась, так как полностью квалифицированное доменное имя не было найдено. Повторно введите полное доменное имя.|
|dnsCheckUnknownError|Проверка DNS не удалось из-за неизвестной ошибки. Обратитесь в службу поддержки клиентов.|
|adJoinCheckFqdnNotFound|Проверка активного присоединиться к домену не удалась, так как полностью квалифицированное доменное имя не было найдено. Повторно введите полное доменное имя.|
|adJoinCheckIncorrectCredentials|Проверка активного входа в домен не удалось, так как учетные данные домена некорректны. Пожалуйста, обнови имя пользователя и пароль.|
|adJoinCheckOrganizationalUnitNotFound|Проверка активного присоединяться к домену не удалась, так как указанное организационное подразделение не было найдено. Повторно введите подразделение организации.|
|adJoinCheckOrganizationalUnitIncorrectFormat|Проверка активного присоединяемого домена не удалась, так как формат указанного организационного подразделения является неправильным. Пример формата: "OU=OU1,OU=OU2,OU=OU3,DC=DC1".|
|adJoinCheckAccessDenied|Проверка присоединений к активному домену не удалась, так как доступ отказано, когда пользователи, не администраторы которых были делегированы, пытаются присоединиться к объектам компьютера к контроллеру домена. Назначьте клиенту правильное разрешение присоединиться к объекту компьютера в домене. Необходимые разрешения: создание объектов компьютера, удаление объектов компьютера.|
|adJoinCheckUnknownError|Проверка активного присоединяться к домену не удалось из-за неизвестной ошибки. Обратитесь в службу поддержки клиентов.|
|endpointConnectivityCheckCloudPcUrlNotAllowListed|Проверка подключения конечной точки не удалась из-за того, что URL-адрес хранилища сценариев обеспечения КПК не указан в списке допустимого подключения в параметрах сетевого брандмауэра. Добавьте URL-адреса в список разрешенных параметров сетевого брандмауэра. URL-адреса можно найти в дополнительных сведениях.|
|endpointConnectivityCheckWVDUrlNotAllowListed|Проверка подключения конечной точки не удалась, так как URL-адрес WVD не указан в списке допустимого доступа в параметрах сетевого брандмауэра. Добавьте URL-адреса в список разрешенных параметров сетевого брандмауэра.|
|endpointConnectivityCheckIntuneUrlNotAllowListed|Проверка подключения конечной точки не удалась, так как URL-адрес Intune не указан в списке допуска в параметрах сетевого брандмауэра. Добавьте URL-адреса в список разрешенных параметров сетевого брандмауэра.|
|endpointConnectivityCheckUnknownError|Проверка подключения конечной точки не удалось из-за неизвестной ошибки. Обратитесь в службу поддержки клиентов.|
|aadConnectivityCheckUnknownError|Проверка Azure Active Directory подключения не удалось из-за неизвестной ошибки. Обратитесь в службу поддержки клиентов.|
|resourceAvailabilityCheckNoSubnetIP|Проверка доступности ресурсов не удалась из-за того, что в подсети не было доступных IP-адресов. Пожалуйста, освободите некоторые или измените другую подсеть и повторно.|
|resourceAvailabilityCheckSubscriptionDisabled|Проверка доступности ресурсов не удалось из-за отключенной подписки Azure. Пожалуйста, повторно ввяйте подписку.|
|resourceAvailabilityCheckAzurePolicyViolation|Создание требуемого ресурса Azure не удалось, так как политика Azure организаций заблокировала действие. Обновите политику Azure, чтобы разрешить создание этого ресурса.|
|resourceAvailabilityCheckUnsupportedVNetRegion|Выбранный vNet не находится в поддерживаемом регионе Azure.|
|resourceAvailabilityCheckUnknownError|Проверка доступности ресурсов не удалось из-за неизвестной ошибки. Обратитесь в службу поддержки клиентов.|
|permissionCheckNoSubscriptionReaderRole|Руководитель службы облачных ПК не имеет разрешений на чтение в указанной подписке Azure. Обратитесь к владельцу подписки, чтобы добавить назначение ролей читателя в подписке Azure для директора службы облачных ПК.|
|permissionCheckNoResourceGroupOwnerRole|У директора службы облачных ПК нет разрешений владельцев указанной группы ресурсов. Обратитесь к владельцу подписки, чтобы добавить назначение роли владельца в группе ресурсов для директора службы облачных ПК.|
|permissionCheckNoVNetContributorRole|В указанной виртуальной сети у директора службы облачных ПК нет разрешений на сетевой вкладчик. Обратитесь к владельцу подписки, чтобы добавить назначение роли вкладчика сети для директора службы облачных ПК. |
|permissionCheckUnknownError|Проверка разрешений не удалась из-за неизвестной ошибки. Обратитесь в службу поддержки клиентов.|
|internalServerErrorDeploymentCanceled|Развертывание было отменено. Повторите попытку позже. Если проблема сохраняется, обратитесь в службу поддержки.|
|internalServerErrorAllocateResourceFailed|Выделение ресурсов не удалось. Попробуйте еще раз или обратитесь в службу поддержки для получения дополнительных сведений.|
|internalServerErrorVMDeploymentTimeout|Развертывание виртуальной машины ото времени. Повторить. Если проблема сохраняется, обратитесь в службу поддержки.|
|internalServerErrorUnableToRunDscScript|Невозможно запустить сценарий DSC во время проверки состояния здоровья. Для успешного обеспечения облачного КОМПЬЮТЕРА службе необходим доступ к WinRM. Убедитесь, что ни одна групповая политика или связанная конфигурация не блокируют использование PowerShell/DSC.|
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
