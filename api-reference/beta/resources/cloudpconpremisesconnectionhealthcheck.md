---
title: тип ресурса cloudPcOnPremisesConnectionHealthCheck
description: Результат проверки состояния сетевого подключения к облачной сети PC Azure.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: fc8ee01576e6381c54455d765a007e89b8f9c0d7
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589270"
---
# <a name="cloudpconpremisesconnectionhealthcheck-resource-type"></a>тип ресурса cloudPcOnPremisesConnectionHealthCheck

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Результат проверки состояния сетевого подключения к облачной сети PC Azure.

[!INCLUDE [on-premise-rename-note](../../includes/on-premise-rename-note.md)]

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[RunHealthChecks cloudPcOnPremisesConnection](../api/cloudpconpremisesconnection-runhealthcheck.md)|Нет|Запустите проверки состояния [здоровья cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Имя отображения этого элемента проверки состояния.|
|status|[cloudPcOnPremisesConnectionStatus](../resources/cloudpconpremisesconnection.md#cloudpconpremisesconnectionstatus-values)|Состояние элемента проверки состояния. Возможные значения: `pending`, `running`, `passed`, `failed`, `unknownFutureValue`. Только для чтения.|
|startDateTime|DateTimeOffset|Время начала элемента проверки состояния. Только для чтения.|
|endDateTime|DateTimeOffset|Конечное время проверки состояния элемента. Только для чтения.|
|errorType|[cloudPcOnPremisesConnectionHealthCheckErrorType](#cloudpconpremisesconnectionhealthcheckerrortype-values)|Тип ошибки, которая произошла во время проверки состояния.|
|recommendedAction|String|Рекомендуемое действие для устранения соответствующей ошибки.|
|additionalDetails|Строка|Дополнительные сведения о проверке состояния здоровья или рекомендуемом действии.|

### <a name="cloudpconpremisesconnectionhealthcheckerrortype-values"></a>значения cloudPcOnPremisesConnectionHealthCheckErrorType

|Member|Описание|
|:---|:---|
|dnsCheckFqdnNotFound|Решение DNS не удалось для доменного имени. Возможные причины ошибки: 1. Указанный DNS-сервер Azure vNet не может разрешить доменное имя. Обновление vNet с помощью соответствующего DNS-сервера; 2. Предоставленное доменное имя не существует или не является правильным. Пожалуйста, обновим сетевое подключение Azure правильным доменным именем. Убедитесь, что vNet, определенный в сетевом соединении Azure, может разрешить доменное имя.|
|dnsCheckNameWithInvalidCharacter|Проверка DNS не удалась, так как введенное доменное имя содержит неподтверченный символ. Убедитесь, что имя домена содержит только поддерживаемые символы.|
|dnsCheckUnknownError|Решение DNS не удалось для доменного имени. Возможные причины ошибки: 1. Указанный DNS-сервер Azure vNet не может разрешить доменное имя. Обновление vNet с помощью соответствующего DNS-сервера; 2. Предоставленное доменное имя не существует или не является правильным. Пожалуйста, обновим сетевое подключение Azure правильным доменным именем. Убедитесь, что vNet, определенный в сетевом соединении Azure, может разрешить доменное имя.|
|adJoinCheckFqdnNotFound|Проверка присоединиться к домену не удалась, так как имя домена не удалось найти. Убедитесь, что к контроллеру домена для доменного имени можно связаться с помощью vNet, определенного в сетевом соединении Azure.|
|adJoinCheckIncorrectCredentials|Проверка присоединиться к домену не удалась, так как учетные данные, предоставленные для домена, не являются правильными. Пожалуйста, обновим сетевое подключение Azure правильными учетными данными.|
|adJoinCheckOrganizationalUnitNotFound|Проверка пользования доменом не удалась, так как не удается найти организационное подразделение (OU). Пожалуйста, укайте OU в домене. OU должен быть в формате различимого имени. Пример формата: "OU=OU1,OU=OU2,OU=OU3,DC=DC1".|
|adJoinCheckOrganizationalUnitIncorrectFormat|Проверка пользования доменом не удалась, так как не удается найти организационное подразделение (OU). Пожалуйста, укайте OU в домене. OU должен быть в формате различимого имени. Пример формата: "OU=OU1,OU=OU2,OU=OU3,DC=DC1".|
|adJoinCheckComputerObjectAlreadyExists|Учетная запись компьютера не может быть найдена в организационном подразделении (OU), предоставляемом в сетевом соединении Azure, но имя компьютера уже существует в домене. Это часто происходит после того, как объект компьютера был перемещен из OU, настроенного в сетевом соединении Azure. Переместите объект компьютера обратно в целевой OU.|
|adJoinCheckAccessDenied|Проверка присоединиться к домену не удалась, так как предоставленная учетная запись пользователя не имеет достаточных разрешений для пользования доменом. Убедитесь, что предоставленная учетная запись имеет достаточное количество разрешений или измените учетную запись пользователя, задатую в свойствах сетевого подключения Azure. Необходимые разрешения: *создание объектов компьютера и* *удаление объектов компьютера*.|
|adJoinCheckCredentialsExpired|Проверка доступа к домену не удалась из-за истечения срока действия пароля пользователя, вступаемого в домен. Сначала обнови пароль, а затем обновив сетевое подключение Azure новыми учетными данными.|
|adJoinCheckAccountLockedOrDisabled|Проверка присоединиться к домену не удалась, так как учетная запись пользователя в настоящее время заблокирована или отключена. Убедитесь, что учетная запись пользователя присоединяться к домену разблокирована, активна и может проверить подлинность домена.|
|adJoinCheckAccountQuotaExceeded|Проверка присоединиться к домену не удалась, так как число пользователей, присоединив к домену, превысило максимальное количество присоединяется к домену. Убедитесь, что регистрация домена разрешена, а свойство **ms-DS-MachineAccountQuota Active Directory** позволяет достаточно присоединяться к домену.|
|adJoinCheckUnknownError|Проверка пользования доменом не удалось из-за неизвестной ошибки. Убедитесь, что сетевое подключение Azure может успешно присоединиться к домену с помощью предоставленных сведений.|
|endpointConnectivityCheckCloudPcUrlNotAllowListed|Во время подготовка не удалось связаться с одним или более требуемой URL-адресами. Убедитесь, что все необходимые URL-адреса разрешены через брандмауэры и прокси.|
|endpointConnectivityCheckWVDUrlNotAllowListed|Во время подготовка не удалось связаться с одним или более требуемой URL-адресами WVD. Убедитесь, что все необходимые URL-адреса разрешены через брандмауэры и прокси.|
|endpointConnectivityCheckIntuneUrlNotAllowListed|Во время предварительной Intune не удалось связаться с одним или более URL-адресами. Убедитесь, что все необходимые URL-адреса разрешены через брандмауэры и прокси.|
|endpointConnectivityCheckUnknownError|Во время подготовка не удалось связаться с одним или более требуемой URL-адресами. Убедитесь, что все необходимые URL-адреса разрешены через брандмауэры и прокси.|
|azureAdDeviceSyncCheckDeviceNotFound|Объект облачного компьютера компьютера не может быть найден в Azure Active Directory (Azure AD). Убедитесь, что Azure AD часто работает и синхронизируется, чтобы объекты облачного компьютера синхронизировались с Azure AD. Синхронизация устройств Azure AD должна быть включена и синхронизирована в течение последних 60 минут.|
|azureAdDeviceSyncCheckLongSyncCircle|Проверка синхронизации объекта облачного компьютера с Azure Active Directory (Azure AD). Убедитесь, что Azure AD часто работает и синхронизируется, чтобы объекты облачного компьютера синхронизировались с Azure AD. Синхронизация устройств Azure AD должна быть включена и синхронизирована в течение последних 60 минут.|
|azureAdDeviceSyncCheckConnectDisabled|Проверка синхронизации Azure Active Directory (Azure AD) не удалось из-за отключения Подключение Azure AD. Убедитесь, что Подключение Azure AD включен и часто синхронизируется. Если служба Azure AD Подключение не синхронизирует компьютер в течение 60 минут, проверка будет неудалась.|
|azureAdDeviceSyncCheckDurationExceeded|Проверка синхронизации Azure Active Directory устройства Azure AD не удалось, так как синхронизация Подключение Azure AD не была синхронизирована в течение 60 минут. Убедитесь, что Подключение Azure AD включен и часто синхронизируется. Если служба Azure AD Подключение не синхронизирует компьютер в течение 60 минут, проверка будет неудалась.|
|azureAdDeviceSyncCheckScpNotConfigured|В гибридной Azure Active Directory (Azure AD) не удалось из-за неправильной конфигурации точки конфигурации службы (SCP). Убедитесь, что конфигурация SCP является допустимой и доступной для выполнения гибридного aD Azure. SCP можно создать и настроить в мастере Azure AD Подключение.|
|azureAdDeviceSyncCheckTransientServiceError|Проверка синхронизации Azure Active Directory устройства Azure AD не удалось из-за преходящей ошибки. Попробуйте еще раз. Если проблема сохраняется, обратитесь в службу поддержки клиентов.|
|azureAdDeviceSyncCheckUnknownError|Проверка подключения Azure Active Directory (Azure AD) не удалось. Убедитесь, что Azure AD часто работает и синхронизируется, чтобы объекты облачного компьютера синхронизировались с Azure AD. Синхронизация устройств Azure AD должна быть включена и синхронизирована в течение последних 60 минут.|
|resourceAvailabilityCheckNoSubnetIP|Предоставленная подсеть не имеет IP-адресов. Убедитесь, что подсети, предоставляемые в сетевом соединении Azure, имеют достаточные IP-адреса. Пожалуйста, расширйте текущую выбранную подсеть или выберите другую подсеть, которая будет использоваться для предварительного обеспечения.|
|resourceAvailabilityCheckSubscriptionDisabled|Предоставленная подписка Azure отключена. Убедитесь, что подписка Azure включена и доступна для предварительной провизии.|
|resourceAvailabilityCheckAzurePolicyViolation|Предоставленная подписка Azure не может быть найдена. Убедитесь, что подписка Azure доступна для предварительного обеспечения.|
|resourceAvailabilityCheckSubscriptionNotFound|Доступ к предоставленной подписке Azure не предоставляется. Убедитесь, что подписка Azure доступна для предварительного обеспечения.|
|resourceAvailabilityCheckSubscriptionTransferred|Доступ к предоставленной подписке Azure не предоставляется. Убедитесь, что подписка Azure доступна для предварительного обеспечения.|
|resourceAvailabilityCheckGeneralSubscriptionError|Политика Azure ограничивает создание ресурсов. Убедитесь, что политика Azure не ограничивает создание ресурсов в группе подписки и/или ресурсов.|
|resourceAvailabilityCheckUnsupportedVNetRegion|Выбранный vNet расположен в неподтверченном регионе. Убедитесь, что выбранный vNet расположен в поддерживаемом регионе.|
|resourceAvailabilityCheckResourceGroupInvalid|Выбранная группа ресурсов Azure недействительна или не найдена. Убедитесь, что выбранная группа ресурсов Azure доступна для предоставления ресурсов. Кроме того, обнови это сетевое подключение Azure с другой группой ресурсов.|
|resourceAvailabilityCheckVNetInvalid|Выбранная виртуальная сеть Azure недействительна. Убедитесь, что выбранная виртуальная сеть доступна и здорова. Кроме того, обновим это сетевое подключение Azure с другой виртуальной сетью.|
|resourceAvailabilityCheckSubnetInvalid|Выбранная подсеть Azure недействительна. Убедитесь, что выбранная подсеть доступна и здорова. Кроме того, обнови это сетевое подключение Azure с помощью другой подсети.|
|resourceAvailabilityCheckResourceGroupBeingDeleted|Выбранная группа ресурсов Azure удаляется. Убедитесь, что выбранная группа ресурсов Azure доступна для предоставления ресурсов. Кроме того, обнови это сетевое подключение Azure с другой группой ресурсов.|
|resourceAvailabilityCheckVNetBeingMoved|Выбранная виртуальная сеть Azure перемещается. Убедитесь, что виртуальная сеть не меняется и не перемещается, и попробуйте еще раз. Кроме того, обнови это сетевое подключение Azure с помощью другого vNet.|
|resourceAvailabilityCheckSubnetDelegationFailed|Выбранная виртуальная сеть Azure имеет делегирующую подсеть, которая блокирует создание сетевого интерфейса (Nic). Попросите владельца виртуальной сети Azure изменить политику делегирования подсетей, чтобы обеспечить успешное подготовка.|
|resourceAvailabilityCheckSubnetWithExternalResources|Выбранную подсеть нельзя использовать, так как она содержит внешние ресурсы. Удалите все ресурсы, которые могут вызвать конфликты, и попробуйте еще раз. Кроме того, обнови это сетевое подключение Azure с помощью другой подсети.|
|resourceAvailabilityCheckResourceGroupLockedForReadonly|Выбранная группа ресурсов заблокирована и не может быть изменена для обеспечения. Удалите этот блокировку, чтобы обеспечить успешное обеспечение.|
|resourceAvailabilityCheckResourceGroupLockedForDelete|Выбранная группа ресурсов или ее родительская область заблокированы для удаления действий. Это может быть из-за использования IP-адресов. Удалите блокировку и попробуйте еще раз.|
|resourceAvailabilityCheckTransientServiceError|Проверка доступности ресурсов не удалось из-за преходящей ошибки. Попробуйте еще раз. Если проблема сохраняется, обратитесь в службу поддержки клиентов.|
|resourceAvailabilityCheckUnknownError|Проверка доступности ресурсов для ресурсов Azure не удалось из-за неизвестной ошибки. Убедитесь, что все ресурсы Azure соответствуют необходимым требованиям.|
|permissionCheckNoSubscriptionReaderRole|У директора службы облачных ПК нет достаточных разрешений на подписку Azure. Убедитесь, что у директора облачной службы ПК есть разрешения *reader* в подписке.|
|permissionCheckNoResourceGroupOwnerRole|Руководитель службы облачных ПК не имеет достаточных разрешений в группе ресурсов Azure. Убедитесь, что у директора службы облачных *ПК есть разрешения* владельца в группе ресурсов. |
|permissionCheckNoVNetContributorRole|У директора службы облачных ПК нет достаточных разрешений в Azure vNet. Убедитесь, что в службе облачных *ПК есть разрешения* на вкладчик Сети в vNet.|
|permissionCheckNoResourceGroupNetworkContributorRole|Руководитель службы облачных ПК не имеет достаточных разрешений в группе ресурсов Azure. Убедитесь, что в группе ресурсов у приложения есть разрешения на авторов сети.|
|permissionCheckTransientServiceError|Проверка разрешений на первое приложение не удалось из-за преходящей ошибки. Попробуйте еще раз. Если проблема сохраняется, обратитесь в службу поддержки клиентов.|
|permissionCheckUnknownError|У директора службы облачных ПК нет достаточных разрешений. Убедитесь, что директору облачной службы ПК предоставлено достаточное количество разрешений Azure.|
|internalServerErrorDeploymentCanceled|Развертывание было отменено. Повторите попытку позже. Если проблема сохраняется, обратитесь в службу поддержки.|
|internalServerErrorAllocateResourceFailed|Выделение ресурсов не удалось. Повторите попытку позже. Если проблема сохраняется, обратитесь в службу поддержки.|
|internalServerErrorVMDeploymentTimeout|Развертывание виртуальной машины ото времени. Попробуйте еще раз. Если проблема сохраняется, обратитесь в службу поддержки.|
|internalServerErrorUnableToRunDscScript|Во время подготовка на облачном компьютере выполняются некоторые скрипты DSC PowerShell. Невозможно скачать эти скрипты DSC или выполнить их во время проверки состояния здоровья. Убедитесь, что vNet имеет неограниченный доступ к требуемой конечной точке, и PowerShell не блокируется в среде или групповая политика.|
|internalServerUnknownError|Подготовка не удалась из-за внутренней ошибки. Обратитесь в службу поддержки клиентов.|
|unknownFutureValue|Эволюционирующее значение sentinel. Не следует использовать.|

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
