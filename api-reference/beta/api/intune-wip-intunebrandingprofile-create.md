---
title: Создание Интунебрандингпрофиле
description: Создание нового объекта Интунебрандингпрофиле.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 01d487da88677db899aea4c2ec25c54d3ae3d1bc
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33898997"
---
# <a name="create-intunebrandingprofile"></a>Создание Интунебрандингпрофиле

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового объекта [интунебрандингпрофиле](../resources/intune-wip-intunebrandingprofile.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementApps.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intuneBrandingProfiles
```

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта Интунебрандингпрофиле в формате JSON.

В следующей таблице приведены свойства, необходимые при создании Интунебрандингпрофиле.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ профиля|
|имя_профиля|Строка|Имя профиля|
|Профиледескриптион|Строка|Описание профиля|
|Исдефаултпрофиле|Логический|Показывает, используется ли профиль по умолчанию.|
|createdDateTime|DateTimeOffset|При создании Брандингпрофиле.|
|lastModifiedDateTime|DateTimeOffset|При последнем изменении Брандингпрофиле.|
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
|showDisplayNameNextToLogo|Boolean|Логическое значение, которое определяет, отображается ли возле изображения логотипа указанное администратором отображаемое имя.|
|Семеколорлого|[mimeContent](../resources/intune-shared-mimecontent.md);|Изображение логотипа, отображаемое в приложениях корпоративного портала на фоновом фоне цвета темы.|
|lightBackgroundLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|Изображение логотипа, отображаемое в приложениях корпоративного портала на светлом фоне.|
|Ландингпажекустомизедимаже|[mimeContent](../resources/intune-shared-mimecontent.md);|Настраиваемое изображение, отображаемое на начальной странице "приложения корпоративного портала"|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [интунебрандингпрофиле](../resources/intune-wip-intunebrandingprofile.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles
Content-type: application/json
Content-length: 1205

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfile",
  "profileName": "Profile Name value",
  "profileDescription": "Profile Description value",
  "isDefaultProfile": true,
  "displayName": "Display Name value",
  "contactITName": "Contact ITName value",
  "contactITPhoneNumber": "Contact ITPhone Number value",
  "contactITEmailAddress": "Contact ITEmail Address value",
  "contactITNotes": "Contact ITNotes value",
  "privacyUrl": "https://example.com/privacyUrl/",
  "onlineSupportSiteUrl": "https://example.com/onlineSupportSiteUrl/",
  "onlineSupportSiteName": "Online Support Site Name value",
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
  }
}
```

### <a name="response"></a>Отклик
Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1377

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfile",
  "id": "fcd6136c-136c-fcd6-6c13-d6fc6c13d6fc",
  "profileName": "Profile Name value",
  "profileDescription": "Profile Description value",
  "isDefaultProfile": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "contactITName": "Contact ITName value",
  "contactITPhoneNumber": "Contact ITPhone Number value",
  "contactITEmailAddress": "Contact ITEmail Address value",
  "contactITNotes": "Contact ITNotes value",
  "privacyUrl": "https://example.com/privacyUrl/",
  "onlineSupportSiteUrl": "https://example.com/onlineSupportSiteUrl/",
  "onlineSupportSiteName": "Online Support Site Name value",
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
  }
}
```




