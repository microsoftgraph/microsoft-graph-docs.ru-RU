---
title: Обновление unifiedRoleDefinition
description: Обновление свойств объекта unifiedRoleDefinition.
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: fc93caf0471c1f8c0e3d73b895a530b809656548
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59097943"
---
# <a name="update-unifiedroledefinition"></a>Обновление unifiedRoleDefinition

Пространство имен: microsoft.graph

Обновление свойств объекта [unifiedRoleDefinition.](../resources/unifiedroledefinition.md) Невозможно обновить встроенные роли.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | RoleManagement.ReadWrite.Directory |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | RoleManagement.ReadWrite.Directory |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
PATCH /roleManagement/directory/roleDefinitions/{id}
```

## <a name="request-headers"></a>Заголовки запросов
    
| Имя       | Описание|
|:-----------|:-----------|
| Авторизация | Bearer {token} |
| Content-Type | application/json. Обязательный. |
    
## <a name="request-body"></a>Текст запроса
    
В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для лучшей производительности не включайте существующие значения, которые не изменились.
    
В следующей таблице показаны свойства, необходимые при обновлении [единогоRoleDefinition.](../resources/unifiedroledefinition.md)

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|description|String| Описание определения роли. Только для чтения, **когда isBuiltIn** `true` является . |
|displayName|Строка| Имя отображения для определения роли. Только для чтения, **когда isBuiltIn** `true` является . Обязательное.|
|isEnabled|Boolean| Флаг, указывающий, включена ли роль для назначения. Если `false` роль недоступна для назначения. Только для чтения, **когда isBuiltIn** является правдой. |
|resourceScopes|Коллекция String| Список областей и разрешений, к которые применяется определение роли. В настоящее `/` время поддерживается только. Только для чтения, **когда isBuiltIn** является правдой. **НЕ ИСПОЛЬЗУЙТЕ. В ближайшее время это свойство будет обесценилось. Прикрепить область к назначению ролей.**|
|rolePermissions|[коллекция unifiedRolePermission](../resources/unifiedrolepermission.md)| Список разрешений, включенных в роль. Только для чтения, **когда isBuiltIn** `true` является . Обязательный. |
|templateId|String| Настраиваемый идентификатор шаблона, который можно установить, **когда isBuiltIn** `false` . Этот идентификатор обычно используется, если требуется, чтобы идентификатор был одинаковым в разных каталогах. Только для чтения, **когда isBuiltIn** `true` является . |
|version|String| Указывает версию определения роли. Только для чтения, **когда isBuiltIn** `true` является .|

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

Ниже приведен пример запроса.



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_unifiedroledefinition"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/roleManagement/directory/roleDefinitions/0d55728d-3e24-4309-9b1b-5ac09921475a
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

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true
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

