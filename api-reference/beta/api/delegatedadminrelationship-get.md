---
title: ДелегированиеAdminRelationship
description: Ознакомьтесь с свойствами объекта делегированияAdminRelationship.
author: adtangir
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 961223dffd108cbb0da063bde20286c2606fe3a9
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589918"
---
# <a name="get-delegatedadminrelationship"></a>ДелегированиеAdminRelationship
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ознакомьтесь с свойствами объекта [делегированияAdminRelationship](../resources/delegatedadminrelationship.md) .

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)| DelegatedAdminRelationship.Read.All, DelegatedAdminRelationship.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт)| Не поддерживается. |
|Для приложений| Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/delegatedAdminRelationships/{delegatedAdminRelationshipId}
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает параметр `$select` запроса OData для получения определенных свойств пользователей, включая те, которые не возвращаются по умолчанию.

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код `200 OK` ответа и объект [делегированияAdminRelationship](../resources/delegatedadminrelationship.md) в тексте ответа.

Объект **delegatedAdminRelationship** также содержит **свойство @odata.etag** по RFC2616.
 
## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "get_delegatedadminrelationship"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/delegatedAdminRelationships/5d027261-d21f-4aa9-b7db-7fa1f56fb163-8777b240-c6f0-4469-9e98-a3205431b836
```


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.delegatedAdminRelationship"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.delegatedAdminRelationship",
  "@odata.context": "https://graph.microsoft.com/beta/tenantRelationships/$metadata#delegatedAdminRelationships/$entity",
  "@odata.etag": "W/\"JyIxODAwZTY4My0wMDAwLTAyMDAtMDAwMC02MTU0OWFmMDAwMDAiJw==\"",
  "id": "5d027261-d21f-4aa9-b7db-7fa1f56fb163-8777b240-c6f0-4469-9e98-a3205431b836",
  "displayName": "Contoso admin relationship",
  "duration": "P730D",
  "customer": {
    "tenantId": "4fdbff88-9d6b-42e0-9713-45c922ba8001",
    "displayName": "Contoso Inc"
  },
  "accessDetails": {
    "unifiedRoles": [
      {
        "roleDefinitionId": "729827e3-9c14-49f7-bb1b-9608f156bbb8"
      },
      {
        "roleDefinitionId": "fe930be7-5e62-47db-91af-98c3a49a38b1"
      },
      {
        "roleDefinitionId": "e6d1a23a-da11-4be4-9570-befc86d067a7"
      }
    ]
  },
  "status": "active",
  "createdDateTime": "2022-02-10T11:24:42.3148266Z",
  "lastModifiedDateTime": "2022-02-10T11:26:44.9941884Z",
  "activatedDateTime": "2022-02-10T11:26:44.9941884Z",
  "endDateTime": "2024-02-10T11:24:42.3148266Z"
}
```

