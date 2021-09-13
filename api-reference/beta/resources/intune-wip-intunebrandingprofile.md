---
title: тип ресурса intuneBrandingProfile
description: Эта сущность содержит данные, используемые при настройке внешнего вида Корпоративный портал приложений, а также веб-портала конечного пользователя.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 280584694d5aa73cf412f7572f1d0f9aba28612c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59054172"
---
# <a name="intunebrandingprofile-resource-type"></a>тип ресурса intuneBrandingProfile

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Эта сущность содержит данные, используемые при настройке внешнего вида Корпоративный портал приложений, а также веб-портала конечного пользователя.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список intuneBrandingProfiles](../api/intune-wip-intunebrandingprofile-list.md)|[коллекция intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|Список свойств и связей объектов [intuneBrandingProfile.](../resources/intune-wip-intunebrandingprofile.md)|
|[Получить intuneBrandingProfile](../api/intune-wip-intunebrandingprofile-get.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|Чтение свойств и связей [объекта intuneBrandingProfile.](../resources/intune-wip-intunebrandingprofile.md)|
|[Создание intuneBrandingProfile](../api/intune-wip-intunebrandingprofile-create.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|Создайте новый [объект intuneBrandingProfile.](../resources/intune-wip-intunebrandingprofile.md)|
|[Удаление intuneBrandingProfile](../api/intune-wip-intunebrandingprofile-delete.md)|Нет|Удаляет [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md).|
|[Обновление intuneBrandingProfile](../api/intune-wip-intunebrandingprofile-update.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|Обновление свойств объекта [intuneBrandingProfile.](../resources/intune-wip-intunebrandingprofile.md)|
|[Действие assign](../api/intune-wip-intunebrandingprofile-assign.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ профиля|
|имя профиля|String|Имя профиля|
|profileDescription|String|Описание профиля|
|isDefaultProfile|Логическое|Boolean, который представляет, используется ли профиль как по умолчанию или нет|
|createdDateTime|DateTimeOffset|Время создания BrandingProfile|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения BrandingProfile|
|displayName|String|Имя компании или организации, отображаемая конечным пользователям|
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
|customPrivacyMessage|String|Текстовые комментарии относительно того, к чему администратор не имеет доступа на устройстве|
|customCanSeePrivacyMessage|String|Текстовые комментарии относительно доступа администратора к устройству|
|customCantSeePrivacyMessage|String|Текстовые комментарии относительно того, к чему администратор не имеет доступа на устройстве|
|isRemoveDeviceDisabled|Логический|Boolean, который представляет, отключил ли администратор действие "Удалить устройство" на корпоративных устройствах.|
|isFactoryResetDisabled|Логический|Boolean, который представляет, отключил ли администратор действие "Сброс фабрики" на корпоративных устройствах.|
|companyPortalBlockedActions|[коллекция companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md)|Коллекция заблокированных действий на портале компании в зависимости от типов владения платформой и устройствами.|
|showAzureADEnterpriseApps|Логическое|Boolean, который указывает, будут ли Enterprise AzureAD приложения будут показаны в Корпоративный портал|
|showOfficeWebApps|Логическое|Boolean, который указывает, Office веб-приложения будут показаны в Корпоративный портал|
|sendDeviceOwnershipChangePushNotification|Логический|Boolean, который указывает, отправляется ли пользователям push-уведомление при смене типа владения устройствами с личного на корпоративный.|
|enrollmentAvailability|[enrollmentAvailabilityOptions](../resources/intune-shared-enrollmentavailabilityoptions.md)|Настраиваемый поток регистрации устройств, отображаемый конечному пользователю. Возможные значения: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.|
|отключениеClientTelemetry|Логическое|Применяется к телеметрии, отправленной от всех клиентов в службу Intune. При отключении все упреждающие предупреждения о неполадок в клиенте отключаются, а параметры телеметрии отображаются неактивными или скрытыми для пользователя устройства.|
|roleScopeTagIds|Коллекция объектов string|Список тегов области, присвоенных профилю брендинга|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|[коллекция intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)|Список групповых назначений для профиля брендинга|

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
  "customCanSeePrivacyMessage": "String",
  "customCantSeePrivacyMessage": "String",
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
  "disableClientTelemetry": true,
  "roleScopeTagIds": [
    "String"
  ]
}
```



