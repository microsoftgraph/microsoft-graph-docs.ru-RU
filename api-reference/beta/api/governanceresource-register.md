---
title: 'governanceResource: Register'
description: Регистрация объекта governanceResource в PIM.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2b8457f7ddee4564ca6b6b300121ddb7b8247e34
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713921"
---
# <a name="governanceresource-register"></a>governanceResource: Register

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Зарегистрируйте объект [governanceResource](../resources/governanceresource.md) в привилегированном управлении удостоверениями.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

>**Примечание:** Этот API также требует, чтобы у запрашивающего по крайней мере одно назначение активной роли для ресурса.

| Тип разрешения | Разрешения |
|:--------------- |:----------- |
| Делегированные (рабочая или учебная учетная запись) | Привилежедакцесс. ReadWrite. Азурересаурцес |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/resources/register
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод **** поддерживает `$select` `$expand` только [Параметры запроса OData](/graph/query-parameters) для настройки ответа.

## <a name="request-headers"></a>Заголовки запросов

| Имя | Описание |
|:---- |:----------- |
| Авторизация | Bearer {token} |
| Content-Type | application/json |

## <a name="request-body"></a>Тело запроса

| Свойства | Тип | Описание |
|:---------- |:---- |:----------- |
| externalId | String | Внешний идентификатор ресурса, регистрируемого в PIM. При регистрации подписки идентификатором является идентификатор подписки, добавленный в начале `/subscriptions/`. Например, `/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac`. |

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `200 OK` отклик.

## <a name="example"></a>Пример

В приведенном ниже примере показано, как вызывать этот API.
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
### <a name="request"></a>Запрос
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/register
Content-type: application/json

{
  "externalId": "/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac"
}
```
### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceResource"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Register governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
