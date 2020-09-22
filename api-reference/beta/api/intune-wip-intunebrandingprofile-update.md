---
title: Обновление Интунебрандингпрофиле
description: Обновление свойств объекта Интунебрандингпрофиле.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4ae851c132bf9bdffa0bd9d4c3dee831418f3e0c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48062465"
---
# <a name="update-intunebrandingprofile"></a>Обновление Интунебрандингпрофиле

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [интунебрандингпрофиле](../resources/intune-wip-intunebrandingprofile.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementApps.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementApps.ReadWrite.All|

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
В тексте запроса добавьте представление объекта [интунебрандингпрофиле](../resources/intune-wip-intunebrandingprofile.md) в формате JSON.

В следующей таблице приведены свойства, необходимые при создании [интунебрандингпрофиле](../resources/intune-wip-intunebrandingprofile.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ профиля|
|имя_профиля|String|Имя профиля|
|профиледескриптион|String|Описание профиля|
|исдефаултпрофиле|Boolean|Логическое значение, указывающее, используется ли профиль по умолчанию или нет|
|createdDateTime|DateTimeOffset|Время создания Брандингпрофиле|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения Брандингпрофиле|
|displayName|String|Название компании или организации, которое отображается для конечных пользователей|
|themeColor|[rgbColor](../resources/intune-shared-rgbcolor.md)|Основной цвет темы, используемый в приложениях портала компании и на веб-портале|
|showLogo|Boolean|Логическое значение, указывающее, отображаются ли изображения логотипа, предоставленные администратором.|
|showDisplayNameNextToLogo|Boolean|Логическое значение, указывающее, будет ли отображаться отображаемое имя, предоставленное администратором, рядом с изображением логотипа.|
|семеколорлого|[mimeContent](../resources/intune-shared-mimecontent.md);|Изображение логотипа, отображаемое в приложениях корпоративного портала, у которых есть фоновый цвет темы позади логотипа|
|lightBackgroundLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|Изображение логотипа, отображаемое в приложениях корпоративного портала, у которых есть светлый фон позади логотипа|
|ландингпажекустомизедимаже|[mimeContent](../resources/intune-shared-mimecontent.md);|Настраиваемое изображение, отображаемое на начальной странице "приложения корпоративного портала"|
|contactITName|String|Имя пользователя или организации, ответственных за ИТ-поддержку|
|contactITPhoneNumber|String|Номер телефона пользователя или организации, ответственного за ИТ-поддержку|
|contactITEmailAddress|String|Адрес электронной почты пользователя или организации, ответственных за ИТ-поддержку|
|contactITNotes|String|Текстовые комментарии о лице или организации, ответственных за ИТ-поддержку|
|onlineSupportSiteUrl|String|URL-адрес сайта ИТ-службы технической поддержки компании или Организации|
|onlineSupportSiteName|String|Отображаемое имя сайта ИТ-службы технической поддержки компании или Организации|
|privacyUrl|String|URL-адрес политики конфиденциальности компании или Организации|
|кустомпривацимессаже|String|Текстовые комментарии относительно того, что у администратора нет доступа к устройству.|
|кустомкансипривацимессаже|String|Текстовые комментарии относительно того, что у администратора есть доступ к устройству.|
|кустомкантсипривацимессаже|String|Текстовые комментарии относительно того, что у администратора нет доступа к устройству.|
|исремоведевицедисаблед|Boolean|Логическое значение, указывающее, отключил ли админсистратор действие "Remove Device" на корпоративных устройствах.|
|исфакториресетдисаблед|Boolean|Логическое значение, указывающее, отключил ли админсистратор действие "Фабричная сброс" на корпоративных устройствах.|
|компанипорталблоккедактионс|Коллекция [компанипорталблоккедактион](../resources/intune-shared-companyportalblockedaction.md)|Коллекция заблокированных действий на портале компании в соответствии с типом владения платформой и устройствами.|
|шовазуреадентерприсеаппс|Boolean|Логическое значение, которое указывает, будут ли отображаться корпоративные приложения AzureAD на портале компании.|
|шовоффицевебаппс|Boolean|Логическое значение, указывающее, будут ли отображаться приложения Office на портале компании.|
|сенддевицеовнершипчанжепушнотификатион|Boolean|Логическое значение, указывающее, отправляются ли пользователям push-уведомления, если их тип собственности изменяется от персонального к корпоративному.|
|енроллментаваилабилити|[enrollmentAvailabilityOptions](../resources/intune-shared-enrollmentavailabilityoptions.md)|Настраиваемый процесс регистрации устройства, отображаемый для конечного пользователя. Возможные значения: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.|
|дисаблеклиенттелеметри|Boolean|Применяется к телеметрии, отправляемой со всех клиентов в службу Intune. Если этот параметр отключен, все предупреждения об устранении неполадок и неполадки в клиенте отключаются, и параметры телеметрии отображаются как неактивные или скрытые для пользователя устройства.|
|roleScopeTagIds|Коллекция String|Список тегов области, назначенных профилю фирменной символики|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [интунебрандингпрофиле](../resources/intune-wip-intunebrandingprofile.md) в тексте отклика.

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






