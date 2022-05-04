---
title: 'contentType: getCompatibleHubContentTypes'
description: Получение списка совместимых типов контента из центра типов контента, которые можно добавить на целевой сайт или в список.
author: swapnil1993
ms.localizationpriority: medium
ms.prod: sites-and-lists
doc_type: apiPageType
ms.openlocfilehash: 1d0f5d421e1f1f68298c555c8e7dad9dd81f294f
ms.sourcegitcommit: 089669703041900c4700c5d4f383ed05a7f193f8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/04/2022
ms.locfileid: "65191891"
---
# <a name="contenttype-getcompatiblehubcontenttypes"></a>contentType: getCompatibleHubContentTypes
Пространство имен: microsoft.graph

Получение списка совместимых типов контента из центра типов контента, которые можно добавить на целевой [сайт](../resources/site.md) или [в список](../resources/list.md).

Этот метод является частью изменений в типе публикации контента, чтобы оптимизировать синхронизацию опубликованных типов контента с сайтами и списками, эффективно переходя от "принудительного везде" к "извлечению по мере необходимости". Этот метод позволяет пользователям извлекать типы контента непосредственно из центра типов контента на сайт или в список. Дополнительные сведения см. в [разделе contentType: addCopyFromContentTypeHub](contenttype-addcopyfromcontenttypehub.md) и записи блога о обновлениях [продукта Syntex — август 2021 г](https://techcommunity.microsoft.com/t5/sharepoint-syntex-blog/syntex-product-updates-august-2021/ba-p/2606438).

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись) | Sites.Manage.All, Sites.FullControl.All |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Приложение | Sites.Manage.All, Sites.FullControl.All |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /sites/{siteId}/lists/{listId}/contentTypes/getCompatibleHubContentTypes
GET /sites/{siteId}/contentTypes/getCompatibleHubContentTypes
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ

В случае успешного выполнения эта функция возвращает код `200 OK` отклика и коллекцию объектов [contentType](../resources/contenttype.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "contenttype_getcompatiblehubcontenttypes"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/sites/root/lists/Documents/contentTypes/getCompatibleHubContentTypes
```

### <a name="response"></a>Отклик

Ниже приведен пример отклика.

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contentType",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.contentType",
      "id": "0x0101",
      "description": "Document content type",
      "group": "Document Content Types",
      "hidden": false,
      "isBuiltIn": true,
      "name": "Document"
    }
  ]
}
```

