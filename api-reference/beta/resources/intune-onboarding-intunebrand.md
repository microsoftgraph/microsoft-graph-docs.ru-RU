---
title: Тип ресурса intuneBrand
description: Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложения "Корпоративный портал" и веб-портала пользователя.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3017408294f8b09abfadccae491ba54a2fbaa15d
ms.sourcegitcommit: 0076eb6abb89be3dca3575631924a74a5202be30
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2022
ms.locfileid: "64629269"
---
# <a name="intunebrand-resource-type"></a>Тип ресурса intuneBrand

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложений "Корпоративный портал" и веб-портала пользователя.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Название компании или организации, которое отображается пользователям.|
|themeColor|[rgbColor](../resources/intune-shared-rgbcolor.md)|Основной цвет темы, который используется в приложениях "Корпоративный портал" и на веб-портале.|
|showLogo|Boolean|Логическое значение, которое определяет, отображаются ли предоставленные администратором изображения логотипов.|
|lightBackgroundLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|Изображение с логотипом на светлом фоне, которое отображается в приложениях "Корпоративный портал".|
|darkBackgroundLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|Изображение с логотипом на темном фоне, которое отображается в приложениях "Корпоративный портал".|
|showNameNextToLogo|Boolean|Логическое значение, которое определяет, отображается ли возле изображения логотипа указанное администратором отображаемое имя.|
|landingPageCustomizedImage|[mimeContent](../resources/intune-shared-mimecontent.md);|Настраиваемые изображения, отображаемые на Корпоративный портал странице приложения|
|showDisplayNameNextToLogo|Boolean|Логическое значение, которое определяет, отображается ли возле изображения логотипа указанное администратором отображаемое имя.|
|roleScopeTagIds|Коллекция объектов string|Список тегов области, присвоенных профилю брендинга по умолчанию|
|contactITName|String|Имя пользователя или название организации, ответственных за ИТ-поддержку.|
|contactITPhoneNumber|String|Номер телефона пользователя или организации, ответственных за ИТ-поддержку.|
|contactITEmailAddress|String|Адрес электронной почты пользователя или организации, ответственных за ИТ-поддержку.|
|contactITNotes|String|Текстовые комментарии в отношении пользователя или организации, ответственных за ИТ-поддержку.|
|onlineSupportSiteUrl|String|URL-адрес сайта ИТ-службы технической поддержки компании или организации.|
|onlineSupportSiteName|String|Отображаемое имя сайта ИТ-службы технической поддержки компании или организации.|
|privacyUrl|String|URL-адрес страницы с политикой конфиденциальности компании или организации.|
|customPrivacyMessage|Строка|Пользовательское сообщение о конфиденциальности, используемом для объяснения того, что организация не может видеть или делать на управляемых устройствах.|
|customCantSeePrivacyMessage|Строка|Пользовательское сообщение о конфиденциальности, используемом для объяснения того, что организация не может видеть или делать на управляемых устройствах.|
|customCanSeePrivacyMessage|Строка|Пользовательское сообщение о конфиденциальности, используемом для объяснения того, что организация может видеть и делать на управляемых устройствах.|
|isRemoveDeviceDisabled|Boolean|Boolean, который представляет, отключил ли администратор действие "Удалить устройство" на корпоративных устройствах.|
|isFactoryResetDisabled|Логическое|Boolean, который представляет, отключил ли администратор действие "Сброс фабрики" на корпоративных устройствах.|
|companyPortalBlockedActions|[коллекция companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md)|Коллекция заблокированных действий на портале компании в зависимости от типов владения платформой и устройствами.|
|showAzureADEnterpriseApps|Boolean|Boolean, который указывает, будут ли Enterprise AzureAD apps в Корпоративный портал|
|showOfficeWebApps|Boolean|Boolean, который указывает, Office веб-приложения будут показаны в Корпоративный портал|
|sendDeviceOwnershipChangePushNotification|Boolean|SendDeviceOwnershipChangePushNotification будет обесценен в 06/2022 и перестанет возвращать значение в 07/2022. A boolean that indicates if a push notification is sent to users when their device ownership type changes from personal to corporate|
|enrollmentAvailability|[enrollmentAvailabilityOptions](../resources/intune-shared-enrollmentavailabilityoptions.md)|Настраиваемый поток регистрации устройств, отображаемый конечному пользователю. Возможные значения: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.|
|отключениеClientTelemetry|Логический|Применяется к телеметрии, отосланной от всех клиентов в Intune службу. При отключении все упреждающие предупреждения о неполадок в клиенте отключаются, а параметры телеметрии отображаются неактивными или скрытыми для пользователя устройства.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.intuneBrand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.intuneBrand",
  "displayName": "String",
  "themeColor": {
    "@odata.type": "microsoft.graph.rgbColor",
    "r": 1024,
    "g": 1024,
    "b": 1024
  },
  "showLogo": true,
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "darkBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "showNameNextToLogo": true,
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "showDisplayNameNextToLogo": true,
  "roleScopeTagIds": [
    "String"
  ],
  "contactITName": "String",
  "contactITPhoneNumber": "String",
  "contactITEmailAddress": "String",
  "contactITNotes": "String",
  "onlineSupportSiteUrl": "String",
  "onlineSupportSiteName": "String",
  "privacyUrl": "String",
  "customPrivacyMessage": "String",
  "customCantSeePrivacyMessage": "String",
  "customCanSeePrivacyMessage": "String",
  "isRemoveDeviceDisabled": true,
  "isFactoryResetDisabled": true,
  "companyPortalBlockedActions": [
    {
      "@odata.type": "microsoft.graph.companyPortalBlockedAction",
      "platform": "String",
      "ownerType": "String",
      "action": "String"
    }
  ],
  "showAzureADEnterpriseApps": true,
  "showOfficeWebApps": true,
  "sendDeviceOwnershipChangePushNotification": true,
  "enrollmentAvailability": "String",
  "disableClientTelemetry": true
}
```




