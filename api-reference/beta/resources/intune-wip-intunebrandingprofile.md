---
title: Тип ресурса Интунебрандингпрофиле
description: Эта сущность содержит данные, которые используются при настройке внешнего вида уровня клиента для приложений корпоративного портала и веб-портала конечных пользователей.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: de98ae69eafcb076ca36985513d1fe3b3c601ac1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43471954"
---
# <a name="intunebrandingprofile-resource-type"></a>Тип ресурса Интунебрандингпрофиле

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Эта сущность содержит данные, которые используются при настройке внешнего вида уровня клиента для приложений корпоративного портала и веб-портала конечных пользователей.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Интунебрандингпрофилес](../api/intune-wip-intunebrandingprofile-list.md)|Коллекция [интунебрандингпрофиле](../resources/intune-wip-intunebrandingprofile.md)|Список свойств и связей объектов [интунебрандингпрофиле](../resources/intune-wip-intunebrandingprofile.md) .|
|[Получение Интунебрандингпрофиле](../api/intune-wip-intunebrandingprofile-get.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|Чтение свойств и связей объекта [интунебрандингпрофиле](../resources/intune-wip-intunebrandingprofile.md) .|
|[Создание Интунебрандингпрофиле](../api/intune-wip-intunebrandingprofile-create.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|Создание нового объекта [интунебрандингпрофиле](../resources/intune-wip-intunebrandingprofile.md) .|
|[Удаление Интунебрандингпрофиле](../api/intune-wip-intunebrandingprofile-delete.md)|Нет|Удаляет объект [интунебрандингпрофиле](../resources/intune-wip-intunebrandingprofile.md).|
|[Обновление Интунебрандингпрофиле](../api/intune-wip-intunebrandingprofile-update.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|Обновление свойств объекта [интунебрандингпрофиле](../resources/intune-wip-intunebrandingprofile.md) .|
|[Действие assign](../api/intune-wip-intunebrandingprofile-assign.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ профиля|
|имя_профиля|String|Имя профиля|
|профиледескриптион|String|Описание профиля|
|исдефаултпрофиле|Boolean|Логическое значение, указывающее, используется ли профиль по умолчанию или нет|
|createdDateTime|DateTimeOffset|Время создания Брандингпрофиле|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения Брандингпрофиле|
|displayName|Строка|Название компании или организации, которое отображается для конечных пользователей|
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
|кустомпривацимессаже|String|Текстовые комментарии относительно того, что у администратора есть доступ к устройству.|
|исремоведевицедисаблед|Boolean|Логическое значение, указывающее, отключил ли админсистратор действие "Remove Device" на корпоративных устройствах.|
|исфакториресетдисаблед|Boolean|Логическое значение, указывающее, отключил ли админсистратор действие "Фабричная сброс" на корпоративных устройствах.|
|компанипорталблоккедактионс|Коллекция [компанипорталблоккедактион](../resources/intune-shared-companyportalblockedaction.md)|Коллекция заблокированных действий на портале компании в соответствии с типом владения платформой и устройствами.|
|шовазуреадентерприсеаппс|Boolean|Логическое значение, которое указывает, будут ли отображаться корпоративные приложения AzureAD на портале компании.|
|шовоффицевебаппс|Boolean|Логическое значение, указывающее, будут ли отображаться приложения Office на портале компании.|
|сенддевицеовнершипчанжепушнотификатион|Boolean|Логическое значение, указывающее, отправляются ли пользователям push-уведомления, если их тип собственности изменяется от персонального к корпоративному.|
|енроллментаваилабилити|[enrollmentAvailabilityOptions](../resources/intune-shared-enrollmentavailabilityoptions.md)|Настраиваемый процесс регистрации устройства, отображаемый для конечного пользователя. Возможные значения: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.|
|roleScopeTagIds|Коллекция объектов string|Список тегов области, назначенных профилю фирменной символики|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|Коллекция [интунебрандингпрофилеассигнмент](../resources/intune-wip-intunebrandingprofileassignment.md)|Список назначений групп для профиля фирменной символики|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.intuneBrandingProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.intuneBrandingProfile",
  "id": "String (identifier)",
  "profileName": "String",
  "profileDescription": "String",
  "isDefaultProfile": true,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "themeColor": {
    "@odata.type": "microsoft.graph.rgbColor",
    "r": 1024,
    "g": 1024,
    "b": 1024
  },
  "showLogo": true,
  "showDisplayNameNextToLogo": true,
  "themeColorLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "contactITName": "String",
  "contactITPhoneNumber": "String",
  "contactITEmailAddress": "String",
  "contactITNotes": "String",
  "onlineSupportSiteUrl": "String",
  "onlineSupportSiteName": "String",
  "privacyUrl": "String",
  "customPrivacyMessage": "String",
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
  "roleScopeTagIds": [
    "String"
  ]
}
```



