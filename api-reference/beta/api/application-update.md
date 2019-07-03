---
title: Обновление приложения
description: Обновление свойств объекта Application.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: dea134cc61e586f94c08755ef812f9f4b7f4e8f7
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35439597"
---
# <a name="update-application"></a>Обновление приложения

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта Application.
## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).


|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) |  Directory.AccessAsUser.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Application.ReadWrite.OwnedBy, Application.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
PATCH /applications/{id}
```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {токен}. Обязательный.  |

## <a name="request-body"></a>Тело запроса
В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|allowPublicClient|Boolean| Указывает, может ли приложение работать в качестве общедоступного клиента. Например, установленное приложение, запущенное на мобильном устройстве. Значение по умолчанию: *false*. |
|api|[apiApplication](../resources/apiapplication.md)| Указывает параметры для приложения API. |
|appRoles|Коллекция [appRole](../resources/approle.md)|Коллекция ролей приложения, которые могут быть объявлены приложением. Эти роли могут назначаться пользователям, группам или субъектам-службам. Значение null не допускается.|
|applicationAliases|Коллекция String| URI, определяющие приложение. Дополнительные сведения см. в статье [Объекты приложения и субъекта-службы](https://azure.microsoft.com/documentation/articles/active-directory-application-objects/). Для выражений фильтра в случае многозначных свойств требуется оператор *any*. Значение null не допускается. |
|createdDateTime|DateTimeOffset| Дата и время регистрации приложения. |
|deletedDateTime|DateTimeOffset| Дата и время удаления приложения. |
|displayName|Строка|Отображаемое имя приложения. |
|id|String|Уникальный идентификатор приложения. Наследуется от [directoryObject](../resources/directoryobject.md). Ключ. Значение null не допускается. Только для чтения. |
|info|[informationalUrl](../resources/informationalurl.md)| Основные сведения о профиле приложения. | Указывает параметры для установленных клиентов, например классических или мобильных устройств. |
|keyCredentials|Коллекция [keyCredential](../resources/keycredential.md)|Коллекция ключевых учетных данных, связанных с приложением. Значение null не допускается. |
|logo|Stream|Основной логотип для приложения. Значение null не допускается. |
|orgRestrictions|Коллекция String| Организационное Тенантидс, к которому приложение ограничено.  Если коллекция пуста, приложение является несколькими клиентами (не ограничено). Если коллекция содержит Тенантидс, приложение ограничено Тенантидс Организации в коллекции. Указание других клиентов, кроме tenantId, где зарегистрировано приложение, предполагает косвенное включение собственного tenantId приложения. |
|passwordCredentials|Коллекция [passwordCredential](../resources/passwordcredential.md)|Коллекция учетных данных паролей, связанных с приложением. Значение null не допускается.|
|Преаусоризедаппликатионс|Коллекция [preAuthorizedApplication](../resources/preauthorizedapplication.md)| Перечисляет приложения и запрашиваемые разрешения для неявного согласия. Необходимо, чтобы администратор предоставил согласие на применение приложения. Преаусоризедаппликатионс не требуют от пользователя согласия с запрошенными разрешениями. Разрешения, перечисленные в Преаусоризедаппликатионс, не требуют согласия пользователя. Однако все дополнительные запрошенные разрешения, не указанные в Преаусоризедаппликатионс, требуют согласия пользователя. |
|requiredResourceAccess|Коллекция [requiredResourceAccess](../resources/requiredresourceaccess.md)|Указывает ресурсы, к которым приложению требуется доступ, и устанавливает области разрешений OAuth и роли приложения, требующиеся приложению для каждого из этих ресурсов. Эта предварительная настройка доступа к необходимым ресурсам определяет интерфейс предоставления согласия. Значение null не допускается.|
|tags|Коллекция String| Настраиваемые строки, которые можно использовать для классификации и определения приложения. |
|web|[webApplication](../resources/webapplication.md)| Указывает параметры для веб-приложения. |

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `204 No Content` код отклика и не возвращает ничего в тексте отклика.
## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_application"
}-->
```http
PATCH https://graph.microsoft.com/beta/applications/{id}
Content-type: application/json
Content-length: 72

{
  "allowPublicClient": false,
  "displayName": "New display name"
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Цель — C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>Отклик
Примечание. Представленный здесь объект отклика может быть усечен для краткости. 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
