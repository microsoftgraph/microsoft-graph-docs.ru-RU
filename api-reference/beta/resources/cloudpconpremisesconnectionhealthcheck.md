---
title: тип ресурса cloudPcOnPremisesConnectionHealthCheck
description: Результат проверки состояния локального подключения облачного КОМПЬЮТЕРА.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: b1b1010c22bed8de73b5d3fa2caf680f26091d00
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2021
ms.locfileid: "53351092"
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
|dnsCheckFqdnNotFound|Решение DNS не удалось для доменного имени. Возможные причины ошибки: 1. Указанный DNS-сервер Azure vNet не может разрешить доменное имя. Обновление vNet с помощью соответствующего DNS-сервера; 2. Предоставленное доменное имя не существует или не является правильным. Пожалуйста, обнови локальное сетевое подключение правильным доменным именем. Убедитесь, что vNet, определенный в локальном сетевом соединении, может разрешить доменное имя.|
|dnsCheckUnknownError|Решение DNS не удалось для доменного имени. Возможные причины ошибки: 1. Указанный DNS-сервер Azure vNet не может разрешить доменное имя. Обновление vNet с помощью соответствующего DNS-сервера; 2. Предоставленное доменное имя не существует или не является правильным. Пожалуйста, обнови локальное сетевое подключение правильным доменным именем. Убедитесь, что vNet, определенный в локальном сетевом соединении, может разрешить доменное имя.|
|adJoinCheckFqdnNotFound|Проверка присоединиться к домену не удалась, так как имя домена не удалось найти. Убедитесь, что к контроллеру домена для доменного имени можно связаться с помощью vNet, определенного в локальном сетевом соединении.|
|adJoinCheckIncorrectCredentials|Проверка присоединиться к домену не удалась, так как учетные данные, предоставленные для домена, не являются правильными. Пожалуйста, обнови локальное сетевое подключение с помощью правильных учетных данных.|
|adJoinCheckOrganizationalUnitNotFound|Проверка пользования доменом не удалась, так как не удается найти организационное подразделение (OU). Пожалуйста, укайте OU в домене. OU должен быть в формате различимого имени. Пример формата: "OU=OU1,OU=OU2,OU=OU3,DC=DC1".|
|adJoinCheckOrganizationalUnitIncorrectFormat|Проверка пользования доменом не удалась, так как не удается найти организационное подразделение (OU). Пожалуйста, укайте OU в домене. OU должен быть в формате различимого имени. Пример формата: "OU=OU1,OU=OU2,OU=OU3,DC=DC1".|
|adJoinCheckComputerObjectAlreadyExists|Учетная запись компьютера не может быть найдена в организационном подразделении (OU), предоставляемом в локальном сетевом соединении, но имя компьютера уже существует в домене. Это часто происходит после того, как объект компьютера был перемещен из OU, настроенного в локальном сетевом подключении. Переместите объект компьютера обратно в целевой OU.|
|adJoinCheckAccessDenied|Проверка присоединиться к домену не удалась, так как предоставленная учетная запись пользователя не имеет достаточных разрешений для пользования доменом. Убедитесь, что предоставленная учетная запись имеет достаточное количество разрешений или измените учетную запись пользователя, определяемую в свойствах локального сетевого подключения. Необходимые разрешения: *создание компьютерных объектов и* удаление объектов *компьютера.*|
|adJoinCheckUnknownError|Проверка пользования доменом не удалось из-за неизвестной ошибки. Убедитесь, что локальное сетевое подключение может успешно присоединиться к домену с помощью предоставленных сведений.|
|endpointConnectivityCheckCloudPcUrlNotAllowListed|Во время подготовка не удалось связаться с одним или более требуемой URL-адресами. Убедитесь, что все необходимые URL-адреса разрешены через брандмауэры и прокси.|
|endpointConnectivityCheckWVDUrlNotAllowListed|Во время подготовка не удалось связаться с одним или более требуемой URL-адресами WVD. Убедитесь, что все необходимые URL-адреса разрешены через брандмауэры и прокси.|
|endpointConnectivityCheckIntuneUrlNotAllowListed|Во время подготовка не удалось связаться с одним или более требуемой URL-адресами Intune. Убедитесь, что все необходимые URL-адреса разрешены через брандмауэры и прокси.|
|endpointConnectivityCheckUnknownError|Во время подготовка не удалось связаться с одним или более требуемой URL-адресами. Убедитесь, что все необходимые URL-адреса разрешены через брандмауэры и прокси.|
|azureAdDeviceSyncCheckDeviceNotFound|Объект облачного компьютера компьютера не может быть найден в Azure Active Directory (Azure AD). Убедитесь, что Azure AD часто работает и синхронизируется, чтобы объекты облачного компьютера синхронизировались с Azure AD. Синхронизация устройств Azure AD должна быть включена и синхронизирована в течение последних 60 минут.|
|azureAdDeviceSyncCheckLongSyncCircle|Проверка синхронизации объекта облачного компьютера с Azure Active Directory (Azure AD). Убедитесь, что Azure AD часто работает и синхронизируется, чтобы объекты облачного компьютера синхронизировались с Azure AD. Синхронизация устройств Azure AD должна быть включена и синхронизирована в течение последних 60 минут.|
|azureAdDeviceSyncCheckUnknownError|Проверка подключения Azure Active Directory (Azure AD) не удалось. Убедитесь, что Azure AD часто работает и синхронизируется, чтобы объекты облачного компьютера синхронизировались с Azure AD. Синхронизация устройств Azure AD должна быть включена и синхронизирована в течение последних 60 минут.|
|resourceAvailabilityCheckNoSubnetIP|Предоставленная подсеть не имеет IP-адресов. Убедитесь, что подсети, предоставляемые в локальном сетевом соединении, имеют достаточные IP-адреса. Пожалуйста, расширйте текущую выбранную подсеть или выберите другую подсеть, которая будет использоваться для предварительного обеспечения.|
|resourceAvailabilityCheckSubscriptionDisabled|Предоставленная подписка Azure отключена. Убедитесь, что подписка Azure включена и доступна для предварительной провизии.|
|resourceAvailabilityCheckAzurePolicyViolation|Предоставленная подписка Azure не может быть найдена. Убедитесь, что подписка Azure доступна для предварительного обеспечения.|
|resourceAvailabilityCheckUnsupportedVNetRegion|Выбранный vNet расположен в неподтверченном регионе. Убедитесь, что выбранный vNet расположен в поддерживаемом регионе.|
|resourceAvailabilityCheckUnknownError|Проверка доступности ресурсов для ресурсов Azure не удалось из-за неизвестной ошибки. Убедитесь, что все ресурсы Azure соответствуют необходимым требованиям.|
|permissionCheckNoSubscriptionReaderRole|У директора службы облачных ПК нет достаточных разрешений на подписку Azure. Убедитесь, что у директора облачной службы ПК есть разрешения *reader* в подписке.|
|permissionCheckNoResourceGroupOwnerRole|Руководитель службы облачных ПК не имеет достаточных разрешений в группе ресурсов Azure. Убедитесь, что у директора службы облачных ПК *есть* разрешения владельца в группе ресурсов. |
|permissionCheckNoVNetContributorRole|У директора службы облачных ПК нет достаточных разрешений в Azure vNet. Убедитесь, что в службе облачных ПК *есть* разрешения на вкладчик Сети в vNet.|
|permissionCheckUnknownError|У директора службы облачных ПК нет достаточных разрешений. Убедитесь, что директору облачной службы ПК предоставлено достаточное количество разрешений Azure.|
|internalServerErrorDeploymentCanceled|Развертывание было отменено. Повторите попытку позже. Если проблема сохраняется, обратитесь в службу поддержки.|
|internalServerErrorAllocateResourceFailed|Выделение ресурсов не удалось. Повторите попытку позже. Если проблема сохраняется, обратитесь в службу поддержки.|
|internalServerErrorVMDeploymentTimeout|Развертывание виртуальной машины ото времени. Попробуйте еще раз. Если проблема сохраняется, обратитесь в службу поддержки.|
|internalServerErrorUnableToRunDscScript|Во время подготовка на облачном компьютере выполняются некоторые скрипты DSC PowerShell. Невозможно скачать эти скрипты DSC или выполнить их во время проверки состояния здоровья. Убедитесь, что vNet имеет неограниченный доступ к требуемой конечной точке, а PowerShell не блокируется в среде или групповой политике.|
|internalServerUnknownError|Подготовка не удалась из-за внутренней ошибки. Обратитесь в службу поддержки клиентов.|

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
