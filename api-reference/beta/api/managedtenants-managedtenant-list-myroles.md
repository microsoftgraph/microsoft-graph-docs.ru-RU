---
title: Перечисление myRoles
description: Получение ролей, которые есть у вошедского пользователя через делегированное отношение между управляемыми клиентами.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: cc1701a57eb77cd667ecf2ec07e6c92fd13b35b7
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/15/2022
ms.locfileid: "66096432"
---
# <a name="list-myroles"></a>Перечисление myRoles
Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение ролей, которые есть у вошедского пользователя через делегированное отношение между управляемыми клиентами.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|ManagedTenants.Read.All, ManagedTenants.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/myRoles
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает некоторые параметры запросов OData для настройки отклика. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код `200 OK` отклика и коллекцию объектов [myRole](../resources/managedtenants-myrole.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_myrole"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/myRoles
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-myrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-myrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-myrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-myrole-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример отклика.

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.myRole",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/tenantRelationships/managedTenants/$metadata#myRoles",
  "value": [
    {
      "tenantId": "06b192f6-991c-4f3a-b4f6-ed85580566cf",
      "assignments": [
        {
          "assignmentType": "delegatedAdminPrivileges",
          "roles": [
            {
              "templateId": "729827e3-9c14-49f7-bb1b-9608f156bbb8",
              "displayName": "Helpdesk Administrator",
              "description": "Can reset passwords for non-administrators and Helpdesk Administrators."
            },
            {
              "templateId": "62e90394-69f5-4237-9190-012177145e10",
              "displayName": "Global Administrator",
              "description": "Can manage all aspects of Azure AD and Microsoft services that use Azure AD identities."
            }
          ]
        },
        {
          "assignmentType": "granularDelegatedAdminPrivileges",
          "roles": [
            {
              "templateId": "3a2c62db-5318-420d-8d74-23affee5d9d5",
              "displayName": "Intune Administrator",
              "description": "Can manage all aspects of the Intune product."
            },
            {
              "templateId": "69091246-20e8-4a56-aa4d-066075b2a7a8",
              "displayName": "Teams Administrator",
              "description": "Can manage the Microsoft Teams service."
            },
            {
              "templateId": "5d6b6bb7-de71-4623-b4af-96380a352509",
              "displayName": "Security Reader",
              "description": "Can read security information and reports in Azure AD and Office 365."
            }
          ]
        }
      ]
    },
    {
      "tenantId": "5618f6-991c-4f3a-b4f6-ed85580566cf",
      "assignments": [
        {
          "assignmentType": "delegatedAdminPrivileges",
          "roles": [
            {
              "templateId": "729827e3-9c14-49f7-bb1b-9608f156bbb8",
              "displayName": "Helpdesk Administrator",
              "description": "Can reset passwords for non-administrators and Helpdesk Administrators."
            }
          ]
        },
        {
          "assignmentType": "granularDelegatedAdminPrivileges",
          "roles": [
            {
              "templateId": "194ae4cb-b126-40b2-bd5b-6091b380977d",
              "displayName": "Security Administrator",
              "description": "Can read security information and reports, and manage configuration in Azure AD and Office 365."
            },
            {
              "templateId": "11451d60-acb2-45eb-a7d6-43d0f0125c13",
              "displayName": "Windows 365 Administrator",
              "description": "Can provision and manage all aspects of Cloud PCs."
            }
          ]
        }
      ]
    }
  ]
}
```
