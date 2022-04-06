---
title: Get governanceResource
description: Извлечение свойств и связей объекта governanceResource.
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: governance
author: japere
ms.openlocfilehash: 7670a7a2fb157d6c9dcf752f54d673c8604ed067
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2022
ms.locfileid: "64510508"
---
# <a name="get-governanceresource"></a>Get governanceResource

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v2ResourceRoles-deprecation](../../includes/pim-v2ResourceRoles-deprecation.md)]

Извлечение свойств и связей объекта [governanceResource](../resources/governanceresource.md) .

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference#privileged-access-permissions).

### <a name="azure-resources"></a>Ресурсы Azure

| Тип разрешения | Разрешения |
|:--------------- |:----------- |
| Делегированное (рабочая или учебная учетная запись) | PrivilegedAccess.ReadWrite.AzureResources |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Приложение | PrivilegedAccess.Read.AzureResources |

### <a name="azure-ad"></a>Azure AD

| Тип разрешения | Разрешения |
|:--------------- |:----------- |
| Делегированное (рабочая или учебная учетная запись) | PrivilegedAccess.ReadWrite.AzureAD |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Приложение | PrivilegedAccess.Read.AzureAD |

### <a name="groups"></a>Группы

|Тип разрешения | Разрешения |
|:-------------- |:----------- |
| Делегированное (рабочая или учебная учетная запись) | PrivilegedAccess.ReadWrite.AzureADGroup |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Приложение | PrivilegedAccess.Read.AzureADGroup |

Помимо области разрешений этот API требует, чтобы у запросителя было как минимум одно назначение ролей на ресурсе.

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{id}
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод **поддерживает** только параметры  `$select` `$expand` [запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ.

## <a name="request-headers"></a>Заголовки запросов
| Имя      |Описание|
|:----------|:----------|
| Авторизация  | Bearer {code}|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.
## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код `200 OK` отклика и [объект governanceResource](../resources/governanceresource.md) в тексте ответа.

## <a name="example"></a>Пример
В этом примере показано, как получить сведения о подписке Wingtip Toys - Prod (e5e7d29d-5465-45ac-885f-4716a5ee74b5).
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
##### <a name="request"></a>Запрос
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5
```
##### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceResource"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-Length: 459

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceResources/$entity",
    "id": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d",
    "type": "subscription",
    "displayName": "Wingtip Toys - Prod",
    "status": "Active",
    "registeredDateTime": "2018-04-05T22:30:37.13Z",
    "registeredRoot": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d",    
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


