---
title: Тип ресурса Интунебрандингпрофиле
description: Эта сущность содержит данные, которые используются при настройке внешнего вида уровня клиента для приложений корпоративного портала и веб-портала конечных пользователей.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6063b07ed9361b00315a7c8a2b170cea72f7dff3
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371910"
---
# <a name="intunebrandingprofile-resource-type"></a>Тип ресурса Интунебрандингпрофиле

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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
|contactITName|String|Имя пользователя или организации, ответственных за ИТ-поддержку|
|contactITPhoneNumber|String|Номер телефона пользователя или организации, ответственного за ИТ-поддержку|
|contactITEmailAddress|String|Адрес электронной почты пользователя или организации, ответственных за ИТ-поддержку|
|contactITNotes|String|Текстовые комментарии о лице или организации, ответственных за ИТ-поддержку|
|privacyUrl|String|URL-адрес политики конфиденциальности компании или Организации|
|onlineSupportSiteUrl|String|URL-адрес сайта ИТ-службы технической поддержки компании или Организации|
|onlineSupportSiteName|String|Отображаемое имя сайта ИТ-службы технической поддержки компании или Организации|
|themeColor|[rgbColor](../resources/intune-shared-rgbcolor.md)|Основной цвет темы, используемый в приложениях портала компании и на веб-портале|
|showLogo|Boolean|Логическое значение, указывающее, отображаются ли изображения логотипа, предоставленные администратором.|
|showDisplayNameNextToLogo|Boolean|Логическое значение, указывающее, будет ли отображаться отображаемое имя, предоставленное администратором, рядом с изображением логотипа.|
|семеколорлого|[mimeContent](../resources/intune-shared-mimecontent.md);|Изображение логотипа, отображаемое в приложениях корпоративного портала, у которых есть фоновый цвет темы позади логотипа|
|lightBackgroundLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|Изображение логотипа, отображаемое в приложениях корпоративного портала, у которых есть светлый фон позади логотипа|
|ландингпажекустомизедимаже|[mimeContent](../resources/intune-shared-mimecontent.md);|Настраиваемое изображение, отображаемое на начальной странице "приложения корпоративного портала"|
|кустомпривацимессаже|String|Текстовые комментарии относительно того, что у администратора есть доступ к устройству.|
|исремоведевицедисаблед|Boolean|Логическое значение, указывающее, отключил ли админсистратор действие "Remove Device" на корпоративных устройствах.|
|исфакториресетдисаблед|Boolean|Логическое значение, указывающее, отключил ли админсистратор действие "Фабричная сброс" на корпоративных устройствах.|

## <a name="relationships"></a>Отношения
|Отношение|Тип|Описание|
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
  "contactITName": "String",
  "contactITPhoneNumber": "String",
  "contactITEmailAddress": "String",
  "contactITNotes": "String",
  "privacyUrl": "String",
  "onlineSupportSiteUrl": "String",
  "onlineSupportSiteName": "String",
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
  "customPrivacyMessage": "String",
  "isRemoveDeviceDisabled": true,
  "isFactoryResetDisabled": true
}
```



