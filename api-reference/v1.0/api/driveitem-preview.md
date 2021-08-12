---
title: 'driveItem: предварительный просмотр'
description: Это действие позволяет получать кратковременные URL-адреса для элемента для отображения временного предварительного просмотра.
localization_priority: Normal
ms.prod: sharepoint
author: JeremyKelley
doc_type: apiPageType
ms.openlocfilehash: b8cac897e67bc0a997b9ea486b1f6956e70c2f07dfe7fe5019ab7285b3eb977c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54234318"
---
# <a name="driveitem-preview"></a>driveItem: предварительный просмотр

Пространство имен: microsoft.graph

Это действие позволяет получить кратковременный URL-адрес для элемента, чтобы отрисовывать временный предварительный просмотр.

Если вы хотите получить длительные встраивемые ссылки, вместо этого используйте [API createLink.][]

> **Примечание:** Действие **предварительного** просмотра в настоящее время доступно только SharePoint и OneDrive для бизнеса.

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

Тело запроса определяет свойства встраяемого URL-адреса, запрашиваемого вашим приложением.
Запрос должен быть объектом JSON с указанными ниже свойствами.

|   Имя      |  Тип         | Описание
|:------------|:--------------|:-----------------------------------------------
| page        | строка/номер | Необязательно. Номер страницы документа, с чего можно начать, если это применимо. Указана в качестве строки для будущих случаев использования в таких типах файлов, как ZIP.
| zoom        | number        | Необязательный параметр. Масштабирование уровня для начала, если применимо.

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
| getUrl         | Строка | URL-адрес, подходящий для встраивки с помощью HTTP GET (iframes и т.д.)
| postUrl        | Строка | URL-адрес, подходящий для встраивки с помощью HTTP POST (столб формы, JS и т.д.)
| postParameters | Строка | Параметры POST, которые необходимо включить при использовании postUrl

Либо getUrl, postUrl, либо оба могут быть возвращены в зависимости от текущего состояния встраив поддержку указанных параметров.

postParameters — это строка, отформатированная как, и при выполнении POST в postUrl тип контента должен быть задат `application/x-www-form-urlencoded` соответствующим образом. Например,
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="pagezoom"></a>Page/zoom

Параметры "page" и "zoom" могут быть недоступны для всех приложений предварительного просмотра, но будут применяться, если приложение предварительного просмотра поддерживает его.

