---
title: 'driveItem: предварительный просмотр'
description: Это действие позволяет получать кратковременного встраиваемые URL-адреса для элемента для визуализации временные предварительного просмотра.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: ae5140bf6164aedd051f04c2c43c361f16517e7a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986077"
---
# <a name="driveitem-preview"></a>driveItem: предварительный просмотр

Это действие позволяет получать кратковременного встраиваемые URL-адреса для элемента для визуализации временные предварительного просмотра.

Если вы хотите получить длинные встраиваемые ссылки, используйте [команду createLink][] API.

> **Примечание:** Действие **предварительного просмотра** в данный момент доступна только на сервере SharePoint и OneDrive для бизнеса.

[команду createLink]: driveitem-createlink.md

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий)
|:---------------------------------------|:-------------------------------------------
| Делегированные (рабочая или учебная учетная запись)     | Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All
| Делегированные (личная учетная запись Майкрософт) | Files.Read, Files.ReadWrite, Files.ReadWrite.All
| Для приложений                            | Не поддерживается.

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/preview
POST /groups/{groupId}/drive/items/{itemId}/preview
POST /me/drive/items/{itemId}/preview
POST /sites/{siteId}/drive/items/{itemId}/preview
POST /users/{userId}/drive/items/{itemId}/preview
POST /shares/{shareId}/driveItem/preview
```

## <a name="request-body"></a>Тело запроса

Текст запроса определяет свойства встраиваемые URL-адреса, запрашивающего приложения.
Запрос должен быть объектом JSON с указанными ниже свойствами.

|   Имя      |  Тип         | Описание
|:------------|:--------------|:-----------------------------------------------
| page        | Строка или номер | Необязательное. Номер документа для запуска, если это возможно. Указан как строка для использования в будущем случаев вокруг типов файлов, например ZIP.
| zoom        | число        | Необязательное. Выбор масштаба для запуска, если это возможно.

## <a name="response"></a>Ответ

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

Ответ будет объект JSON, который содержит следующие свойства:

| Имя           | Тип   | Описание
|:---------------|:-------|:---------------------------------------------------
| getUrl         | строка | URL-адрес для внедрения с помощью HTTP GET (Интернет-кадров, и т.д.)
| postUrl        | строка | URL-адрес для внедрения с помощью HTTP POST (отправки формы, JS, и т.д.)
| postParameters | строка | Параметры отправки для включения при использовании postUrl

В зависимости от текущего состояния внедрить поддержку указанные параметры могут возвращаться getUrl, postUrl или оба.

postParameters — это строка в формате `application/x-www-form-urlencoded`, и, если для выполнения ОТПРАВКУ postUrl типа контента необходимо задать соответствующим образом. Примеры:
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="pagezoom"></a>Масштаб страницы /

«Страница» и «отобразить» параметры могут быть недоступны для всех приложений предварительного просмотра, но будет применяться, если версия приложения поддерживает его.
