---
author: JeremyKelley
title: Обновление пакета
description: Обновление пакета driveItems
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: b4925016b63569bba1915ce83100f59e647acc1e
ms.sourcegitcommit: f5382652b6880fab42040df40a08de7cb2d74d35
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/17/2022
ms.locfileid: "63561662"
---
# <a name="update-bundle"></a>Пакет обновления

Пространство имен: microsoft.graph

Обновление метаданных [для пакета][] [driveItemsdriveItem] [по] ID.
Можно обновить только следующие метаданные:

* Имя пакета
* Альбом `coverImageItemId` (если применимо)

Любые другие запросы на изменение будут игнорироваться.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Не поддерживается.                             |
|Делегированные (личная учетная запись Майкрософт) | Files.ReadWrite, Files.ReadWrite.All   |
|Для приложений          | Не поддерживается.                                           |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
PATCH /drive/items/{bundle-id}
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание  |
|:------------- |:------------ |
| Authorization | Носитель \{токен\}. Обязательный. |
| if-match      | eTag. Необязательное свойство. Если этот загон запроса включен, а предоставленный eTag не соответствует текущему eTag на койке, `412 Precondition Failed` возвращается ответ.

## <a name="request-body"></a>Текст запроса

В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.

## <a name="response"></a>Отклик

В случае успешного использования этот метод возвращает [ресурс driveItem][] , который представляет обновленный пакет в теле отклика.

Сведения об ответах на ошибки см. в этой [информации][error-response].

## <a name="example"></a>Пример

В этом примере переименовка пакета.

### <a name="request"></a>Запрос

<!-- { "blockType": "request", "name": "rename-bundle" } -->

```http
PATCH https://graph.microsoft.com/beta/drive/items/{bundle-id}
Content-Type: application/json

{
  "name": "Shared legal agreements"
}
```

### <a name="response"></a>Отклик

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "0123456789abc",
  "name": "Shared legal agreements",
  "bundle": {
    "childCount": 3
  }
}
```

Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.


[bundle]: ../resources/bundle.md
[driveItem]: ../resources/driveItem.md
[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Update or replace the contents or properties of a bundle.",
  "keywords": "update,replace,contents,bundle",
  "section": "documentation",
    "tocPath&quot;: &quot;Bundles/Update"
} -->


