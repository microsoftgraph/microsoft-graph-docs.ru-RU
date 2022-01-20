---
author: swapnil1993
title: Обновление contentType
description: Обновление типа контента.
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 78be26b9e0804565bc02f2f95e6964837bc96395
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62134097"
---
# <a name="update-contenttype"></a>Обновление contentType
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
Обновление [контента типа][контента.]
  

## <a name="permissions"></a>Разрешения

  

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

  

|Тип разрешения | Разрешения (в порядке повышения привилегий) |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Sites.Manage.All, Sites.FullControl.All |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Приложение |Sites.Manage.All, Sites.FullControl.All |

  

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
```http
PATCH /sites/{site-id}/contentTypes/{contentType-id}
PATCH /sites/{site-id}/lists/{list-id}/contentTypes/{contentType-id}
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

В теле запроса поставляем представление JSON ресурса [contentType][] для обновления.  

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект contentType][] в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_contenttype"
}
-->

```http
PATCH https://graph.microsoft.com/beta/sites/{site-id}/contentTypes/{contentType-id}
Content-Type: application/json

{
   "name":"updatedCt",
   "documentSet":{
      "shouldPrefixNameToFile":true,
      "allowedContentTypes":[
         {
            "id":"0x0101",
            "name":"Document"
         }
      ],
      "defaultContents":[
         {
            "fileName":"a.txt",
            "contentType":{
               "id":"0x0101"
            }
         },
         {
            "fileName":"b.txt",
            "contentType":{
               "id":"0x0101"
            }
         }
      ],
      "sharedColumns":[
         {
            "name":"Description",
            "id":"cbb92da4-fd46-4c7d-af6c-3128c2a5576e"
         },
         {
            "name":"Address",
            "id":"fc2e188e-ba91-48c9-9dd3-16431afddd50"
         }
      ],
      "welcomePageColumns":[
         {
            "name":"Address",
            "id":"fc2e188e-ba91-48c9-9dd3-16431afddd50"
         }
      ]
   }
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-contenttype-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-contenttype-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-contenttype-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-contenttype-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

<!-- { "blockType": "response", "@type": "microsoft.graph.contentType", "truncated": true} -->

  

```http
HTTP/1.1 200 OK
Content-type: application/json

{
   "id":"0x0101009B237E76EF94DC49B4E58139041E7C60",
   "description":"",
   "eTag":"\"7\"",
   "group":"Custom Content Types",
   "hidden":false,
   "name":"testdoc",
   "parentId":"0x0101",
   "base":{
      "id":"0x0101",
      "name":"Document"
   }
}
```

[contentType]: ../resources/contentType.md
