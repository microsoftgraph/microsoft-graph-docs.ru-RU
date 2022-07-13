---
title: Получение externalIdentitiesPolicy
description: Чтение свойств и связей объекта externalIdentitiesPolicy на уровне клиента, который определяет, могут ли внешние пользователи покинуть клиент Azure AD с помощью элементов управления самообслуживания.
author: KuiGithui
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: dd7defc8cdbedf1d4d47120edd791bdda4fb829f
ms.sourcegitcommit: f99b4d365ba381f8f1997d3857ab43da03528924
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2022
ms.locfileid: "66768373"
---
# <a name="get-externalidentitiespolicy"></a>Получение externalIdentitiesPolicy
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Чтение свойств и связей объекта [externalIdentitiesPolicy](../resources/externalidentitiespolicy.md) на уровне клиента, который определяет, могут ли внешние пользователи покинуть клиент Azure AD с помощью элементов управления самообслуживания.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|Policy.Read.All, Policy.ReadWrite.ExternalIdentities|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|Policy.Read.All, Policy.ReadWrite.ExternalIdentities|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/externalIdentitiesPolicy
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод не поддерживает параметры запроса OData для настройки ответа. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код `200 OK` отклика и объект [externalIdentitiesPolicy](../resources/externalidentitiespolicy.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "get_externalidentitiespolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/externalIdentitiesPolicy
```


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalIdentitiesPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#policies/externalIdentitiesPolicy/$entity",
    "id": "externalIdentityPolicy",
    "deletedDateTime": null,
    "allowExternalIdentitiesToLeave": true,
    "allowDeletedIdentitiesDataRemoval": false,
    "displayName": "External Identities Policy"
  }
}
```

