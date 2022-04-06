---
author: JeremyKelley
title: Удаление пакета
description: Удаление пакета driveItems
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: b574c73db2f4e0dd71d0e2e5c6685b58f8ad8143
ms.sourcegitcommit: f5382652b6880fab42040df40a08de7cb2d74d35
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/17/2022
ms.locfileid: "63561667"
---
# <a name="delete-bundle"></a>Удаление пакета

Пространство имен: microsoft.graph

Удалите [пакет][] driveItems с помощью **его id**. Обратите внимание, что удаление пакета с помощью этого метода навсегда удаляет пакет и не перемещает его в корзину.
Однако он не удаляет элементы, на которые ссылается пакет.
Они останутся в родительских папках.

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
DELETE /drive/items/{bundle-id}
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание  |
|:------------- |:------------ |
| Authorization | Носитель \{токен\}. Обязательный. |
| if-match      | eTag. Необязательное свойство. Если этот загон запроса включен, а предоставленный eTag (или cTag) не соответствует текущему тегу в пакете, `412 Precondition Failed` возвращается ответ и пакет не удаляется.

## <a name="request-body"></a>Тело запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ

В случае успешного запроса этот вызов возвращает отклик `204 No Content`, указывающий, что ресурс удален, поэтому данные не возвращаются.

Сведения об ответах на ошибки см. в этой [информации][error-response].

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

<!-- { "blockType": "request", "name": "delete-bundle" } -->

```http
DELETE https://graph.microsoft.com/beta/drive/items/{bundle-id}
```

### <a name="response"></a>Отклик

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```


[bundle]: ../resources/bundle.md
[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Delete a bundle from OneDrive",
  "keywords": "delete,existing bundle,onedrive",
  "section": "documentation",
  "tocPath&quot;: &quot;Bundles/Delete"
} -->


