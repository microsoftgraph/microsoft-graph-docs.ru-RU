---
title: Создание хранителя unifiedGroupSource
description: Создайте новый объект unifiedGroupSource хранителя, связанный с хранителями обнаружения электронных данных.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 71a8174570cc6fed779e564447569a7d832de138
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2022
ms.locfileid: "66838103"
---
# <a name="create-custodian-unifiedgroupsource"></a>Создание хранителя unifiedGroupSource
Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте новый [объект unifiedGroupSource](../resources/security-unifiedgroupsource.md) , связанный с хранителям [обнаружения электронных данных](../resources/security-ediscoverycustodian.md).

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|eDiscovery.Read.All, eDiscovery.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /security/cases/ediscoveryCases/{ediscoveryCaseId}/custodians/{custodianId}/unifiedGroupSources
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [unifiedGroupSource](../resources/security-unifiedgroupsource.md) в формате JSON.

При создании **unifiedGroupSource** можно указать следующие свойства.

>**Примечание:** Для **создания** **unifiedGroupSource** требуется group или **group@odata.bind**.

|Свойство|Тип|Описание|
|:---|:---|:---|
|includedSources|microsoft.graph.security.sourceType|Указывает источники, включенные в эту группу. Возможные значения: `mailbox`, `site`.|
|group;|String|Указывает адрес электронной почты для группы. Чтобы получить адрес электронной почты группы, используйте группы [list или](../api/group-list.md) [Get](../api/group-get.md). Затем можно выполнить запрос по имени группы, используя `$filter`, например, `https://graph.microsoft.com/v1.0/groups?$filter=displayName eq 'secret group'&$select=mail,id,displayName`.|
|group@odata.bind|Строка|Идентификатор группы. Вы можете получить его так же, как и группу. |

## <a name="response"></a>Отклик

В случае успешного выполнения этот `201 Created` метод возвращает код отклика и объект [microsoft.graph.security.unifiedGroupSource](../resources/security-unifiedgroupsource.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="example-1-create-unifiedgroupsource-with-group-smtp-address"></a>Пример 1. Создание unifiedGroupSource с smTP-адресом группы
#### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedgroupsource_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/custodians/0053a61a3b6c42738f7606791716a22a/unifiedGroupSources
Content-Type: application/json

{
    "group": {
        "mail": "SOCTeam@M365x809305.onmicrosoft.com"
    },
    "includedSources": "mailbox, site"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedgroupsource-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedgroupsource-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedgroupsource-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-unifiedgroupsource-from--go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-unifiedgroupsource-from--powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Отклик
Ниже приведен пример отклика.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security.unifiedGroupSource"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#security/cases/ediscoveryCases('b0073e4e-4184-41c6-9eb7-8c8cc3e2288b')/custodians('0053a61a3b6c42738f7606791716a22a')/unifiedGroupSources/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/groups/1ce58bf6-e0fd-403d-a655-312a838110cf",
    "displayName": "SOC Team (Mailbox)",
    "createdDateTime": "0001-01-01T00:00:00Z",
    "holdStatus": "applied",
    "id": "1ce58bf6-e0fd-403d-a655-312a838110cf",
    "includedSources": "mailbox,site",
    "createdBy": {
        "user": {
            "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
            "displayName": "MOD Administrator",
            "userPrincipalName": "admin@M365x809305.onmicrosoft.com"
        },
        "application": {
            "id": "de8bc8b5-d9f9-48b1-a8ad-b748da725064",
            "displayName": "Graph Explorer"
        }
    }
}
```

### <a name="example-2-create-unifiedgroupsource-with-groupodatabind"></a>Пример 2. Создание unifiedGroupSource с group@odata.bind
#### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedgroupsource_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/custodians/0053a61a3b6c42738f7606791716a22a/unifiedGroupSources
Content-Type: application/json

{
    "group@odata.bind": "https://graph.microsoft.com/v1.0/groups/93f90172-fe05-43ea-83cf-ff785a40d610",
    "includedSources": "mailbox"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedgroupsource-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedgroupsource-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedgroupsource-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-unifiedgroupsource-from--go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-unifiedgroupsource-from--powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Отклик
Ниже приведен пример отклика.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security.unifiedGroupSource"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#security/cases/ediscoveryCases('b0073e4e-4184-41c6-9eb7-8c8cc3e2288b')/custodians('0053a61a3b6c42738f7606791716a22a')/unifiedGroupSources/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/groups/93f90172-fe05-43ea-83cf-ff785a40d610",
    "displayName": "Finance Team (Mailbox)",
    "createdDateTime": "0001-01-01T00:00:00Z",
    "holdStatus": "applied",
    "id": "93f90172-fe05-43ea-83cf-ff785a40d610",
    "includedSources": "mailbox",
    "createdBy": {
        "user": {
            "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
            "displayName": "MOD Administrator",
            "userPrincipalName": "admin@M365x809305.onmicrosoft.com"
        },
        "application": {
            "id": "de8bc8b5-d9f9-48b1-a8ad-b748da725064",
            "displayName": "Graph Explorer"
        }
    }
}
```
