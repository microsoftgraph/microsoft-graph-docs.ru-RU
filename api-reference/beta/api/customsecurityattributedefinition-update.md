---
title: Обновление customSecurityAttributeDefinition
description: Обновление свойств объекта customSecurityAttributeDefinition.
author: rolyon
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
---

# <a name="update-customsecurityattributedefinition"></a>Обновление customSecurityAttributeDefinition
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [customSecurityAttributeDefinition](../resources/customsecurityattributedefinition.md) .

## <a name="permissions"></a>Разрешения:
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|CustomSecAttributeDefinition.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|CustomSecAttributeDefinition.ReadWrite.All|

Кроме того, пользователю, заявив о подписании, должна быть назначена роль администратора [определения атрибутов](/azure/active-directory/roles/permissions-reference). По умолчанию глобальные роли администратора и других администраторов не имеют разрешений на чтение, определение или назначение настраиваемого атрибута безопасности.

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /directory/customSecurityAttributeDefinitions/{customSecurityAttributeDefinitionId}
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|
|OData-Version|4.01. Необязательный параметр.|

> [!NOTE]
> Чтобы обновить заданные значения для настраиваемого атрибута безопасности, необходимо добавить заглавную статью **OData-Version** и назначить ему значение `4.01`.

## <a name="request-body"></a>Текст запроса
Укажите в тексте запроса *только* значения обновляемых свойств. Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.

В следующей таблице указаны свойства, которые можно обновить. 

|Свойство|Тип|Описание|
|:---|:---|:---|
|description|Строка|Описание настраиваемого атрибута безопасности. Может иметь длину до 128 символов и включать символы Unicode. Необязательный параметр.|
|status|String|Указывает, активен ли настраиваемый атрибут безопасности или отключен. Допустимые значения и `Available` `Deprecated`. Необязательный параметр.|
|usePreDefinedValuesOnly|Логический|Указывает, могут ли быть назначены только предопределяемые значения атрибуту настраиваемой безопасности. Если установлено значение false, разрешены значения свободной формы. Может быть изменена с true на false, но не может быть изменена с false на true. Если `type` задана настройка Boolean, `usePreDefinedValuesOnly` не может быть задана истина. Необязательный параметр.|



## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

## <a name="examples"></a>Примеры

### <a name="example-1-update-a-custom-security-attribute"></a>Пример 1. Обновление настраиваемой атрибута безопасности

В следующем примере обновляется описание пользовательского определения атрибута безопасности.

+ Набор атрибутов: `Engineering`
+ Атрибут: `ProjectDate`

#### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_customsecurityattributedefinition"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/directory/customSecurityAttributeDefinitions/Engineering_ProjectDate
Content-Type: application/json

{
  "description": "Target completion date (YYYY/MM/DD)",
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-customsecurityattributedefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-customsecurityattributedefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-customsecurityattributedefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-customsecurityattributedefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-customsecurityattributedefinition-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-customsecurityattributedefinition-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-the-predefined-values-for-a-custom-security-attribute"></a>Пример 2. Обновление предопределяемых значений для настраиваемой атрибута безопасности

В следующем примере обновляется состояние существующего предопределяемого значения и добавляется новое предопределеное значение для настраиваемого определения атрибута безопасности.

+ Набор атрибутов: `Engineering`
+ Атрибут: `Project`
+ Тип данных атрибута: коллекция строк
+ Обновление предопределяемой величины: `Baker`
+ Новое заранее заранее заранеее значение: `Skagit`

> [!NOTE]
> Для этого запроса необходимо добавить **загодер OData-Version** и назначить ему значение `4.01`.

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "update_customsecurityattributedefinition_allowedvalues"
}
-->
``` msgraph-interactive
PATCH https://graph.microsoft.com/beta/directory/customSecurityAttributeDefinitions/Engineering_Project
Content-Type: application/json
OData-Version: 4.01

{
    "allowedValues@delta": [
        {
            "id": "Baker",
            "isActive": false
        },
        {
            "id": "Skagit",
            "isActive": true
        }
    ]
}
```

#### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-deactivate-a-custom-security-attribute"></a>Пример 3. Деактивировать настраиваемый атрибут безопасности

В следующем примере деактивирует настраиваемую определение атрибута безопасности.

+ Набор атрибутов: `Engineering`
+ Атрибут: `Project`

#### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_customsecurityattributedefinition_deactivate"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/directory/customSecurityAttributeDefinitions/Engineering_Project
Content-Type: application/json

{
  "status": "Deprecated"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-customsecurityattributedefinition-deactivate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-customsecurityattributedefinition-deactivate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-customsecurityattributedefinition-deactivate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-customsecurityattributedefinition-deactivate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-customsecurityattributedefinition-deactivate-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-customsecurityattributedefinition-deactivate-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
