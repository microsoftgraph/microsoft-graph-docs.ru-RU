---
author: swapnil1993
title: 'contentType: copyToDefaultContentLocation'
description: Скопируйте файл в расположение контента по умолчанию в типе контента.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 913db69991d176d8537baef5abbbb8734d6c10cc
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447290"
---
# <a name="contenttype-copytodefaultcontentlocation"></a>contentType: copyToDefaultContentLocation
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
Скопируйте файл в расположение контента по умолчанию в [типе контента.][contentType] Затем файл может быть добавлен в качестве файла или шаблона по умолчанию с помощью операции POST.

## <a name="permissions"></a>Разрешения  

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions_reference.md).

  

|Тип разрешения | Разрешения (в порядке повышения привилегий) |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All  |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Приложение | Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All |

  

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->

```http

POST /sites/id/contentTypes/id/copyToDefaultContentLocation 
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
|sourceFile| [itemReference](../resources/itemreference.md) |Метаданные о исходных файлах, которые необходимо скопировать в расположение контента по умолчанию. Обязательный.|
|destinationFileName| string |Имя файла назначения. 

## <a name="response"></a>Отклик


В случае успешного ответа этот вызов возвращает `204 No Content` ответ.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "contenttype_copytodefaultcontentlocation"
}
-->
```http
POST https://graph.microsoft.com/beta/sites/{id}/contentTypes/{contentTypeId}/copyToDefaultContentLocation 
Content-Type: application/json

{
    "sourceFile": {
        "sharepointIds": {
            "listId": "e2ecf63b-b0fd-48f7-a54a-d8c15479e3b0",
            "listItemId": "2"
        }
    },
    "destinationFileName": "newname.txt"
}
```



### <a name="response"></a>Отклик


<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content

```

  

[contentType]: ../resources/contentType.md
