---
title: Список accessPackageResources
description: Извлечение списка объектов accesspackageresource.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 6948b7ca0d7c8b9b4c3d47221516cc4ea79d7992
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62091114"
---
# <a name="list-accesspackageresources"></a>Список accessPackageResources

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Извлечение списка [объектов accessPackageResource](../resources/accesspackageresource.md) в [accessPackageCatalog](../resources/accesspackagecatalog.md).  Чтобы попросить добавить или удалить [accessPackageResource,](../resources/accesspackageresource.md)используйте [создание accessPackageResourceRequest.](entitlementmanagement-post-accesspackageresourcerequests.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Приложение                            | EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{id}/accessPackageResources
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает параметры запросов OData для настройки ответа. Например, чтобы получить области и среды пакета доступа для каждого ресурса, включайте `$expand=accessPackageResourceScopes,accessPackageResourceEnvironment` в запрос. Чтобы получить доступные роли ресурса, включай `$expand=accessPackageResourceRoles` . Чтобы получить только ресурсы для приложений, а не групп или сайтов, включайте `$filter=resourceType eq 'Application'` запрос. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов

| Имя      |Описание|
|:----------|:----------|
| Авторизация | Носитель \{токен\}. Обязательный. |

## <a name="request-body"></a>Тело запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [accessPackageResource](../resources/accesspackageresource.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приводится пример запроса с помощью фильтра для выбора ресурсов определенного типа и возврата областей ресурсов `$expand` каждого ресурса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresources"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/{id}/accessPackageResources?$filter=resourceType eq 'Application'&$expand=accessPackageResourceScopes
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageresources-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageresources-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageresources-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageresources-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-accesspackageresources-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-accesspackageresources-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример ответа.

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResource",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "400279ff-8e85-4dcf-b1d6-d3a6be372951",
      "displayName": "Faculty cafeteria ordering",
      "description": "Example application",
      "url": "https://myapps.microsoft.com/example.com/signin/Faculty%20cafeteria%20ordering/f1e3b407-942d-4934-9a3f-cef1975cb988/",
      "resourceType": "Application",
      "originId": "2f1099a6-d4fc-4cc9-a0ef-ddd3f1bf0b7e",
      "accessPackageResourceScopes": [
          {
              "id": "452d78a7-69a5-482d-a82f-859a5169c55e",
              "displayName": "Root",
              "description": "Root Scope",
              "originId": "2f1099a6-d4fc-4cc9-a0ef-ddd3f1bf0b7e",
              "originSystem": "AadApplication",
              "isRootScope": true
          }
      ],
      "attributes": [
          {
              "id": "4f28e638-93de-4152-b631-2135da14c94a",
              "attributeName": "country",
              "attributeDefaultValue": null,
              "isEditable": true,
              "isPersistedOnAssignmentRemoval": false,
              "attributeSource": {
                  "@odata.type": "#microsoft.graph.resourceAttributeQuestion",
                  "question": {
                      "@odata.type": "#microsoft.graph.accessPackageMultipleChoiceQuestion",
                      "id": "6c797e12-e608-4ac9-90da-a8f18df37a94",
                      "isRequired": false,
                      "isAnswerEditable": null,
                      "sequence": 0,
                      "allowsMultipleSelection": false,
                      "text": {
                          "defaultText": "Enter your country",
                          "localizedTexts": []
                      },
                      "choices": [
                          {
                              "actualValue": "USA",
                              "displayValue": {
                                  "defaultText": "USA",
                                  "localizedTexts": [
                                      {
                                          "text": "USA",
                                          "languageCode": "en-US"
                                      }
                                  ]
                              }
                          },
                          {
                              "actualValue": "Canada",
                              "displayValue": {
                                  "defaultText": "Canada",
                                  "localizedTexts": [
                                      {
                                          "text": "Canada",
                                          "languageCode": "en-US"
                                      }
                                  ]
                              }
                          },
                          {
                              "actualValue": "India",
                              "displayValue": {
                                  "defaultText": "India",
                                  "localizedTexts": [
                                      {
                                          "text": "English",
                                          "languageCode": "en-US"
                                      }
                                  ]
                              }
                          }
                      ]
                  }
              },
              "attributeDestination": {
                  "@odata.type": "#microsoft.graph.userDirectoryAttributeStore"
              }
          }
      ]
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageResources",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
