---
title: Тип ресурса intuneBrand
description: Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложения "Корпоративный портал" и веб-портала пользователя.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6e4d005c4b5eccf0775e0a671088a5de09f95fe2
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940206"
---
# <a name="intunebrand-resource-type"></a>Тип ресурса intuneBrand

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложений "Корпоративный портал" и веб-портала пользователя.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Название компании или организации, которое отображается пользователям.|
|contactITName|Строка|Имя пользователя или название организации, ответственных за ИТ-поддержку.|
|contactITPhoneNumber|Строка|Номер телефона пользователя или организации, ответственных за ИТ-поддержку.|
|contactITEmailAddress|Строка|Адрес электронной почты пользователя или организации, ответственных за ИТ-поддержку.|
|contactITNotes|Строка|Текстовые комментарии в отношении пользователя или организации, ответственных за ИТ-поддержку.|
|privacyUrl|Строка|URL-адрес страницы с политикой конфиденциальности компании или организации.|
|onlineSupportSiteUrl|Строка|URL-адрес сайта ИТ-службы технической поддержки компании или организации.|
|onlineSupportSiteName|String|Отображаемое имя сайта ИТ-службы технической поддержки компании или организации.|
|themeColor|[rgbColor](../resources/intune-shared-rgbcolor.md)|Основной цвет темы, который используется в приложениях "Корпоративный портал" и на веб-портале.|
|showLogo|Логический|Логическое значение, которое определяет, отображаются ли предоставленные администратором изображения логотипов.|
|lightBackgroundLogo|[mimeContent](../resources/intune-shared-mimecontent.md);|Изображение с логотипом на светлом фоне, которое отображается в приложениях "Корпоративный портал".|
|darkBackgroundLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|Изображение с логотипом на темном фоне, которое отображается в приложениях "Корпоративный портал".|
|showNameNextToLogo|Boolean|Логическое значение, которое определяет, отображается ли возле изображения логотипа указанное администратором отображаемое имя.|
|Ландингпажекустомизедимаже|[mimeContent](../resources/intune-shared-mimecontent.md);|Настраиваемое изображение, отображаемое на начальной странице приложения корпоративного портала|
|Кустомпривацимессаже|Строка|Пользовательское сообщение о конфиденциальности.|
|showDisplayNameNextToLogo|Boolean|Логическое значение, которое определяет, отображается ли возле изображения логотипа указанное администратором отображаемое имя.|

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
  "customPrivacyMessage": "String",
  "showDisplayNameNextToLogo": true
}
```




