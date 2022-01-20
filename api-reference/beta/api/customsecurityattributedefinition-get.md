---
title: Get customSecurityAttributeDefinition
description: Ознакомьтесь с свойствами и отношениями объекта customSecurityAttributeDefinition.
author: rolyon
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 85d2fe3cdce1517a01fa2905fa7073540f56be24
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62134042"
---
# <a name="get-customsecurityattributedefinition"></a>Get customSecurityAttributeDefinition
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ознакомьтесь с свойствами и отношениями объекта [customSecurityAttributeDefinition.](../resources/customsecurityattributedefinition.md)

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|CustomSecAttributeAssignment.ReadWrite.All, CustomSecAttributeDefinition.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|CustomSecAttributeAssignment.ReadWrite.All, CustomSecAttributeDefinition.ReadWrite.All|

Кроме того, пользователю, заявляемого на учет, должна быть назначена одна из следующих ролей [каталога:](/azure/active-directory/roles/permissions-reference)

+ Считыватель определения атрибутов
+ Администратор назначения атрибутов
+ Администратор определения атрибутов

По умолчанию глобальные роли администратора и других администраторов не имеют разрешений на чтение, определение или назначение настраиваемого атрибута безопасности.

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /directory/customSecurityAttributeDefinitions/{customSecurityAttributeDefinitionId}
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает `$select` параметры запроса OData для настройки ответа. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Тело запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика и настраиваемый `200 OK` [объектSecurityAttributeDefinition](../resources/customsecurityattributedefinition.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="example-get-a-custom-security-attribute"></a>Пример: Получить настраиваемый атрибут безопасности

В следующем примере получается одно настраиваемая определение атрибута безопасности.

+ Набор атрибутов: `Engineering`
+ Атрибут: `ProjectDate`

#### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_customsecurityattributedefinition"
}
-->
``` http
GET https://graph.microsoft.com/beta/directory/customSecurityAttributeDefinitions/Engineering_ProjectDate
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-customsecurityattributedefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-customsecurityattributedefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-customsecurityattributedefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-customsecurityattributedefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-customsecurityattributedefinition-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-customsecurityattributedefinition-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.customSecurityAttributeDefinition"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#directory/customSecurityAttributeDefinitions/$entity",
    "attributeSet": "Engineering",
    "description": "Target completion date",
    "id": "Engineering_ProjectDate",
    "isCollection": false,
    "isSearchable": true,
    "name": "ProjectDate",
    "status": "Available",
    "type": "String",
    "usePreDefinedValuesOnly": false
}
```
