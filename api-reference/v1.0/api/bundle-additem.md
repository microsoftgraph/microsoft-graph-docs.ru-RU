---
author: JeremyKelley
title: Добавление элемента в пакет
description: Добавьте элемент в пакет driveItems.
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 88b8e8c5e93d746522979f4086adeae5d5212e00
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/22/2022
ms.locfileid: "63724258"
---
# <a name="add-item-to-a-bundle"></a>Добавление элемента в пакет

Пространство имен: microsoft.graph

Добавьте дополнительный [driveItem][] из диска в [пакет][].

[bundle]: ../resources/bundle.md
[driveItem]: ../resources/driveItem.md

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Не поддерживается.                             |
|Делегированные (личная учетная запись Майкрософт) | Files.ReadWrite, Files.ReadWrite.All   |
|Для приложений          | Не поддерживается.                                           |

## <a name="http-request"></a>HTTP-запрос

```http
POST /drive/bundles/{bundle-id}/children
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание  |
|:------------- |:------------ |
| Авторизация | Bearer {token}. Обязательный. |
| Content-Type  | application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

В теле запроса поставляем JSON-представление [объекта driveItem][] .

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `204 No Content`.

Сведения об ответах на ошибки см. в Graph ответы на ошибки [и типы ресурсов][error-response].

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

Ниже приводится пример запроса, который добавляет существующий элемент в указанный пакет.

<!-- {"blockType": "request", "name": "add-to-bundle", "isCollection": true, "@odata.type": "microsoft.graph.driveItem", "tags": "onedrive.only" } -->

```http
POST https://graph.microsoft.com/v1.0/drive/bundles/{bundle-id}/children
Content-Type: application/json

{
  "id": "123456!87"
}
```

### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Add items to an existing bundle.",
  "keywords": "",
  "section&quot;: &quot;documentation"
} -->


