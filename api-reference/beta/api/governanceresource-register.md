---
title: 'governanceResource: регистрация'
description: Регистрация объекта governanceResource в PIM.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 363ee47fcded93062b325f3f58df14dfa4a3c625
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2021
ms.locfileid: "53350868"
---
# <a name="governanceresource-register"></a>governanceResource: регистрация

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Регистрация [объекта governanceResource](../resources/governanceresource.md) в управление привилегированными пользователями.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference#privileged-access-permissions).

>**Примечание:** Этот API также требует, чтобы у запрашиваемой стороны было по крайней мере одно назначение активной роли на ресурсе.

### <a name="azure-resources"></a>Ресурсы Azure

| Тип разрешения | Разрешения |
|:--------------- |:----------- |
| Делегированное (рабочая или учебная учетная запись) | PrivilegedAccess.ReadWrite.AzureResources |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений | Не поддерживается. |

### <a name="azure-ad"></a>Azure AD

| Тип разрешения | Разрешения |
|:--------------- |:----------- |
| Делегированное (рабочая или учебная учетная запись) | PrivilegedAccess.ReadWrite.AzureAD |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений | Не поддерживается. |

### <a name="groups"></a>Группы

|Тип разрешения | Разрешения |
|:-------------- |:----------- |
| Делегированное (рабочая или учебная учетная запись) | PrivilegedAccess.ReadWrite.AzureADGroup |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/resources/register
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод **поддерживает** только `$select` параметры `$expand` [запроса oData и OData,](/graph/query-parameters) чтобы помочь настроить ответ.

## <a name="request-headers"></a>Заголовки запросов

| Имя | Описание |
|:---- |:----------- |
| Authorization | Bearer {token} |
| Content-Type | application/json |

## <a name="request-body"></a>Текст запроса

| Свойства | Тип | Описание |
|:---------- |:---- |:----------- |
| externalId | String | Внешний идентификатор ресурса, который будет зарегистрирован в PIM. При регистрации подписки идентификатором является идентификатор подписки, предварительно заранее задверяющий `/subscriptions/` . Например, `/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac`. |

## <a name="response"></a>Ответ

В случае успешной работы этот метод возвращает `200 OK` ответ.

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


