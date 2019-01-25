---
title: Получение объектов каталога из списка идентификаторов
description: Выберите "параметр запроса не поддерживается для этой операции.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7c76335889f336af6098eb00740085b40614c1ee
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512229"
---
# <a name="get-directory-objects-from-a-list-of-ids"></a>Получение объектов каталога из списка идентификаторов

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Возвращает объекты каталогов, указанные в списке идентификаторов.  ПРИМЕЧАНИЕ. Возвращаемые объекты каталогов представляют собой полные объекты, содержащие **все** свойства. Параметр запроса `$select` недоступен для этой операции.

Ниже перечислены некоторые распространенные случаи использования этой функции.

* Разрешение идентификаторов, возвращаемых как часть коллекций идентификаторов функциями, например [getMemberObjects](/graph/api/directoryobject-getmemberobjects.md?view=graph-rest-beta) или [getMemberGroups](/graph/api/directoryobject-getmembergroups.md?view=graph-rest-beta), в базовые объекты каталогов.
* Разрешение идентификаторов, которые приложение хранит во внешнем хранилище, в базовые объекты каталогов.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).


|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Directory.Read.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Directory.Read.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getByIds
```

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Тип | Описание|
|:---------------|:--------|:----------|
| Authorization  | string  | Bearer {токен}. Обязательный. |
| Content-Type  | application/json  |

## <a name="request-body"></a>Текст запроса

В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр   | Тип |Описание|
|:---------------|:--------|:----------|
|ids|Коллекция String| Коллекция идентификаторов, для которой необходимо возвратить объекты. Вы можете указать до 1000 идентификаторов. |
|types|Коллекция String| Коллекция типов ресурсов, определяющий набор ресурсов семейств сайтов для поиска. Если не указан, по умолчанию — [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta), которая содержит все типы ресурсов, определенные в каталоге. Любого объекта, производного от [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta) может быть указано в коллекции; Например: [пользователей](/graph/api/resources/user?view=graph-rest-beta), [группы](/graph/api/resources/group?view=graph-rest-beta), [устройства](/graph/api/resources/device?view=graph-rest-beta)и т. д. Для поиска справочных материалов, которые [Поставщик облаке решения](https://partner.microsoft.com/en-us/cloud-solution-provider) партнеров организации задается [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-beta). Если не указан, по умолчанию — [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta), которая содержит все типы ресурсов, определенные в каталоге, за исключением справочные материалы, которые [Поставщик решения облачных](https://partner.microsoft.com/en-us/cloud-solution-provider) партнерской организации. Значения не учитывают регистр.|

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "directoryobject_getByIds"
}-->

```http
POST https://graph.microsoft.com/beta/directoryObjects/getByIds
Content-type: application/json

{
    "ids":["84b80893-8749-40a3-97b7-68513b600544","5d6059b6-368d-45f8-91e1-8e07d485f1d0"],
    "types":["user"]
}
```

##### <a name="response"></a>Ответ

Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#directoryObjects",
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
<!--
{
  "type": "#page.annotation",
  "description": "directoryObject: getById",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directoryobject-getbyids.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
