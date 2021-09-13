---
title: Тип ресурса deviceAppManagement
description: Одноэлементный объект, служащий контейнером для всех функций управления приложениями на устройствах.
author: rolyon
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a021bc627833ecc0187938b18b7ac39f515c2ff6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59063673"
---
# <a name="deviceappmanagement-resource-type"></a>Тип ресурса deviceAppManagement

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Одноэлементный объект, служащий контейнером для всех функций управления приложениями на устройствах.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение объекта deviceAppManagement](../api/intune-shared-deviceappmanagement-get.md)|Чтение свойств и связей объекта [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).|
|[Обновление объекта deviceAppManagement](../api/intune-shared-deviceappmanagement-update.md)|Обновление свойств объекта [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).|
|**Адаптация**|
|[Действие syncMicrosoftStoreForBusinessApps](../api/intune-shared-deviceappmanagement-syncmicrosoftstoreforbusinessapps.md)|Нет|Синхронизирует учетную запись Intune с Microsoft Store для бизнеса|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|**Адаптация**|
|isEnabledForMicrosoftStoreForBusiness|Boolean|Указывает, включена ли для учетной запись синхронизация приложений из Microsoft Store для бизнеса.|
|microsoftStoreForBusinessLanguage|String|Сведения о языковом стандарте, используемом для синхронизации приложений из Microsoft Store для бизнеса. Региональные параметры, относящиеся к стране или региону. Названия этих региональных параметров соответствуют стандарту RFC 4646 (для Windows Vista и более поздних версий). Используется формат <languagecode2>-<страна/код_региона2>, где <languagecode2> — это двухбуквенный код в нижнем регистре, полученный из стандарта ISO 639-1, а <страна/код_регион2> — код из двух прописных букв по стандарту ISO 3166. Например, en-US для английского (США) — это определенный региональный стандарт.|
|microsoftStoreForBusinessLastCompletedApplicationSyncTime|DateTimeOffset|Время последней завершенной синхронизации приложений из Microsoft Store для бизнеса.|
|microsoftStoreForBusinessLastSuccessfulSyncDateTime|DateTimeOffset|Время последней успешной синхронизации приложений из Microsoft Store для бизнеса с учетной записью.|
|MicrosoftStoreForBusinessPortalSelection|[microsoftStoreForBusinessPortalSelectionOptions](../resources/intune-onboarding-microsoftstoreforbusinessportalselectionoptions.md)|Сведения о портале конечных пользователей используются для синхронизации приложений с Microsoft Store для бизнеса до Корпоративный портал Intune. Существует три варианта выбора из "Только портала компании", "Портал компании и частный \[ магазин", "Только частный \] магазин". Возможные значения: `none`, `companyPortal`, `privateStore`.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|**Приложения**|
|enterpriseCodeSigningCertificates|[коллекция enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)|Сертификат Windows Enterprise кода.|
|iosLobAppProvisioningConfigurations|[коллекция iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md)|Конфигурации подготовка приложений IOS Lob.|
|mobileAppCategories|Коллекция [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Категории мобильных приложений|
|mobileAppConfigurations|Коллекция [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)|Конфигурации мобильных приложений для управляемых устройств.|
|mobileApps|Коллекция [mobileApp](../resources/intune-shared-mobileapp.md)|Мобильные приложения.|
|symantecCodeSigningCertificate|[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)|Сертификат подписи кода WinPhone Symantec.|
|**Книги**|
|managedEBooks|Коллекция [managedEBook](../resources/intune-books-managedebook.md)|Управляемая электронная книга.|
|managedEBookCategories|[коллекция managedEBookCategory](../resources/intune-books-managedebookcategory.md)|Категории мобильных книг.|
|**Управление устройствами**|
|windowsManagementApp|[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)|Windows управления приложением.|
|**Управление мобильным приложением (MAM)**|
|androidManagedAppProtections|Коллекция [androidManagedAppProtection](../resources/intune-shared-androidmanagedappprotection.md)|Политики управляемых приложений для Android.|
|defaultManagedAppProtections|Коллекция [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md)|Политики управляемых приложений по умолчанию.|
|iosManagedAppProtections|Коллекция [iosManagedAppProtection](../resources/intune-shared-iosmanagedappprotection.md)|Политики управляемых приложений для iOS.|
|managedAppPolicies|Коллекция [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|Политики управляемых приложений.|
|managedAppRegistrations|Коллекция [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|Регистрации управляемых приложений.|
|managedAppStatuses|Коллекция [managedAppStatus](../resources/intune-mam-managedappstatus.md)|Состояния управляемых приложений.|
|mdmWindowsInformationProtectionPolicies|Коллекция [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md)|Windows Information Protection для приложений на устройствах, зарегистрированных с использованием MDM.|
|targetedManagedAppConfigurations|Коллекция [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md)|Целевые конфигурации управляемых приложений.|
|windowsInformationProtectionPolicies|Коллекция [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md)|Windows Information Protection для приложений на устройствах, не зарегистрированных с использованием MDM.|
|**Адаптация**|
|sideLoadingKeys|[коллекция sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)|Клавиши боковой загрузки, необходимые для установки Windows 8 и 8.1 Apps.|
|VPP токены|[vpp Токен](../resources/intune-onboarding-vpptoken.md) коллекция|Список Vpp маркеров для данной организации.|
|**Набор политик**|
|policySets|[коллекция policySet](../resources/intune-policyset-policyset.md)|The PolicySet of Policies and Applications|
|mobileApps|Коллекция [mobileApp](../resources/intune-shared-mobileapp.md)|Мобильные приложения.|
|targetedManagedAppConfigurations|Коллекция [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md)|Целевые конфигурации управляемых приложений.|
|androidManagedAppProtections|Коллекция [androidManagedAppProtection](../resources/intune-shared-androidmanagedappprotection.md)|Политики управляемых приложений для Android.|
|iosManagedAppProtections|Коллекция [iosManagedAppProtection](../resources/intune-shared-iosmanagedappprotection.md)|Политики управляемых приложений для iOS.|
|mdmWindowsInformationProtectionPolicies|Коллекция [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md)|Windows Information Protection для приложений на устройствах, зарегистрированных с использованием MDM.|
|iosLobAppProvisioningConfigurations|[коллекция iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md)|Конфигурации подготовка приложений IOS Lob.|
|**Интеграция партнеров**|
|deviceAppManagementTasks|[коллекция deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|Задачи управления приложениями устройства.|
|**Unlock**|
|wdacSupplementalPolicies|[коллекция windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md)|Коллекция дополнительных политик Защитник Windows управления приложениями.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.  Обратите внимание, что это только пример; Ответы запроса на фактические запросы будут содержать свойства, соответствующие контексту.  
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAppManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "String (identifier)",
  "microsoftStoreForBusinessLastSuccessfulSyncDateTime": "String (timestamp)",
  "isEnabledForMicrosoftStoreForBusiness": true,
  "microsoftStoreForBusinessLanguage": "String",
  "microsoftStoreForBusinessLastCompletedApplicationSyncTime": "String (timestamp)"
}
```



