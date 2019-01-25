---
title: 'driveItem: предварительный просмотр'
description: Это действие позволяет получать кратковременного встраиваемые URL-адреса для элемента для визуализации временные предварительного просмотра.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5a49a05e1e01616bc9bbbb713fd05805d9af3070
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508540"
---
# <a name="driveitem-preview"></a>driveItem: предварительный просмотр

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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

## <a name="request-body"></a>Текст запроса

Текст запроса определяет свойства встраиваемые URL-адреса, запрашивающего приложения.
Запрос должен быть объектом JSON с указанными ниже свойствами.

|   Имя      |  Тип         | Описание
|:------------|:--------------|:-----------------------------------------------
| Средство просмотра      | string        | Необязательный параметр. Предварительная версия приложения для использования. `onedrive` или `office`. Если значение null, подходящее средство просмотра выбирается автоматически.
| chromeless  | boolean       | Необязательный параметр. Если `true` (по умолчанию), внедренное представление не будет содержать все элементы управления.
| AllowEdit   | boolean       | Необязательный параметр. Если `true`, файл можно редактировать в пользовательском Интерфейсе внедренных.
| page        | Строка или номер | Необязательный параметр. Номер документа для запуска, если это возможно. Указан как строка для использования в будущем случаев вокруг типов файлов, например ZIP.
| zoom        | число        | Необязательный параметр. Выбор масштаба для запуска, если это возможно.

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
| getUrl         | string | URL-адрес для внедрения с помощью HTTP GET (Интернет-кадров, и т.д.)
| postUrl        | string | URL-адрес для внедрения с помощью HTTP POST (отправки формы, JS, и т.д.)
| postParameters | string | Параметры отправки для включения при использовании postUrl

В зависимости от текущего состояния внедрить поддержку указанные параметры могут возвращаться getUrl, postUrl или оба.

postParameters — это строка в формате `application/x-www-form-urlencoded`, и, если для выполнения ОТПРАВКУ postUrl типа контента необходимо задать соответствующим образом. Пример:
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="viewers"></a>Средства просмотра

Для **просмотра** параметров могут следующие значения.

| Значение типа | Описание
|:-----------|:----------------------------------------------------------------
| Null     | Выбирает соответствующие приложения для отображения файла. В большинстве случаев это будет использовать `onedrive` средство просмотра, но могут в зависимости от типа файла.
| `onedrive` | Использование приложения просмотра OneDrive для отображения файла.
| `office`   | Используйте WAC (Office online) для отображения файла. Поддерживается только при работе с документами Office.

### <a name="chrome-vs-chromeless"></a>Chromeless хрома vs

Если `chromeless` имеет значение true, предварительный просмотр будет исходного состояния отображения файла.
В противном случае может быть дополнительные панели инструментов и кнопок, отображаемых для взаимодействия с документов и представлений.

### <a name="viewedit"></a>Просмотр и изменение

Если `allowEdit` имеет значение true, документ можно изменить взаимодействия с пользователем с внедренным предварительного просмотра.
Эта возможность не могут быть доступны для всех приложений предварительного просмотра или типов файлов.

### <a name="pagezoom"></a>Масштаб страницы /

`page` И `zoom` параметры могут быть недоступны для всех приложений предварительного просмотра, но будет применяться, если версия приложения поддерживает его.
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-preview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
