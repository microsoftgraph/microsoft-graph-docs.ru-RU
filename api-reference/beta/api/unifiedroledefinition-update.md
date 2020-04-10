---
title: Обновление Унифиедроледефинитион
description: Обновление свойств объекта Унифиедроледефинитион.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fb1cd8a7e8cbef279c5007b3cd721193ff25e518
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218943"
---
# <a name="update-unifiedroledefinition"></a>Обновление Унифиедроледефинитион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [унифиедроледефинитион](../resources/unifiedroledefinition.md) .

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Ролеманажемент. Read. Directory, Ролеманажемент. ReadWrite. Directory |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | Ролеманажемент. Read. Directory, Ролеманажемент. ReadWrite. Directory |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
PATCH /roleManagement/directory/roleDefinitions/{id}
```

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Описание|
|:-----------|:-----------|
| Authorization | Bearer {token} |

## <a name="request-body"></a>Текст запроса

В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|description|String| Описание определения роли. Только для чтения, если для Builtin задано значение true. |
|displayName|Строка| Отображаемое имя определения роли. Только для чтения, если для Builtin задано значение true. Обязательный.|
|id|Строка| Уникальный идентификатор для определения роли. Key, не допускающая значение null, только для чтения. |
|isBuiltIn|Boolean| Флаг, указывающий, является ли определение роли частью набора по умолчанию, входящего в состав продукта или настраиваемого. Только для чтения. |
|isEnabled|Boolean| Флаг, указывающий, включена ли роль для назначения. Если значение false, роль недоступна для назначения. Только для чтения, если для Builtin задано значение true. |
|resourceScopes|Коллекция String| Список разрешений областей, к которым применяется определение роли. В настоящее время поддерживается только "/". Только для чтения, если для Builtin задано значение true. **НЕ ИСПОЛЬЗУЙТЕ. Это свойство будет нерекомендуемым в ближайшее время. Присоединение области к назначению ролей.**|
|rolePermissions|Коллекция [унифиедролепермиссион](../resources/unifiedrolepermission.md)| Список разрешений, включенных в роль. Только для чтения, если для Builtin задано значение true. Обязательный атрибут. |
|templateId|Строка| Настраиваемый идентификатор шаблона, который можно задать, если параметру Builtin присвоено значение false. Этот идентификатор обычно используется, если необходимо, чтобы один идентификатор совпадал для разных каталогов. Только для чтения, если для Builtin задано значение true. |
|version|String| Указывает версию определения роли. Только для чтения, если для Builtin задано значение true.|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [унифиедроледефинитион](../resources/unifiedroledefinition.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_unifiedroledefinition"
}-->

```http
PATCH https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/0d55728d-3e24-4309-9b1b-5ac09921475a
Content-type: application/json

{
  "description": "Update basic properties of application registrations",
  "displayName": "Application Registration Support Administrator",
  "rolePermissions":
    [
        {
            "allowedResourceActions": 
            [
                "microsoft.directory/applications/basic/read"
            ]
        }
    ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример отклика.
> **Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition"
} -->

```http
HTTP/1.1 204 OK
Content-type: application/json

```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update unifiedroledefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
