---
title: Тип ресурса Интунебрандингпрофиле
description: Эта сущность содержит данные, которые используются при настройке внешнего вида уровня клиента для приложений корпоративного портала и веб-портала конечных пользователей.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3eae52bbb19eaca46c74d275ae7da3d16050a50e
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31799918"
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
|[Действие назначения](../api/intune-wip-intunebrandingprofile-assign.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ профиля|
|имя_профиля|String|Имя профиля|
|Профиледескриптион|String|Описание профиля|
|Исдефаултпрофиле|Boolean|Показывает, используется ли профиль по умолчанию.|
|createdDateTime|DateTimeOffset|При создании Брандингпрофиле.|
|lastModifiedDateTime|DateTimeOffset|При последнем изменении Брандингпрофиле.|
|displayName|Строка|Название компании или организации, которое отображается пользователям.|
|contactITName|String|Имя пользователя или название организации, ответственных за ИТ-поддержку.|
|contactITPhoneNumber|String|Номер телефона пользователя или организации, ответственных за ИТ-поддержку.|
|contactITEmailAddress|String|Адрес электронной почты пользователя или организации, ответственных за ИТ-поддержку.|
|contactITNotes|String|Текстовые комментарии в отношении пользователя или организации, ответственных за ИТ-поддержку.|
|privacyUrl|String|URL-адрес страницы с политикой конфиденциальности компании или организации.|
|onlineSupportSiteUrl|String|URL-адрес сайта ИТ-службы технической поддержки компании или организации.|
|onlineSupportSiteName|String|Отображаемое имя сайта ИТ-службы технической поддержки компании или организации.|
|themeColor|[rgbColor](../resources/intune-shared-rgbcolor.md)|Основной цвет темы, который используется в приложениях "Корпоративный портал" и на веб-портале.|
|showLogo|Boolean|Логическое значение, которое определяет, отображаются ли предоставленные администратором изображения логотипов.|
|showDisplayNameNextToLogo|Boolean|Логическое значение, которое определяет, отображается ли возле изображения логотипа указанное администратором отображаемое имя.|
|Семеколорлого|[mimeContent](../resources/intune-shared-mimecontent.md)|Изображение логотипа, отображаемое в приложениях корпоративного портала на фоновом фоне цвета темы.|
|lightBackgroundLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|Изображение логотипа, отображаемое в приложениях корпоративного портала на светлом фоне.|
|Ландингпажекустомизедимаже|[mimeContent](../resources/intune-shared-mimecontent.md)|Настраиваемое изображение, отображаемое на начальной странице "приложения корпоративного портала"|

## <a name="relationships"></a>Связи
|Отношение|Тип|Описание|
|:---|:---|:---|
|assignments|Коллекция [интунебрандингпрофилеассигнмент](../resources/intune-wip-intunebrandingprofileassignment.md)|Список назначений групп для профиля фирменной символики.|

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
  }
}
```





