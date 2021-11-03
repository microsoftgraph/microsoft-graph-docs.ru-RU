---
author: swapnil1993
title: Обновление столбцаDefinition
description: Обновление сайта, списка или столбца типа контента.
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: a0fbd27355e96c5e09651dbc16dde705f5f536e0
ms.sourcegitcommit: 64d27a0e3dcccc9d857e62aace4153e5d98fb3d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60729635"
---
# <a name="update-columndefinition"></a>Обновление столбцаDefinition
Пространство имен: microsoft.graph


Обновление [сайта,][] [списка][]или [типа контента.][contentType] [column][columnDefinition]
  

## <a name="permissions"></a>Разрешения  

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

  

|Тип разрешения | Разрешения (в порядке повышения привилегий) |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Sites.Manage.All, Sites.FullControl.All  |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Для приложений | Sites.Manage.All, Sites.FullControl.All |

  

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->

```http
PATCH /sites/{site-id}/columns/{column-id}
PATCH /sites/{site-id}/lists/{list-id}/columns/{column-id}
PATCH /sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}
PATCH /sites/{site-id}/lists/{list-id}/contentTypes/{contentType-id}/columns/{column-id}
```


## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|


## <a name="request-body"></a>Основной текст запроса

В теле запроса поставляем представление JSON этих свойств ресурса [columnDefinition][] для обновления. Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.

Для столбцов **в сайте** или списке **можно** обновить любое свойство **columnDefinition,** кроме **свойства id.**

Для столбцов **в contentType** можно обновить только **необходимое или** **скрытое** свойство.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и обновленный `200 OK` [объект columnDefinition][] в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

```http
PATCH /sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}
Content-Type: application/json

{
  "required": true,
  "hidden": false,
  "propagateChanges": false     
}
```

### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.columnDefinition"
}
-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "description": "",
  "displayName": "Custom Column",
  "enforceUniqueValues": false,
  "hidden": false,
  "id": "11dfef35-e2f7-4f17-82b0-6fba34445103",
  "indexed": false,
  "name": "Custom Column",
  "readOnly": false,
  "required": true,
  "text": {
    "allowMultipleLines": false,
    "appendChangesToExistingText": false,
    "linesForEditing": 0,
    "maxLength": 255
  }
}
```

  

[columnDefinition]: ../resources/columnDefinition.md
[contentType]: ../resources/contentType.md
[list]: ../resources/list.md
[site]: ../resources/site.md

