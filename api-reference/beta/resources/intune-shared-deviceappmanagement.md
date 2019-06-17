---
title: Тип ресурса deviceAppManagement
description: Одноэлементный объект, служащий контейнером для всех функций управления приложениями на устройствах.
author: rolyon
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9ebb14421204c364e04a7151f7898d253798f440
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34996129"
---
# <a name="deviceappmanagement-resource-type"></a>Тип ресурса deviceAppManagement

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Одноэлементный объект, служащий контейнером для всех функций управления приложениями на устройствах.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение объекта deviceAppManagement](../api/intune-shared-deviceappmanagement-get.md)|Чтение свойств и связей объекта [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).|
|[Обновление объекта deviceAppManagement](../api/intune-shared-deviceappmanagement-update.md)|Обновление свойств объекта [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).|
|**Входящая миграция**|
|[Действие syncMicrosoftStoreForBusinessApps](../api/intune-shared-deviceappmanagement-syncmicrosoftstoreforbusinessapps.md)|Нет|Синхронизирует учетную запись Intune с Microsoft Store для бизнеса|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|**Входящая миграция**|
|isEnabledForMicrosoftStoreForBusiness|Boolean|Указывает, включена ли для учетной запись синхронизация приложений из Microsoft Store для бизнеса.|
|microsoftStoreForBusinessLanguage|String|Сведения о языковом стандарте, используемом для синхронизации приложений из Microsoft Store для бизнеса. Региональные параметры, относящиеся к стране или региону. Названия этих региональных параметров соответствуют стандарту RFC 4646 (для Windows Vista и более поздних версий). Используется формат <languagecode2>-<страна/код_региона2>, где <languagecode2> — это двухбуквенный код в нижнем регистре, полученный из стандарта ISO 639-1, а <страна/код_регион2> — код из двух прописных букв по стандарту ISO 3166. Например, en-US для английского (США) — это определенный региональный стандарт.|
|microsoftStoreForBusinessLastCompletedApplicationSyncTime|DateTimeOffset|Время последней завершенной синхронизации приложений из Microsoft Store для бизнеса.|
|microsoftStoreForBusinessLastSuccessfulSyncDateTime|DateTimeOffset|Время последней успешной синхронизации приложений из Microsoft Store для бизнеса с учетной записью.|
|Микрософтсторефорбусинесспорталселектион|[microsoftStoreForBusinessPortalSelectionOptions](../resources/intune-onboarding-microsoftstoreforbusinessportalselectionoptions.md)|Сведения о портале конечного пользователя используются для синхронизации приложений из Microsoft Store для бизнеса и портала компании Intune. Выбрать можно три варианта: \["только корпоративный портал", "Корпоративный портал и частный магазин", "только частный магазин".\] Возможные значения: `none`, `companyPortal`, `privateStore`.|

## <a name="relationships"></a>Отношения
|Отношение|Тип|Описание|
|:---|:---|:---|
|**Приложения**|
|enterpriseCodeSigningCertificates|Коллекция [ентерприсекодесигнингцертификате](../resources/intune-apps-enterprisecodesigningcertificate.md)|Сертификат для подписи кода предприятия Windows.|
|iosLobAppProvisioningConfigurations|Коллекция [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)|Конфигурации подготовки бизнес-приложений IOS.|
|mobileAppCategories|Коллекция [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Категории мобильных приложений|
|mobileAppConfigurations|Коллекция [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)|Конфигурации мобильных приложений для управляемых устройств.|
|mobileApps|Коллекция [mobileApp](../resources/intune-apps-mobileapp.md)|Мобильные приложения.|
|symantecCodeSigningCertificate|[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md);|Сертификат для подписи кода Винфоне Symantec.|
|**Книг**|
|managedEBooks|Коллекция [managedEBook](../resources/intune-books-managedebook.md)|Управляемая электронная книга.|
|Манажедебуккатегориес|Коллекция [манажедебуккатегори](../resources/intune-books-managedebookcategory.md)|Категории мобильных электронных книг.|
|**Управление устройствами**|
|windowsManagementApp|[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)|Приложение управления Windows.|
|**Управление мобильным приложением (MAM)**|
|androidManagedAppProtections|Коллекция [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md)|Политики управляемых приложений для Android.|
|defaultManagedAppProtections|Коллекция [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md)|Политики управляемых приложений по умолчанию.|
|iosManagedAppProtections|Коллекция [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md)|Политики управляемых приложений для iOS.|
|managedAppPolicies|Коллекция [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|Политики управляемых приложений.|
|managedAppRegistrations|Коллекция [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|Регистрации управляемых приложений.|
|managedAppStatuses|Коллекция [managedAppStatus](../resources/intune-mam-managedappstatus.md)|Состояния управляемых приложений.|
|mdmWindowsInformationProtectionPolicies|Коллекция [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md)|Windows Information Protection для приложений на устройствах, зарегистрированных с использованием MDM.|
|targetedManagedAppConfigurations|Коллекция [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)|Целевые конфигурации управляемых приложений.|
|windowsInformationProtectionPolicies|Коллекция [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md)|Windows Information Protection для приложений на устройствах, не зарегистрированных с использованием MDM.|
|**Входящая миграция**|
|sideLoadingKeys|Коллекция [сиделоадингкэй](../resources/intune-onboarding-sideloadingkey.md)|Ключи загрузки на стороне, необходимые для установки приложений для Windows 8 и 8,1.|
|VPP токены|[vpp Токен](../resources/intune-onboarding-vpptoken.md) коллекция|Список Vpp маркеров для данной организации.|
|**Интеграция партнеров**|
|Девицеаппманажементтаскс|Коллекция [девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md)|Задачи управления приложениями для устройств.|

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



