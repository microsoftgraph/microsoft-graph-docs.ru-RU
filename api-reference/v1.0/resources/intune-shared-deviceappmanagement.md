---
title: Тип ресурса deviceAppManagement
description: Одноэлементный объект, служащий контейнером для всех функций управления приложениями на устройствах.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 169db36319b9436900d5b6664fb5422828ad6689
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732766"
---
# <a name="deviceappmanagement-resource-type"></a>Тип ресурса deviceAppManagement

Пространство имен: microsoft.graph

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

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|**Приложения**|
|mobileAppCategories|Коллекция [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Категории мобильных приложений|
|mobileAppConfigurations|Коллекция [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)|Конфигурации мобильных приложений для управляемых устройств.|
|mobileApps|Коллекция [mobileApp](../resources/intune-apps-mobileapp.md)|Мобильные приложения.|
|**Книги**|
|managedEBooks|Коллекция [managedEBook](../resources/intune-books-managedebook.md)|Управляемая электронная книга.|
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
|**Адаптация**|
|VPP токены|[vpp Токен](../resources/intune-onboarding-vpptoken.md) коллекция|Список Vpp маркеров для данной организации.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.  Обратите внимание, что это только пример; Ответы запроса на фактические запросы будут содержать свойства, соответствующие контексту.  
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
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









