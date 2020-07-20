---
title: Обновление serviceprincipal
description: Обновление свойств объекта serviceprincipal.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 49f9d1f19b1c77eb2b0b4873e75ec44cb5a43422
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895967"
---
# <a name="update-serviceprincipal"></a>Обновление servicePrincipal

Пространство имен: microsoft.graph

Обновление свойств объекта [servicePrincipal](../resources/serviceprincipal.md) .

> [!IMPORTANT]
> Использование PATCH для установки [**пассвордкредентиал**](../resources/passwordcredential.md) не поддерживается. Используйте методы [аддпассворд](./serviceprincipal-addpassword.md) и [ремовепассворд](./serviceprincipal-removepassword.md) , чтобы обновить пароль для servicePrincipal.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Application. ReadWrite. ALL, Directory. AccessAsUser. ALL    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Application.ReadWrite.OwnedBy, Application.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
PATCH /servicePrincipals/{id}
```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Описание|
|:-----------|:----------|
| Авторизация | Bearer {токен}. Обязательный.  |
| Content-Type | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса
В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.

| Свойство     | Тип |Описание|
|:---------------|:--------|:----------|
|accountEnabled|Логический| Значение **true**, если учетная запись субъекта-службы включена. В противном случае используется значение **false**.|
|addIns| [addIn](../resources/addin.md) | Определяет пользовательское поведение, которое служба может использовать для вызова приложения в определенных контекстах. Например, приложения, которые способны визуализировать файловые потоки, [могут установить свойство addIns](https://docs.microsoft.com/onedrive/developer/file-handlers/?view=odsp-graph-online) для его функции "FileHandler". Это позволит таким службам, как Microsoft 365, вызывать приложение в контексте документа, над которым работает пользователь.|
|алтернативенамес|Коллекция String| Используется для получения субъектов служб по подписке, идентификации группы ресурсов и полных идентификаторов ресурсов для [управляемых удостоверений](https://aka.ms/azuremanagedidentity).|
|appRoleAssignmentRequired|Boolean|Указывает, требуется ли объект **appRoleAssignment** для пользователя или группы, перед тем как Azure AD выпустит маркер пользователя или доступа для приложения. Значение null не допускается. |
|appRoles|Коллекция [appRole](../resources/approle.md)|Роли приложения, предоставляемые связанным приложением. Дополнительные сведения см. в описании свойства **appRoles** ресурса [Application](../resources/application.md) . Значение null не допускается. |
|displayName|Строка|Отображаемое имя для субъекта-службы.|
|homepage|String|Домашняя или целевая страница приложения.|
|keyCredentials|Коллекция [keyCredential](../resources/keycredential.md)|Коллекция ключевых учетных данных, связанных с субъектом-службой. Значение null не допускается.            |
|logoutUrl|String| Указывает URL-адрес, используемый службой проверки подлинности корпорации Майкрософт для выхода пользователя с помощью [основного канала](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [обратного канала](https://openid.net/specs/openid-connect-backchannel-1_0.html) или протоколов выхода SAML.|
|oauth2PermissionScopes|Коллекция [permissionScope](../resources/permissionScope.md)|Области разрешений OAuth 2,0, предоставляемые связанным приложением. Дополнительные сведения см. в описании свойства **oauth2PermissionScopes** ресурса [Application](../resources/application.md) . Значение null не допускается.|
|replyUrls|Коллекция String|URL-адреса, которым отправляются маркеры пользователей для входа с помощью связанного приложения, или URI перенаправления, которым отправляются коды авторизации OAuth 2.0 и маркеры доступа для связанного приложения. Значение null не допускается. |
|ServicePrincipalNames|Коллекция String|Содержит список **идентифиерсурис**, скопированных из связанного [приложения](../resources/application.md). В гибридные приложения можно добавлять дополнительные значения. Эти значения можно использовать для определения разрешений, предоставляемых приложением в Azure AD. For example,<ul><li>Клиентские приложения, запрашивающие разрешения для этого ресурса, могут использовать эти URI для указания необходимых разрешений в свойстве **рекуиредресаурцеакцесс** манифеста приложения или в колонке "разрешения API" в функции регистрации приложений.</li><li>Клиентские приложения могут указывать URI ресурса, основанный на значениях этого свойства для получения маркера доступа, который представляет собой URI, возвращенный в утверждении "ауд".</li></ul><br>Для выражений фильтра в случае многозначных свойств требуется оператор any. Значение null не допускается.|
|tags|Коллекция String| Настраиваемые строки, которые можно использовать для классификации и определения приложения. Значение null не допускается. |
| tokenEncryptionKeyId |String|Задает значение открытого ключа keyId из коллекции keyCredentials. При настройке в Azure AD маркеры проблем для этого приложения шифруются с помощью ключа, указанного этим свойством. Код приложения, получающий зашифрованный маркер, должен использовать соответствующий закрытый ключ для расшифровки маркера, прежде чем его можно будет применить для пользователя, выполнившего вход.|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `204 No Content` код отклика и обновленный объект [servicePrincipal](../resources/serviceprincipal.md) в тексте отклика.
## <a name="example"></a>Пример
### <a name="request"></a>Запрос
Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_serviceprincipal"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/servicePrincipals/{id}
Content-type: application/json
Content-length: 391

{
  "appRoleAssignmentRequired": true
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update serviceprincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
