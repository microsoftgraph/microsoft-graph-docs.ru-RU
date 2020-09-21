---
title: 'driveItem: Preview'
description: Это действие позволяет получать кратковременно недопустимые URL-адреса для встраиваемых элементов, чтобы отобразить временный предварительный просмотр.
localization_priority: Normal
ms.prod: sharepoint
author: JeremyKelley
doc_type: apiPageType
ms.openlocfilehash: 5fea16ce14e2df4b87ddc2b3f9246dfe758ec5b1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48073266"
---
# <a name="driveitem-preview"></a>driveItem: Preview

Пространство имен: microsoft.graph

Это действие позволяет получить короткий URL-адрес, который можно внедрить для элемента, чтобы отобразить временный предварительный просмотр.

Если вы хотите получить ссылки с большим сроком действия, используйте вместо этого API [CreateLink][] .

> **Примечание:** В настоящее время действие **Предварительный просмотр** доступно только в SharePoint и OneDrive для бизнеса.

[createLink]: driveitem-createlink.md

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий)
|:---------------------------------------|:-------------------------------------------
| Делегированные (рабочая или учебная учетная запись)     | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.
| Для приложений                            | Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All

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

## <a name="request-body"></a>Текст запроса

В теле запроса определяются свойства внедряемого URL-адреса, запрашиваемого приложением.
Запрос должен быть объектом JSON с указанными ниже свойствами.

|   Имя      |  Тип         | Описание
|:------------|:--------------|:-----------------------------------------------
| page        | строка или число | Необязательное. Номер страницы для начала документа, если это необходимо. Указывается как строка для будущих случаев использования для типов файлов, таких как ZIP.
| zoom        | number        | Необязательный параметр. Масштаб (при необходимости) для запуска.

## <a name="response"></a>Отклик

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

Ответом будет объект JSON, содержащий следующие свойства:

| Имя           | Тип   | Описание
|:---------------|:-------|:---------------------------------------------------
| Команда         | string | URL-адрес, подходящие для внедрения с помощью HTTP GET (Iframes и т. д.)
| постурл        | string | URL-адрес, подходящий для внедрения с помощью HTTP POST (форма POST, JS и т. д.)
| Параметры | string | Параметры POST для включения при использовании Постурл

В зависимости от текущего состояния поддержки внедрения для заданных параметров может возвращаться либо getUrl, Постурл, либо и то, и другое.

i-параметры — это строка, отформатированная как `application/x-www-form-urlencoded` , и при выполнении POST для постурл Content-Type необходимо задать соответствующие параметры. Пример.
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="pagezoom"></a>Страница/масштаб

Параметры "Page" и "Zoom" могут быть недоступны для всех предварительных приложений, но будут применены, если это приложение поддерживает приложение Preview.

