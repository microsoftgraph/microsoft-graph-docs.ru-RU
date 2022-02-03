---
title: 'applicationTemplate: instantiate'
description: Используйте этот API для создания нового приложенияTemplate
ms.localizationpriority: medium
author: luleonpla
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: c55b93249535bc12b26c299a3d4a916f739d0fe4
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62339300"
---
# <a name="applicationtemplate-instantiate"></a>applicationTemplate: instantiate

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Добавьте экземпляр приложения из галереи приложений Azure AD в каталог.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Application.ReadWrite.All, Directory.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Приложение                            | Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /applicationTemplates/{id}/instantiate
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание   |
|:--------------|:--------------|
| Авторизация | Bearer {code} |

## <a name="request-body"></a>Текст запроса

В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр    | Тип        | Описание |
|:-------------|:------------|:------------|
|displayName|String|Настраиваемая фамилия приложения|

## <a name="response"></a>Отклик

В случае успешного применения этот метод возвращает код `201 OK` отклика и новый [объект applicationServicePrincipal](../resources/applicationserviceprincipal.md) в тексте ответа.

## <a name="examples"></a>Примеры

В приведенном ниже примере показано, как вызывать этот API.

### <a name="request"></a>Запрос

Ниже приведен пример запроса.
 
> Этот API можно использовать для мгновенного запуска приложений [, не в галерее](/azure/active-directory/manage-apps/add-non-gallery-app). Используйте следующий ID для **applicationTemplate**: `8adf8e6e-67b2-4cf2-a259-e3dc5476c621`.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "applicationtemplate_instantiate"
}-->

```http
POST https://graph.microsoft.com/beta/applicationTemplates/{id}/instantiate
Content-type: application/json

{
  "displayName": "My custom name"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/applicationtemplate-instantiate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/applicationtemplate-instantiate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/applicationtemplate-instantiate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/applicationtemplate-instantiate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/applicationtemplate-instantiate-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/applicationtemplate-instantiate-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример отклика.

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости. 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationServicePrincipal"
} -->

```http
HTTP/1.1 201 OK
Content-type: application/json

{
   "servicePrincipal":{
      "accountEnabled":true,
      "addIns":[
         {
            "id":"id-value",
            "type":"type-value",
            "properties":[
               {
                  "key":"key-value",
                  "value":"value-value"
               }
            ]
         }
      ],
      "appDisplayName":"appDisplayName-value",
      "appId":"appId-value",
      "appOwnerOrganizationId":"appOwnerOrganizationId-value",
      "appRoleAssignmentRequired":true
   },
   "application":{
      "api":{
         "acceptedAccessTokenVersion":1,
         "publishedPermissionScopes":[
            {
               "adminConsentDescription":"adminConsentDescription-value",
               "adminConsentDisplayName":"adminConsentDisplayName-value",
               "id":"id-value",
               "isEnabled":true,
               "type":"type-value",
               "userConsentDescription":"userConsentDescription-value",
               "userConsentDisplayName":"userConsentDisplayName-value",
               "value":"value-value"
            }
         ]
      },
      "allowPublicClient":true,
      "applicationAliases":[
         "applicationAliases-value"
      ],
      "createdDateTime":"datetime-value",
      "installedClients":{
         "redirectUrls":[
            "redirectUrls-value"
         ]
      }
   }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationTemplate: instantiate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

