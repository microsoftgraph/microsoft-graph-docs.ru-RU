---
title: 'directoryObject: getByIds'
description: Возвращает объекты каталогов, указанные в списке идентификаторов.
author: keylimesoda
ms.localizationpriority: high
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 1872f70a4f8d94ad5f0c7b7fe7c6cecbf31dbcfa
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "60979305"
---
# <a name="directoryobject-getbyids"></a>directoryObject: getByIds

Пространство имен: microsoft.graph

Возвращение объектов каталогов, указанных в списке идентификаторов.

>[!NOTE]
>У этого API есть [известная проблема](/graph/known-issues#incomplete-objects-when-using-getbyids-request). Не все возвращаемые объекты каталогов представляют собой полные объекты, содержащие все свойства.

Ниже перечислены некоторые распространенные случаи использования этой функции.

* Разрешение идентификаторов, возвращаемых как часть коллекций идентификаторов функциями, например [getMemberObjects](directoryobject-getmemberobjects.md) или [getMemberGroups](directoryobject-getmembergroups.md), в базовые объекты каталогов.
* Разрешение идентификаторов, которые приложение хранит во внешнем хранилище, в базовые объекты каталогов.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).


|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Directory.Read.All, Directory.AccessAsUser.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Directory.Read.All |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getByIds
```

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Описание|
|:---------------|:--------|
| Авторизация  | Bearer {token}. Обязательный. |
| Content-Type  | application/json. Обязательный.  |

## <a name="request-body"></a>Текст запроса

В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр   | Тип |Описание|
|:---------------|:--------|:----------|
|ids|Коллекция String| Коллекция идентификаторов, для которой необходимо возвратить объекты. Идентификаторы имеют формат GUID и представлены в виде строк. Вы можете указать до 1000 идентификаторов. |
|types|Коллекция объектов string| Коллекция типов ресурсов, указывающая набор коллекций ресурсов, в котором необходимо выполнить поиск. Если аргумент не указан, по умолчанию используется объект [directoryObject](../resources/directoryobject.md), который содержит все типы ресурсов, определенные в каталоге. В коллекции можно указать любой объект, производный от [directoryObject](../resources/directoryobject.md). Пример: объекты [user](../resources/user.md), [group](../resources/group.md) и [device](../resources/device.md). <br/><br/>Для поиска ссылок на партнерскую организацию, [поставляющую облачные решения](https://partner.microsoft.com/cloud-solution-provider), укажите [directoryObjectPartnerReference](../resources/directoryobjectpartnerreference.md). Если аргумент не указан, по умолчанию используется объект [directoryObject](../resources/directoryobject.md), который содержит все типы ресурсов, определенные в каталоге, кроме ссылок на партнерскую организацию, [поставляющую облачные решения](https://partner.microsoft.com/cloud-solution-provider).</br><br/> В значениях не учитывается регистр символов.|

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код ответа `200 OK` и объект коллекции строк в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_getById"
}-->

```http
POST https://graph.microsoft.com/v1.0/directoryObjects/getByIds
Content-type: application/json

{
    "ids":["84b80893874940a3-97b7-68513b600544","5d6059b6368d-45f8-91e18e07d485f1d0"],
    "types":["user"]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-getbyid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getbyid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-getbyid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-getbyid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/directoryobject-getbyid-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryObjects",
    "value": [
      {
        "@odata.type": "#microsoft.graph.user",
        "id": "84b80893-8749-40a3-97b7-68513b600544",
        "accountEnabled": true,
        "displayName": "Trevor Jones"
      },
      {
        "@odata.type": "#microsoft.graph.user",
        "id": "84b80893-8749-40a3-97b7-68513b600544",
        "accountEnabled": true,
        "displayName": "Billy Smith"
      }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getById",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

