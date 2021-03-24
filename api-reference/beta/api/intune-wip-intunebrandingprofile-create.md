---
title: Создание intuneBrandingProfile
description: Создайте новый объект intuneBrandingProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0e6b8d89b2575402cc38b5f86ecd8a872fd666b3
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133854"
---
# <a name="create-intunebrandingprofile"></a>Создание intuneBrandingProfile

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создайте новый [объект intuneBrandingProfile.](../resources/intune-wip-intunebrandingprofile.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)|DeviceManagementApps.ReadWrite.All|
|Делегированное (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementApps.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intuneBrandingProfiles
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для объекта intuneBrandingProfile.

В следующей таблице показаны свойства, необходимые при создании intuneBrandingProfile.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ профиля|
|имя профиля|Строка|Имя профиля|
|profileDescription|Строка|Описание профиля|
|isDefaultProfile|Boolean|Boolean, который представляет, используется ли профиль как по умолчанию или нет|
|createdDateTime|DateTimeOffset|Время создания BrandingProfile|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения BrandingProfile|
|displayName|Строка|Имя компании или организации, отображаемая конечным пользователям|
|themeColor|[rgbColor](../resources/intune-shared-rgbcolor.md)|Основной цвет темы, используемый в приложениях портала компании и веб-портале|
|showLogo|Boolean|Boolean, который представляет, показаны ли изображения логотипа, предоставленные администратором, или нет.|
|showDisplayNameNextToLogo|Boolean|Boolean, который представляет, будет ли отображаться имя дисплея, предоставленное администратором, рядом с изображением логотипа или нет.|
|themeColorLogo|[mimeContent](../resources/intune-shared-mimecontent.md);|Изображение логотипа, отображаемого в приложениях портала компании, которые имеют фон цвета темы за логотипом|
|lightBackgroundLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|Изображение логотипа, отображаемого в приложениях портала компании, которые имеют светлый фон за логотипом|
|landingPageCustomizedImage|[mimeContent](../resources/intune-shared-mimecontent.md);|Настраиваемые изображения, отображаемые на странице посадки приложений портала компании|
|contactITName|String|Имя лица или организации, ответственной за ИТ-поддержку|
|contactITPhoneNumber|String|Номер телефона лица или организации, ответственной за ИТ-поддержку|
|contactITEmailAddress|String|Адрес электронной почты лица или организации, ответственной за ИТ-поддержку|
|contactITNotes|String|Текстовые комментарии в отношении лица или организации, ответственной за ИТ-поддержку|
|onlineSupportSiteUrl|String|URL-адрес сайта it-справки компании/организации|
|onlineSupportSiteName|String|Отображение имени сайта it-справки компании/организации|
|privacyUrl|String|URL-адрес политики конфиденциальности компании и организации|
|customPrivacyMessage|Строка|Текстовые комментарии относительно того, к чему администратор не имеет доступа на устройстве|
|customCanSeePrivacyMessage|Строка|Текстовые комментарии относительно доступа администратора к устройству|
|customCantSeePrivacyMessage|Строка|Текстовые комментарии относительно того, к чему администратор не имеет доступа на устройстве|
|isRemoveDeviceDisabled|Boolean|Boolean, который представляет, отключил ли администратор действие "Удалить устройство" на корпоративных устройствах.|
|isFactoryResetDisabled|Boolean|Boolean, который представляет, отключил ли администратор действие "Сброс фабрики" на корпоративных устройствах.|
|companyPortalBlockedActions|[коллекция companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md)|Коллекция заблокированных действий на портале компании в зависимости от типов владения платформой и устройствами.|
|showAzureADEnterpriseApps|Boolean|Boolean, который указывает, будут ли корпоративные приложения AzureAD показаны на портале компании|
|showOfficeWebApps|Boolean|Boolean, который указывает, будут ли веб-приложения Office показаны на портале компании|
|sendDeviceOwnershipChangePushNotification|Boolean|Boolean, который указывает, отправляется ли пользователям push-уведомление при смене типа владения устройствами с личного на корпоративный.|
|enrollmentAvailability|[enrollmentAvailabilityOptions](../resources/intune-shared-enrollmentavailabilityoptions.md)|Настраиваемый поток регистрации устройств, отображаемый конечному пользователю. Возможные значения: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.|
|отключениеClientTelemetry|Boolean|Применяется к телеметрии, отправленной от всех клиентов в службу Intune. При отключении все упреждающие предупреждения о неполадок в клиенте отключаются, а параметры телеметрии отображаются неактивными или скрытыми для пользователя устройства.|
|roleScopeTagIds|Коллекция String|Список тегов области, присвоенных профилю брендинга|



## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles
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
HTTP/1.1 201 Created
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




