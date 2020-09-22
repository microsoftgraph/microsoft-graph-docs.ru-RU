---
title: Тип ресурса intuneBrand
description: Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложения "Корпоративный портал" и веб-портала пользователя.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4550fa46df5db366342495491f1e4207f1a1bffc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029493"
---
# <a name="intunebrand-resource-type"></a>Тип ресурса intuneBrand

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложений "Корпоративный портал" и веб-портала пользователя.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Название компании или организации, которое отображается пользователям.|
|themeColor|[rgbColor](../resources/intune-shared-rgbcolor.md)|Основной цвет темы, который используется в приложениях "Корпоративный портал" и на веб-портале.|
|showLogo|Boolean|Логическое значение, которое определяет, отображаются ли предоставленные администратором изображения логотипов.|
|lightBackgroundLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|Изображение с логотипом на светлом фоне, которое отображается в приложениях "Корпоративный портал".|
|darkBackgroundLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|Изображение с логотипом на темном фоне, которое отображается в приложениях "Корпоративный портал".|
|showNameNextToLogo|Boolean|Логическое значение, которое определяет, отображается ли возле изображения логотипа указанное администратором отображаемое имя.|
|ландингпажекустомизедимаже|[mimeContent](../resources/intune-shared-mimecontent.md);|Настраиваемое изображение, отображаемое на начальной странице приложения корпоративного портала|
|showDisplayNameNextToLogo|Boolean|Логическое значение, которое определяет, отображается ли возле изображения логотипа указанное администратором отображаемое имя.|
|roleScopeTagIds|Коллекция String|Список тегов областей, назначенных профилю фирменной символики по умолчанию|
|contactITName|String|Имя пользователя или название организации, ответственных за ИТ-поддержку.|
|contactITPhoneNumber|String|Номер телефона пользователя или организации, ответственных за ИТ-поддержку.|
|contactITEmailAddress|String|Адрес электронной почты пользователя или организации, ответственных за ИТ-поддержку.|
|contactITNotes|String|Текстовые комментарии в отношении пользователя или организации, ответственных за ИТ-поддержку.|
|onlineSupportSiteUrl|String|URL-адрес сайта ИТ-службы технической поддержки компании или организации.|
|onlineSupportSiteName|String|Отображаемое имя сайта ИТ-службы технической поддержки компании или организации.|
|privacyUrl|String|URL-адрес страницы с политикой конфиденциальности компании или организации.|
|кустомпривацимессаже|String|Настраиваемое сообщение о конфиденциальности, используемое для объяснения того, что Организация не может просматривать или делать на управляемых устройствах.|
|кустомкантсипривацимессаже|String|Настраиваемое сообщение о конфиденциальности, используемое для объяснения того, что Организация не может просматривать или делать на управляемых устройствах.|
|кустомкансипривацимессаже|String|Настраиваемое сообщение о конфиденциальности, используемое для объяснения того, что Организация может просматривать и выполнять на управляемых устройствах.|
|исремоведевицедисаблед|Boolean|Логическое значение, указывающее, отключил ли админсистратор действие "Remove Device" на корпоративных устройствах.|
|исфакториресетдисаблед|Boolean|Логическое значение, указывающее, отключил ли админсистратор действие "Фабричная сброс" на корпоративных устройствах.|
|компанипорталблоккедактионс|Коллекция [компанипорталблоккедактион](../resources/intune-shared-companyportalblockedaction.md)|Коллекция заблокированных действий на портале компании в соответствии с типом владения платформой и устройствами.|
|шовазуреадентерприсеаппс|Boolean|Логическое значение, которое указывает, будут ли отображаться корпоративные приложения AzureAD на портале компании.|
|шовоффицевебаппс|Boolean|Логическое значение, указывающее, будут ли отображаться приложения Office на портале компании.|
|сенддевицеовнершипчанжепушнотификатион|Boolean|Логическое значение, указывающее, отправляются ли пользователям push-уведомления, если их тип собственности изменяется от персонального к корпоративному.|
|енроллментаваилабилити|[enrollmentAvailabilityOptions](../resources/intune-shared-enrollmentavailabilityoptions.md)|Настраиваемый процесс регистрации устройства, отображаемый для конечного пользователя. Возможные значения: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.|
|дисаблеклиенттелеметри|Boolean|Применяется к телеметрии, отправляемой со всех клиентов в службу Intune. Если этот параметр отключен, все предупреждения об устранении неполадок и неполадки в клиенте отключаются, и параметры телеметрии отображаются как неактивные или скрытые для пользователя устройства.|

## <a name="relationships"></a>Отношения
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






