---
title: Регистрация governanceResource
description: Регистрация неуправляемого объекта governanceResource в PIM.
localization_priority: Normal
ms.openlocfilehash: f65c8b5884f08377967d3418bade0d5fc70c2063
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463952"
---
# <a name="register-governanceresource"></a>Регистрация governanceResource

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Регистрация неуправляемого объекта [governanceResource](../resources/governanceresource.md) в привилегированном управлении удостоверениями.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

>**Примечание:** Этот API также требует, чтобы у запрашивающего по крайней мере одно назначение активной роли для ресурса.

|Тип разрешения      | Разрешения              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Привилежедакцесс. ReadWrite. Азурересаурцес  |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Привилежедакцесс. ReadWrite. Азурересаурцес |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/resources/register
```

### <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод **** поддерживает `$select` `$expand` только [Параметры запроса OData](/graph/query-parameters) для настройки ответа.

### <a name="request-headers"></a>Заголовки запросов
| Имя      |Описание|
|:----------|:----------|
| Авторизация  | Bearer {code}|
| Content-Type  | application/json|

### <a name="request-body"></a>Текст запроса

|Параметры      |Тип                 |Обязательный |Описание|
|:-------------|:----------------------|:--------|:----------|
|externalId    |String                 |✓        |Екстерналид ресурса, регистрируемого в PIM.|

### <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `200 OK` отклик.

### <a name="example"></a>Пример
В этом примере показано, как зарегистрировать подписку Azure Wingtip Toys — произ.
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
##### <a name="request"></a>Запрос
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/register
```
##### <a name="response"></a>Отклик
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
  "suppressions": [
    "Error: /api-reference/beta/api/governanceresource-register.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
