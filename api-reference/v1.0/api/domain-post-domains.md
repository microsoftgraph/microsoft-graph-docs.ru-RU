---
title: Создание домена
description: Добавление домена в клиент.
author: adimitui
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 6583efd2d00e320bd268e1fad606bd6a30b7d0b6
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2021
ms.locfileid: "60940775"
---
# <a name="create-domain"></a>Создание домена

Пространство имен: microsoft.graph

Добавление домена в клиент.

**Важно!** Вам не удастся использовать сопоставленный домен с вашим клиентом Azure AD, пока не будет проверено владение доменом. Дополнительные сведения см. в статье [Перечисление verificationDnsRecords](domain-list-verificationdnsrecords.md). Для корневых доменов требуется проверка. Например, для домена contoso.com требуется проверка. Если корневой домен проверен, то его дочерние домены будут автоматически считаться проверенными. Например, если домен contoso.com проверен, то его дочерний домен subdomain.contoso.com будет автоматически считаться проверенным.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).


|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Domain.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Domain.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->
```http
POST /domains
```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Описание|
|:---------------|:----------|
| Авторизация  | Bearer {token}. Обязательный.|
| Content-Type  | application/json |

## <a name="request-body"></a>Текст запроса
В теле запроса укажите представление JSON объекта [domain](../resources/domain.md).

> Тело запроса содержит свойство id для нового домена. id — это единственное свойство, которое можно указать, и оно является обязательным. Значение свойства id — полное доменное имя, которое необходимо создать.

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [domain](../resources/domain.md) в теле отклика.

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос

В теле запроса укажите представление JSON объекта [domain](../resources/domain.md).

<!-- {
  "blockType": "request",
  "id": "create_domain_from_domains"
}-->
```http
POST https://graph.microsoft.com/v1.0/domains
Content-type: application/json

{
  "id": "contoso.com"
}
```

##### <a name="response"></a>Отклик
Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "authenticationType": "authenticationType-value",
  "availabilityStatus": "availabilityStatus-value",
  "id": "contoso.com",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

