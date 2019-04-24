---
title: 'driveItem: Preview'
description: Это действие позволяет получать кратковременно недопустимые URL-адреса для встраиваемых элементов, чтобы отобразить временный предварительный просмотр.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5a49a05e1e01616bc9bbbb713fd05805d9af3070
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454372"
---
# <a name="driveitem-preview"></a>driveItem: Preview

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Это действие позволяет получать кратковременно недопустимые URL-адреса для встраиваемых элементов, чтобы отобразить временный предварительный просмотр.

Если вы хотите получить ссылки с большим сроком действия, используйте вместо этого API [CreateLink][] .

> **Примечание:** В настоящее время действие **Предварительный просмотр** доступно только в SharePoint и OneDrive для бизнеса.

[createLink]: driveitem-createlink.md

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий)
|:---------------------------------------|:-------------------------------------------
| Делегированные (рабочая или учебная учетная запись)     | Files. Read, Files. ReadWrite, Files. ReadWrite. ALL, sites. ReadWrite. ALL.
| Делегированное (личная учетная запись Майкрософт) | Files. Read, Files. ReadWrite, Files. ReadWrite. ALL
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
| Просмотр      | string        | Необязательно. Предварительная версия приложения для использования. `onedrive` или `office`. Если значение равно null, подходящее средство просмотра будет выбрано автоматически.
| не для Chrome  | boolean       | Необязательный параметр. Если `true` выбрано значение (по умолчанию), то Внедренное представление не будет содержать элементы управления.
| Алловедит   | boolean       | Необязательный параметр. Если `true`файл можно редактировать из встроенного пользовательского интерфейса.
| page        | строка или число | Необязательный атрибут. Номер страницы для начала документа, если это необходимо. Указывается как строка для будущих случаев использования для типов файлов, таких как ZIP.
| zoom        | number        | Необязательный атрибут. Масштаб (при необходимости) для запуска.

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
| Команда         | строка | URL-адрес, подходящие для внедрения с помощью HTTP GET (Iframes и т. д.)
| Постурл        | строка | URL-адрес, подходящий для внедрения с помощью HTTP POST (форма POST, JS и т. д.)
| Параметры | строка | Параметры POST для включения при использовании Постурл

В зависимости от текущего состояния поддержки внедрения для заданных параметров может возвращаться либо getUrl, Постурл, либо и то, и другое.

i-параметры — это строка, `application/x-www-form-urlencoded`отформатированная как, и при выполнении POST для постурл Content-Type необходимо задать соответствующие параметры. Пример:
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="viewers"></a>Наблюдател

Для параметра **средства просмотра** разрешены следующие значения.

| Значение типа | Описание
|:-----------|:----------------------------------------------------------------
| определен     | Выбирает соответствующее приложение для отображения файла. В большинстве случаев будет использоваться `onedrive` предварительный просмотр, но он может варьироваться в зависимости от типа файла.
| `onedrive` | Использование приложения предварительного просмотра OneDrive для отображения файла.
| `office`   | Используйте WAC (Office Online) для отображения файла. Допускается только для документов Office.

### <a name="chrome-vs-chromeless"></a>Хром VS Chrome

Если `chromeless` этот параметр имеет значение true, предварительный просмотр будет иметь исходное представление файла.
В противном случае для взаимодействия с документом или представлением могут отображаться дополнительные панели инструментов и кнопки.

### <a name="viewedit"></a>Просмотр и редактирование

Если `allowEdit` имеет значение true, документ можно изменить с помощью встроенной предварительной версии.
Эта возможность может быть недоступна для предварительных версий приложений и типов файлов.

### <a name="pagezoom"></a>Страница/масштаб

Параметры `page` и `zoom` могут быть недоступны для всех предварительных версий приложений, но будут применены, если это приложение поддерживает приложение предварительного просмотра.
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-preview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
