---
title: Обновление allowedValue
description: Обновление свойств объекта allowedValue.
author: rolyon
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 2f0f8a20ea4b78bfab332082bca780a61ed0d4bf
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62103924"
---
# <a name="update-allowedvalue"></a>Обновление allowedValue
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [allowedValue.](../resources/allowedvalue.md)

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|CustomSecAttributeDefinition.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|CustomSecAttributeDefinition.ReadWrite.All|

Пользователю, заявиму, также должна быть назначена роль администратора [определения атрибутов.](/azure/active-directory/roles/permissions-reference) По умолчанию глобальные роли администратора и других администраторов не имеют разрешений на чтение, определение или назначение настраиваемого атрибута безопасности.

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /directory/customSecurityAttributeDefinitions/{customSecurityAttributeDefinitionId}/allowedValues/{allowedValueId}
```


## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
Укажите в тексте запроса *только* значения обновляемых свойств. Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.

В следующей таблице указаны свойства, которые можно обновить. 

|Свойство|Тип|Описание|
|:---|:---|:---|
|isActive|Логическое|Указывает, активна ли заранее заранее активная или деактивированная величина. Если установлено значение, это предварительное значение не может быть назначено дополнительным поддерживаемым `false` объектам каталога. Необязательный параметр.|



## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

## <a name="examples"></a>Примеры

### <a name="example-deactivate-a-predefined-value"></a>Пример: отключение заранее

В следующем примере отключает предварительное значение для настраиваемой определения атрибута безопасности.

+ Набор атрибутов: `Engineering`
+ Атрибут: `Project`
+ Предопределяемая величина: `Alpine`

#### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_allowedvalue"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/directory/customSecurityAttributeDefinitions/Engineering_Project/allowedValues/Alpine
Content-Type: application/json
Content-length: 80

{
    "isActive": "false"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-allowedvalue-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-allowedvalue-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-allowedvalue-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-allowedvalue-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-allowedvalue-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-allowedvalue-powershell-snippets.md)]
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
