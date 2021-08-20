---
title: Обновление intuneBrandingProfile
description: Обновление свойств объекта intuneBrandingProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a066bcb055101b639833f1f81ecca61d57b6acbd716631db67389c7453b5996d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54207245"
---
# <a name="update-intunebrandingprofile"></a>Обновление intuneBrandingProfile

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [intuneBrandingProfile.](../resources/intune-wip-intunebrandingprofile.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementApps.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementApps.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для [объекта intuneBrandingProfile.](../resources/intune-wip-intunebrandingprofile.md)

В следующей таблице показаны свойства, необходимые при создании [intuneBrandingProfile.](../resources/intune-wip-intunebrandingprofile.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ профиля|
|имя профиля|Строка|Имя профиля|
|profileDescription|Строка|Описание профиля|
|isDefaultProfile|Логический|Boolean, который представляет, используется ли профиль как по умолчанию или нет|
|createdDateTime|DateTimeOffset|Время создания BrandingProfile|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения BrandingProfile|
|displayName|Строка|Имя компании или организации, отображаемая конечным пользователям|
|themeColor|[rgbColor](../resources/intune-shared-rgbcolor.md)|Основной цвет темы, используемый в Корпоративный портал приложениях и веб-портале|
|showLogo|Boolean|Boolean, который представляет, показаны ли изображения логотипа, предоставленные администратором, или нет.|
|showDisplayNameNextToLogo|Boolean|Boolean, который представляет, будет ли отображаться имя дисплея, предоставленное администратором, рядом с изображением логотипа или нет.|
|themeColorLogo|[mimeContent](../resources/intune-shared-mimecontent.md);|Изображение логотипа, отображаемого в Корпоративный портал приложениях с фоном цвета темы за логотипом|
|lightBackgroundLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|Изображение логотипа, отображаемого в Корпоративный портал приложениях со светлым фоном за логотипом|
|landingPageCustomizedImage|[mimeContent](../resources/intune-shared-mimecontent.md);|Настраиваемый образ, отображаемый на Корпоративный портал странице Корпоративный портал приложений|
|contactITName|String|Имя лица или организации, ответственной за ИТ-поддержку|
|contactITPhoneNumber|String|Телефон человека или организации, ответственной за ИТ-поддержку|
|contactITEmailAddress|String|Адрес электронной почты лица или организации, ответственной за ИТ-поддержку|
|contactITNotes|String|Текстовые комментарии в отношении лица или организации, ответственной за ИТ-поддержку|
|onlineSupportSiteUrl|String|URL-адрес сайта it-справки компании/организации|
|onlineSupportSiteName|String|Отображение имени сайта it-справки компании/организации|
|privacyUrl|String|URL-адрес политики конфиденциальности компании и организации|
|customPrivacyMessage|Строка|Текстовые комментарии относительно того, к чему администратор не имеет доступа на устройстве|
|customCanSeePrivacyMessage|String|Текстовые комментарии относительно доступа администратора к устройству|
|customCantSeePrivacyMessage|Строка|Текстовые комментарии относительно того, к чему администратор не имеет доступа на устройстве|
|isRemoveDeviceDisabled|Логический|Boolean, который представляет, отключил ли администратор действие "Удалить устройство" на корпоративных устройствах.|
|isFactoryResetDisabled|Логический|Boolean, который представляет, отключил ли администратор действие "Сброс фабрики" на корпоративных устройствах.|
|companyPortalBlockedActions|[коллекция companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md)|Коллекция заблокированных действий на портале компании в зависимости от типов владения платформой и устройствами.|
|showAzureADEnterpriseApps|Логический|Boolean, который указывает, будут ли Enterprise AzureAD приложения будут показаны в Корпоративный портал|
|showOfficeWebApps|Логический|Boolean, который указывает, Office веб-приложения будут показаны в Корпоративный портал|
|sendDeviceOwnershipChangePushNotification|Логический|Boolean, который указывает, отправляется ли пользователям push-уведомление при смене типа владения устройствами с личного на корпоративный.|
|enrollmentAvailability|[enrollmentAvailabilityOptions](../resources/intune-shared-enrollmentavailabilityoptions.md)|Настраиваемый поток регистрации устройств, отображаемый конечному пользователю. Возможные значения: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.|
|отключениеClientTelemetry|Логический|Применяется к телеметрии, отправленной от всех клиентов в службу Intune. При отключении все упреждающие предупреждения о неполадок в клиенте отключаются, а параметры телеметрии отображаются неактивными или скрытыми для пользователя устройства.|
|roleScopeTagIds|Коллекция String|Список тегов области, присвоенных профилю брендинга|



## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код ответа и обновленный `200 OK` [объект intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
Content-type: application/json
Content-length: 1975

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfile",
  "profileName": "Profile Name value",
  "profileDescription": "Profile Description value",
  "isDefaultProfile": true,
  "displayName": "Display Name value",
  "themeColor": {
    "@odata.type": "microsoft.graph.rgbColor",
    "r": 1,
    "g": 1,
    "b": 1
  },
  "showLogo": true,
  "showDisplayNameNextToLogo": true,
  "themeColorLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "contactITName": "Contact ITName value",
  "contactITPhoneNumber": "Contact ITPhone Number value",
  "contactITEmailAddress": "Contact ITEmail Address value",
  "contactITNotes": "Contact ITNotes value",
  "onlineSupportSiteUrl": "https://example.com/onlineSupportSiteUrl/",
  "onlineSupportSiteName": "Online Support Site Name value",
  "privacyUrl": "https://example.com/privacyUrl/",
  "customPrivacyMessage": "Custom Privacy Message value",
  "customCanSeePrivacyMessage": "Custom Can See Privacy Message value",
  "customCantSeePrivacyMessage": "Custom Cant See Privacy Message value",
  "isRemoveDeviceDisabled": true,
  "isFactoryResetDisabled": true,
  "companyPortalBlockedActions": [
    {
      "@odata.type": "microsoft.graph.companyPortalBlockedAction",
      "platform": "androidForWork",
      "ownerType": "company",
      "action": "remove"
    }
  ],
  "showAzureADEnterpriseApps": true,
  "showOfficeWebApps": true,
  "sendDeviceOwnershipChangePushNotification": true,
  "enrollmentAvailability": "availableWithoutPrompts",
  "disableClientTelemetry": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2147

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfile",
  "id": "fcd6136c-136c-fcd6-6c13-d6fc6c13d6fc",
  "profileName": "Profile Name value",
  "profileDescription": "Profile Description value",
  "isDefaultProfile": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "themeColor": {
    "@odata.type": "microsoft.graph.rgbColor",
    "r": 1,
    "g": 1,
    "b": 1
  },
  "showLogo": true,
  "showDisplayNameNextToLogo": true,
  "themeColorLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "contactITName": "Contact ITName value",
  "contactITPhoneNumber": "Contact ITPhone Number value",
  "contactITEmailAddress": "Contact ITEmail Address value",
  "contactITNotes": "Contact ITNotes value",
  "onlineSupportSiteUrl": "https://example.com/onlineSupportSiteUrl/",
  "onlineSupportSiteName": "Online Support Site Name value",
  "privacyUrl": "https://example.com/privacyUrl/",
  "customPrivacyMessage": "Custom Privacy Message value",
  "customCanSeePrivacyMessage": "Custom Can See Privacy Message value",
  "customCantSeePrivacyMessage": "Custom Cant See Privacy Message value",
  "isRemoveDeviceDisabled": true,
  "isFactoryResetDisabled": true,
  "companyPortalBlockedActions": [
    {
      "@odata.type": "microsoft.graph.companyPortalBlockedAction",
      "platform": "androidForWork",
      "ownerType": "company",
      "action": "remove"
    }
  ],
  "showAzureADEnterpriseApps": true,
  "showOfficeWebApps": true,
  "sendDeviceOwnershipChangePushNotification": true,
  "enrollmentAvailability": "availableWithoutPrompts",
  "disableClientTelemetry": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```




