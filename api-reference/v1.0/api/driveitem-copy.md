---
author: JeremyKelley
title: 'driveItem: скопируйте'
ms.localizationpriority: medium
ms.prod: sharepoint
description: Асинхронно создает копию элемента driveItem (включая все дочерние элементы) в новом родительском элементе или с новым именем.
doc_type: apiPageType
ms.openlocfilehash: f5ec199fee10ca140f0fc9a067244a73660a3dee
ms.sourcegitcommit: 4c8444b732b8d6d0de8a95f6666c42095f146266
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/08/2022
ms.locfileid: "62443354"
---
# <a name="driveitem-copy"></a>driveItem: скопируйте

Пространство имен: microsoft.graph

Асинхронно создает копию элемента [driveItem][item-resource] (включая все дочерние элементы) в новом родительском элементе или с новым именем.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Files.ReadWrite, Files.ReadWrite.All    |
|Для приложений | Files.ReadWrite.All, Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/copy
POST /groups/{groupId}/drive/items/{itemId}/copy
POST /me/drive/items/{item-id}/copy
POST /sites/{siteId}/drive/items/{itemId}/copy
POST /users/{userId}/drive/items/{itemId}/copy
```

## <a name="optional-query-parameters"></a>Необязательные параметры запроса

Этот метод поддерживает параметр `@microsoft.graph.conflictBehavior` запроса для настройки поведения при конфликте.

| Значение           | Описание                                    |
|:----------------|:---------------------------------------------- |
| сбой            | По умолчанию необходимо сообщить о сбое.     |
| replace         | Переопиши существующий элемент на целевом сайте.    |
| rename          | Переименовать элемент.                               |

**Примечание:** _ConflictBehavior_ не поддерживается для OneDrive Consumer.

## <a name="request-body"></a>Текст запроса

В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.


| Имя            | Значение                                          | Описание                                                                                                 |
|:----------------|:-----------------------------------------------|:------------------------------------------------------------------------------------------------------------|
| parentReference | [ItemReference](../resources/itemreference.md) | Необязательный. Отсылает к родительскому элементу, в котором будет создана копия.                                         |
| name            | string                                         | Необязательный. Новое имя копии. Если оно не предоставлено, будет использовано такое же имя, как в оригинале.    |

**Примечание.** Элемент _parentReference_ должен включать параметры `driveId` и `id` для целевой папки.

## <a name="response"></a>Отклик

Возвращает сведения о том, как [отслеживать ход](/graph/long-running-actions-overview) копирования после принятия запроса.

## <a name="example"></a>Пример

В этом примере показано, как копировать файл с идентификатором `{item-id}` в папку с идентификатором `driveId` и значением `id`.
У новой копии файла будет имя `contoso plan (copy).txt`.


### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "copy-item", "scopes": "files.readwrite", "tags": "service.graph", "target": "action" } -->

```http
POST /me/drive/items/{item-id}/copy
Content-Type: application/json

{
  "parentReference": {
    "driveId": "6F7D00BF-FC4D-4E62-9769-6AEA81F3A21B",
    "id": "DCD0D3AD-8989-4F23-A5A2-2C086050513F"
  },
  "name": "contoso plan (copy).txt"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/copy-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/copy-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/copy-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/copy-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>Отклик

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 202 Accepted
Location: https://contoso.sharepoint.com/_api/v2.0/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

В значении заголовка `Location` имеется URL-адрес службы, которая возвращает сведения о текущем состоянии операции копирования.
Эти сведения можно использовать для [определения завершения копирования](/graph/long-running-actions-overview).

### <a name="remarks"></a>Замечания

Во многих случаях копирование выполняется асинхронно.
В ответе API будет указано только, что операция копирования была принята или отклонена; например, из-за имени файла назначения, уже используемом.

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
  ]
} -->

