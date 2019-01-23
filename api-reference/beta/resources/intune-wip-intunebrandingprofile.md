---
title: Тип ресурса intuneBrandingProfile
description: Этот объект содержит данные, используемые в настройке уровня внешнего клиента приложения портала компании, а также веб-портала конечного пользователя.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b299964627a89598c28f15dfeed8ce6e13bede8c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411101"
---
# <a name="intunebrandingprofile-resource-type"></a>Тип ресурса intuneBrandingProfile

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Этот объект содержит данные, используемые в настройке уровня внешнего клиента приложения портала компании, а также веб-портала конечного пользователя.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список intuneBrandingProfiles](../api/intune-wip-intunebrandingprofile-list.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) коллекции|Свойства списка и связей объектов [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) .|
|[Получение intuneBrandingProfile](../api/intune-wip-intunebrandingprofile-get.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|Чтение свойства и связи объекта [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) .|
|[Создание intuneBrandingProfile](../api/intune-wip-intunebrandingprofile-create.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|Создание нового объекта [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) .|
|[Удаление intuneBrandingProfile](../api/intune-wip-intunebrandingprofile-delete.md)|Нет|Удаляет [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md).|
|[Обновление intuneBrandingProfile](../api/intune-wip-intunebrandingprofile-update.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|Обновление свойства объекта [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) .|
|[Действие assign](../api/intune-wip-intunebrandingprofile-assign.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Клавиша профилей|
|Имя_профиля|String|Имя профиля|
|profileDescription|String|Описание профиля|
|isDefaultProfile|Логический|Представляет при использовании профиля по умолчанию.|
|createdDateTime|DateTimeOffset|При создании BrandingProfile.|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения BrandingProfile.|
|displayName|String|Название компании или организации, которое отображается пользователям.|
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
|themeColorLogo|[mimeContent](../resources/intune-shared-mimecontent.md);|Изображения эмблемы, отображаемые в приложениях портала компании на темы цвет фона.|
|lightBackgroundLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|Изображения эмблемы, отображаемые в приложениях портала компании на светлый фон.|
|landingPageCustomizedImage|[mimeContent](../resources/intune-shared-mimecontent.md);|Настраиваемая изображение, отображаемое в приложениях портал "Компания" Главная страница|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) коллекции|Список назначений группы для фирменной настройки профиля.|

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




