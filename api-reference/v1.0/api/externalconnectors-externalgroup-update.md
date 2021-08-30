---
title: Обновление externalGroup
description: Обновление свойств объекта externalGroup.
author: sacampbe-msft
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 52a818e5679d212a0afe1318c9125d1d8f88ffcd
ms.sourcegitcommit: 6efd9df497d795988cd85474f379d1989b0995b7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/30/2021
ms.locfileid: "58697555"
---
# <a name="update-externalgroup"></a>Обновление externalGroup
Пространство имен: microsoft.graph.externalConnectors



Обновление свойств объекта [externalGroup.](../resources/externalconnectors-externalgroup.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированное (рабочая или учебная учетная запись)     | Не поддерживается                               |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается                               |
| Для приложений                            | ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All             

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /connections/{connectionsId}/groups/{externalGroupId}
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание                 |
|:--------------|:----------------------------|
| Авторизация | Bearer {токен}. Обязательный.   |
| Content-Type  | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса
В теле запроса укажи значения для соответствующих свойств, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств. Для лучшей производительности не включаем свойства, которые не изменяются.

| Свойство    | Тип   | Описание                                                                                                              |
|:------------|:-------|:-------------------------------------------------------------------------------------------------------------------------|
| displayName | Строка | Дружеское имя внешней группы. Необязательный параметр.                                                                      |
| description | Строка | Описание внешней группы. Необязательный параметр.                                                                         |



## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "update_externalgroup"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/connections/{connectionsId}/groups/{externalGroupId}
Content-Type: application/json

{
  "displayName": "Contoso Marketing",
  "description": "The product marketing team"
}
```


### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
