---
title: Регистрация governanceResource
description: Регистрация объекта неуправляемые governanceResource в PIM.
localization_priority: Normal
ms.openlocfilehash: ce439d53eb9f017340f561ca509e8da43dbafbfc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837753"
---
# <a name="register-governanceresource"></a>Регистрация governanceResource

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Регистрация объекта неуправляемые [governanceResource](../resources/governanceresource.md) в привилегированной управления удостоверениями.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

>**Примечание:** Этот интерфейс API также требуется наличие по крайней мере один назначения роли active источник запроса на ресурс.

|Тип разрешения      | Permissions              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | PrivilegedAccess.ReadWrite.AzureResources  |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | PrivilegedAccess.ReadWrite.AzureResources |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/resources/register
```

### <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод **только** поддерживает `$select` и `$expand` [Параметры запроса OData](/graph/query-parameters) для настройки ответа.

### <a name="request-headers"></a>Заголовки запросов
| Имя      |Описание|
|:----------|:----------|
| Authorization  | Bearer {code}|
| Content-Type  | application/json|

### <a name="request-body"></a>Тело запроса

|Параметры      |Тип                 |Обязательный |Описание|
|:-------------|:----------------------|:--------|:----------|
|externalId    |String                 |✓        |ExternalId ресурс, который должен быть зарегистрирован в PIM.|

### <a name="response"></a>Ответ
Успешно завершена, этот метод возвращает `200 OK` ответа.

### <a name="example"></a>Пример
В этом примере показано, как зарегистрировать подписка на Azure Wingtip Toys - производственного.
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
##### <a name="request"></a>Запрос
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/register
```
##### <a name="response"></a>Ответ
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
<!-- {
  "type": "#page.annotation",
  "description": "Register governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
