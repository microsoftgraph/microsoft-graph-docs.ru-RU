---
title: Обновление приложения
description: Обновляет свойства объекта приложения.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 335281a0ac37ae3b966f731112223f019a67437d
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642830"
---
# <a name="update-application"></a>Обновление приложения

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновляет свойства объекта приложения.
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
| Authorization  | строка  | Bearer {токен}. Обязательный.  |

## <a name="request-body"></a>Тело запроса
В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|allowPublicClient|Boolean| Указывает, если приложения могут выступать в качестве открытого клиента. Например установленные приложения, запущенного на мобильном устройстве. Значение по умолчанию: *false*. |
|api|[api](../resources/api.md)| Указывает параметры для приложения API. |
|appRoles|Коллекция [appRole](../resources/approle.md)|Коллекция ролей приложения, которые могут быть объявлены приложением. Эти роли могут назначаться пользователям, группам или субъектам-службам. Значение null не допускается.|
|applicationAliases|Коллекция String| URI, определяющие приложение. Дополнительные сведения см. в статье [Объекты приложения и субъекта-службы](https://azure.microsoft.com/documentation/articles/active-directory-application-objects/). Для выражений фильтра в случае многозначных свойств требуется оператор *any*. Значение null не допускается. |
|createdDateTime|DateTimeOffset| Дата и время регистрации приложения. |
|deletedDateTime|DateTimeOffset| Дата и время удаления приложения. |
|displayName|String|Отображаемое имя приложения. |
|id|String|Уникальный идентификатор приложения. Наследуется от [directoryObject](../resources/directoryobject.md). Ключ. Значение null не допускается. Только для чтения. |
|info|[informationalUrl](../resources/informationalurl.md)| Основные сведения о профиле приложения. | Указывает параметры для установленных клиентов, например классических или мобильных устройств. |
|keyCredentials|Коллекция [keyCredential](../resources/keycredential.md)|Коллекция ключевых учетных данных, связанных с приложением. Значение null не допускается. |
|logo|Stream|Основной логотип для приложения. Значение null не допускается. |
|orgRestrictions|Коллекция String| Организационные tenantIds, к которому ограничен приложения.  Если коллекции пустое, приложение несколькими клиентами (не ограничено). Если коллекция содержит tenantIds, приложение ограничивается организационной tenantIds в коллекции. Указание других клиентов, но не tenantid расположения, где приложение регистрируется при значении tenantId приложения косвенно включен. |
|passwordCredentials|Коллекция [passwordCredential](../resources/passwordcredential.md)|Коллекция учетных данных паролей, связанных с приложением. Значение null не допускается.|
|preAuthorizedApplications|[preAuthorizedApplication](../resources/preauthorizedapplication.md) коллекции| Содержит список приложений и запрошенные разрешения для явного согласия пользователя. Требуется администраторам предоставляются разрешения для приложения. preAuthorizedApplications пользователя согласие на запрошенные разрешения не требуются. Разрешения, перечисленные в preAuthorizedApplications не требуют согласия пользователя. Тем не менее любые дополнительные запрошенные разрешения, не указанные в preAuthorizedApplications требуется согласия пользователя. |
|requiredResourceAccess|Коллекция [requiredResourceAccess](../resources/requiredresourceaccess.md)|Указывает ресурсы, к которым приложению требуется доступ, и устанавливает области разрешений OAuth и роли приложения, требующиеся приложению для каждого из этих ресурсов. Эта предварительная настройка доступа к необходимым ресурсам определяет интерфейс предоставления согласия. Значение null не допускается.|
|tags|Коллекция String| Настраиваемые строки, которые можно использовать для классификации и определения приложения. |
|web|[web](../resources/web.md)| Указывает параметры для веб-приложения. |

## <a name="response"></a>Отклик

Успешно завершена, этот метод возвращает `204 No Content` код ответа и не возвращает все действия в теле ответа.
## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
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
    "Error: /api-reference/beta/api/application-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
