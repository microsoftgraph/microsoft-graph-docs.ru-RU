---
title: 'accessPackage: getApplicablePolicyRequirements'
description: Разрешить звонителям находить требования для запроса назначения для определенного accessPackage.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 21f3f3537ffc24f157a6dbd46673af35d92f1452
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62341847"
---
# <a name="accesspackage-getapplicablepolicyrequirements"></a>accessPackage: getApplicablePolicyRequirements
Пространство имен: microsoft.graph


В [управлении правами Azure AD](../resources/entitlementmanagement-overview.md) это действие извлекает список объектов [accessPackageAssignmentRequestRequirements](../resources/accesspackageassignmentrequestrequirements.md) , которые в настоящее время пользователь может использовать для создания [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md).  Каждый объект требования соответствует политике назначения пакетов доступа, для которых подписанное в настоящее время пользователь может запрашивать назначение.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/entitlementManagement/accessPackages/{accessPackageId}/getApplicablePolicyRequirements
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик
`200 OK` В случае успешного выполнения этот метод возвращает код ответа и коллекцию [accessPackageAssignmentRequestRequirements](../resources/accesspackageassignmentrequestrequirements.md) в тексте отклика, по одному объекту для каждой политики, для которой пользователь является **разрешеннымRequestor**. Если политика не имеет требований, то будут иметься и значения **accessPackageAssignmentRequestRequirements** `false` `null` . Если нет политик, в которых пользователь является **разрешеннымRequestor**, вместо него будет возвращена пустая коллекция.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accesspackage_getapplicablepolicyrequirements"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/accessPackages/{accessPackageId}/getApplicablePolicyRequirements
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accesspackage-getapplicablepolicyrequirements-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accesspackage-getapplicablepolicyrequirements-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accesspackage-getapplicablepolicyrequirements-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accesspackage-getapplicablepolicyrequirements-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/accesspackage-getapplicablepolicyrequirements-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/accesspackage-getapplicablepolicyrequirements-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessPackageAssignmentRequestRequirements)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "microsoft.graph.accessPackageAssignmentRequestRequirements"
    }
  ]
}
```


