---
title: Обновление tenantTag
description: Обновление свойств объекта tenantTag.
author: isaiahwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: fc3460209c4f6c8cb81663b75eb7d024999402c2
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2021
ms.locfileid: "60938750"
---
# <a name="update-tenanttag"></a>Обновление tenantTag
Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [tenantTag.](../resources/managedtenants-tenanttag.md)

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|ManagedTenants.WriteRead.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /tenantRelationships/managedTenants/tenantTags/{tenantTagId}
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В теле запроса укажи значения для соответствующих [полей tenantTag,](../resources/managedtenants-tenanttag.md) которые должны быть обновлены. Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств. Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.

Следующие свойства можно обновить:

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|displayName|String|Имя отображения тега клиента.|
|description|String|Описание тега клиента.|
|клиенты|[коллекция microsoft.graph.managedTenants.tenantInfo](../resources/managedtenants-tenantinfo.md)|Коллекция управляемых клиентов, связанных с тегом клиента.|

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и `200 OK` обновленный [объект tenantTag](../resources/managedtenants-tenanttag.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_tenanttag"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantTags/{tenantTagId}
Content-Type: application/json

{
  "displayName": "Onboarding",
  "description": "Tenants that we are currently onboarding"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tenanttag-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tenanttag-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tenanttag-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-tenanttag-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.tenantTag"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantTags/$entity",
  "id": "913391c0-5466-42b4-900d-0a7501399cb0",
  "displayName": "Onboarding",
  "description": "Tenants that we are currently onboarding",
  "tenantIds": [
    {
      "tenantId": "38227791-a88b-4fcc-81c5-58cf77668320"
    }
  ],
  "isDeleted": null,
  "createdDateTime": "2021-06-16T20:36:31.086644Z",
  "createdByUserId": "9bf6a5ad-aecb-4194-a16b-38e02702a602",
  "lastActionDateTime": "2021-07-11T18:54:44.5262828Z",
  "lastActionByUserId": "cad28f13-0158-43c5-9c59-952f2caa62c0"
}
```
