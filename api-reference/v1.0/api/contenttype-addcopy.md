---
author: swapnil1993
title: 'contentType: addCopy'
description: Добавьте копию типа контента сайта в список.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 819e0c3bcf5455153d53eb8b84f423f99afebe67
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/30/2021
ms.locfileid: "58696720"
---
# <a name="contenttype-addcopy"></a>contentType: addCopy
Пространство имен: microsoft.graph


Добавьте копию контента [типа][контентаType] с сайта [в][site] [список][list].
 
  

## <a name="permissions"></a>Разрешения  

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions_reference.md).

  

|Тип разрешения | Разрешения (в порядке повышения привилегий) |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) |Sites.Manage.All, Sites.FullControl.All  |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Приложение | Sites.Manage.All, Sites.FullControl.All |

  

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
```http
POST /sites/{site-id}/lists/{list-id}/contentTypes/addCopy
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON параметров.

В следующей таблице указаны параметры, которые можно использовать с этим действием.

|Параметр|Тип|Описание|
|-|-|-|
|contentType| string | Канонический URL-адрес типа контента сайта, который будет скопирован в список. Обязательный.|

## <a name="response"></a>Отклик

В случае успешного ответа этот вызов возвращает код отклика и `201 Created` [объект contentType][] в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "contenttype_addcopy"
}
-->
```http
POST https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/contentTypes/addCopy
Content-Type: application/json

{
  "contentType": "https://graph.microsoft.com/v1.0/sites/{site-id}/contentTypes/0x0101"
}
```


### <a name="response"></a>Отклик


<!-- { "blockType": "response", "@type": "microsoft.graph.contentType", "truncated": true} -->

```http
HTTP/1.1 201 Created

{
    "id": "0x0101",
    "description": "Create a new custom CSR JavaScript Display Template.",
    "group": "Display Template Content Types",
    "hidden": false,
    "name": "JavaScript Display Template",
    "parentId": "0x01",
    "readOnly": false,
    "sealed": false,
    "base": {
        "id": "0x01",
        "description": "Create a new custom CSR JavaScript Display Template.",
        "group": "Display Template Content Types",
        "hidden": false,
        "name": "JavaScript Display Template",
        "readOnly": false,
        "sealed": false
    }
}
```

[site]: ../resources/site.md
[list]: ../resources/list.md
[contentType]: ../resources/contentType.md
