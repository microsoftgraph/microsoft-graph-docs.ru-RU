---
title: 'driveItem: Preview'
description: Это действие позволяет получать кратковременно недопустимые URL-адреса для встраиваемых элементов, чтобы отобразить временный предварительный просмотр.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: ae5140bf6164aedd051f04c2c43c361f16517e7a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572705"
---
# <a name="driveitem-preview"></a>driveItem: Preview

Это действие позволяет получать кратковременно недопустимые URL-адреса для встраиваемых элементов, чтобы отобразить временный предварительный просмотр.

Если вы хотите получить ссылки с большим сроком действия, используйте вместо этого API [CreateLink][] .

> **Примечание:** В настоящее время действие **Предварительный просмотр** доступно только в SharePoint и OneDrive для бизнеса.

[createLink]: driveitem-createlink.md

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий)
|:---------------------------------------|:-------------------------------------------
| Делегированные (рабочая или учебная учетная запись)     | Files. Read, Files. ReadWrite, Files. ReadWrite. ALL, sites. ReadWrite. ALL.
| Делегированные (личная учетная запись Майкрософт) | Files. Read, Files. ReadWrite, Files. ReadWrite. ALL
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

## <a name="request-body"></a>Текст запроса

В теле запроса определяются свойства внедряемого URL-адреса, запрашиваемого приложением.
Запрос должен быть объектом JSON с указанными ниже свойствами.

|   Имя      |  Тип         | Описание
|:------------|:--------------|:-----------------------------------------------
| page        | строка или число | Необязательный параметр. Номер страницы для начала документа, если это необходимо. Указывается как строка для будущих случаев использования для типов файлов, таких как ZIP.
| zoom        | number        | Необязательный параметр. Масштаб (при необходимости) для запуска.

## <a name="response"></a>Ответ

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
| Постурл        | string | URL-адрес, подходящий для внедрения с помощью HTTP POST (форма POST, JS и т. д.)
| Параметры | string | Параметры POST для включения при использовании Постурл

В зависимости от текущего состояния поддержки внедрения для заданных параметров может возвращаться либо getUrl, Постурл, либо и то, и другое.

i-параметры — это строка, `application/x-www-form-urlencoded`отформатированная как, и при выполнении POST для постурл Content-Type необходимо задать соответствующие параметры. Примеры:
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="pagezoom"></a>Страница/масштаб

Параметры "Page" и "Zoom" могут быть недоступны для всех предварительных приложений, но будут применены, если это приложение поддерживает приложение Preview.
