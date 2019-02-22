---
title: Тип ресурса intuneBrand
description: Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложения "Корпоративный портал" и веб-портала пользователя.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e3e899f418ea9214530ac3b70e493a15655ca873
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167384"
---
# <a name="intunebrand-resource-type"></a>Тип ресурса intuneBrand

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложений "Корпоративный портал" и веб-портала пользователя.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Название компании или организации, которое отображается пользователям.|
|contactITName|String|Имя пользователя или название организации, ответственных за ИТ-поддержку.|
|contactITPhoneNumber|String|Номер телефона пользователя или организации, ответственных за ИТ-поддержку.|
|contactITEmailAddress|String|Адрес электронной почты пользователя или организации, ответственных за ИТ-поддержку.|
|contactITNotes|String|Текстовые комментарии в отношении пользователя или организации, ответственных за ИТ-поддержку.|
|privacyUrl|String|URL-адрес страницы с политикой конфиденциальности компании или организации.|
|onlineSupportSiteUrl|String|URL-адрес сайта ИТ-службы технической поддержки компании или организации.|
|onlineSupportSiteName|String|Отображаемое имя сайта ИТ-службы технической поддержки компании или организации.|
|themeColor|[rgbColor](../resources/intune-shared-rgbcolor.md)|Основной цвет темы, который используется в приложениях "Корпоративный портал" и на веб-портале.|
|showLogo|Логический|Логическое значение, которое определяет, отображаются ли предоставленные администратором изображения логотипов.|
|lightBackgroundLogo|[mimeContent](../resources/intune-shared-mimecontent.md);|Изображение с логотипом на светлом фоне, которое отображается в приложениях "Корпоративный портал".|
|darkBackgroundLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|Изображение с логотипом на темном фоне, которое отображается в приложениях "Корпоративный портал".|
|showNameNextToLogo|Boolean|Логическое значение, которое определяет, отображается ли возле изображения логотипа указанное администратором отображаемое имя.|
|Ландингпажекустомизедимаже|[mimeContent](../resources/intune-shared-mimecontent.md);|Настраиваемое изображение, отображаемое на начальной странице приложения портала Компнай|
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
  "showDisplayNameNextToLogo": true
}
```




