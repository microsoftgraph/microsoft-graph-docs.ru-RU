---
title: Тип ресурса deviceAppManagement
description: Одноэлементный объект, служащий контейнером для всех функций управления приложениями на устройствах.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 197a44a9db9e42598592ff359cb3892298791eba
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523739"
---
# <a name="deviceappmanagement-resource-type"></a>Тип ресурса deviceAppManagement

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

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
|id|String|Ключ объекта.|
|**Адаптация**|
|isEnabledForMicrosoftStoreForBusiness|Boolean|Указывает, включена ли для учетной запись синхронизация приложений из Microsoft Store для бизнеса.|
|microsoftStoreForBusinessLanguage|String|Сведения о языковом стандарте, используемом для синхронизации приложений из Microsoft Store для бизнеса. Региональные параметры, относящиеся к стране или региону. Названия этих региональных параметров соответствуют стандарту RFC 4646 (для Windows Vista и более поздних версий). Используется формат <languagecode2>-<страна/код_региона2>, где <languagecode2> — это двухбуквенный код в нижнем регистре, полученный из стандарта ISO 639-1, а <страна/код_регион2> — код из двух прописных букв по стандарту ISO 3166. Например, en-US для английского (США) — это определенный региональный стандарт.|
|microsoftStoreForBusinessLastCompletedApplicationSyncTime|DateTimeOffset|Время последней завершенной синхронизации приложений из Microsoft Store для бизнеса.|
|microsoftStoreForBusinessLastSuccessfulSyncDateTime|DateTimeOffset|Время последней успешной синхронизации приложений из Microsoft Store для бизнеса с учетной записью.|
|микрософтсторефорбусинесспорталселектион|[microsoftStoreForBusinessPortalSelectionOptions](../resources/intune-onboarding-microsoftstoreforbusinessportalselectionoptions.md)|Сведения о портале конечного пользователя используются для синхронизации приложений из Microsoft Store для бизнеса и портала компании Intune. Выбрать можно три варианта: \["только корпоративный портал", "Корпоративный портал и частный магазин", "только частный магазин".\] Возможные значения: `none`, `companyPortal`, `privateStore`.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|**Приложения**|
|enterpriseCodeSigningCertificates|Коллекция [ентерприсекодесигнингцертификате](../resources/intune-apps-enterprisecodesigningcertificate.md)|Сертификат для подписи кода предприятия Windows.|
|iosLobAppProvisioningConfigurations|Коллекция [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md)|Конфигурации подготовки бизнес-приложений IOS.|
|mobileAppCategories|Коллекция [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Категории мобильных приложений|
|mobileAppConfigurations|Коллекция [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)|Конфигурации мобильных приложений для управляемых устройств.|
|mobileApps|Коллекция [mobileApp](../resources/intune-shared-mobileapp.md)|Мобильные приложения.|
|symantecCodeSigningCertificate|[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md);|Сертификат для подписи кода Винфоне Symantec.|
|**Книг**|
|managedEBooks|Коллекция [managedEBook](../resources/intune-books-managedebook.md)|Управляемая электронная книга.|
|манажедебуккатегориес|Коллекция [манажедебуккатегори](../resources/intune-books-managedebookcategory.md)|Категории мобильных электронных книг.|
|**Управление устройствами**|
|windowsManagementApp|[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)|Приложение управления Windows.|
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
|sideLoadingKeys|Коллекция [сиделоадингкэй](../resources/intune-onboarding-sideloadingkey.md)|Ключи загрузки на стороне, необходимые для установки приложений для Windows 8 и 8,1.|
|VPP токены|[vpp Токен](../resources/intune-onboarding-vpptoken.md) коллекция|Список Vpp маркеров для данной организации.|
|**Набор политик**|
|полицисетс|Коллекция набора [политик](../resources/intune-policyset-policyset.md)|Набор политик политик и приложений|
|mobileApps|Коллекция [mobileApp](../resources/intune-shared-mobileapp.md)|Мобильные приложения.|
|targetedManagedAppConfigurations|Коллекция [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md)|Целевые конфигурации управляемых приложений.|
|androidManagedAppProtections|Коллекция [androidManagedAppProtection](../resources/intune-shared-androidmanagedappprotection.md)|Политики управляемых приложений для Android.|
|iosManagedAppProtections|Коллекция [iosManagedAppProtection](../resources/intune-shared-iosmanagedappprotection.md)|Политики управляемых приложений для iOS.|
|mdmWindowsInformationProtectionPolicies|Коллекция [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md)|Windows Information Protection для приложений на устройствах, зарегистрированных с использованием MDM.|
|iosLobAppProvisioningConfigurations|Коллекция [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md)|Конфигурации подготовки бизнес-приложений IOS.|
|**Интеграция партнеров**|
|девицеаппманажементтаскс|Коллекция [девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md)|Задачи управления приложениями для устройств.|
|**Unlock**|
|вдаксупплементалполиЦиес|Коллекция [виндовсдефендераппликатионконтролсупплементалполици](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md)|Коллекция дополнительных политик для управления приложением защитника Windows.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.  Обратите внимание, что это пример; Ответы на запросы к реальным запросам будут содержать свойства, подходящие для контекста.  
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



