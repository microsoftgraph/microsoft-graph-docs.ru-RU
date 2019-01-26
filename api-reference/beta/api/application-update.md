---
title: Обновление приложения
description: Обновляет свойства объекта приложения.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9965a46e340063940e1a9af18a89ada7e492bf26
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572215"
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
|Для приложений | Application.ReadWrite.OwnedBy Application.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
PATCH /applications/{id}
```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {токен}. Обязательный.  |

## <a name="request-body"></a>Текст запроса
В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|allowPublicClient|Boolean| Указывает, если приложения могут выступать в качестве открытого клиента. Например установленные приложения, запущенного на мобильном устройстве. Значение по умолчанию: *false*. |
|API|[API](../resources/api.md)| Задает параметры для приложения API. |
|appRoles|Коллекция [роли приложения](../resources/approle.md)|Коллекция ролей приложений, которые могут объявить приложения. Эти роли можно назначить только пользователей, групп и субъектов-служб. Значение null не допускается.|
|applicationAliases|Коллекция String| Коды URI, определения приложения. Дополнительные сведения содержатся, [приложения и объекты участников-служб](https://azure.microsoft.com/documentation/articles/active-directory-application-objects/). Для выражений фильтра в случае многозначных свойств требуется оператор *any*. Значение null не допускается. |
|createdDateTime|DateTimeOffset| Дата и время регистрации приложения. |
|deletedDateTime|DateTimeOffset| Дата и время приложения был удален. |
|displayName|Строка|Отображаемое имя для приложения. |
|id|Строка|Уникальный идентификатор для приложения. Наследуется от [directoryObject](../resources/directoryobject.md). Ключ. Значение null не допускается. Только для чтения. |
|сведения о|[informationalUrl](../resources/informationalurl.md)| Сведения о базовой профиля приложения. | Задает параметры для установленных клиентов, таких как настольного компьютера или мобильного устройства. |
|keyCredentials|[keyCredential](../resources/keycredential.md) коллекции|Коллекция ключа учетных данных, связанных с приложением, не допускает значение NULL. |
|logo|Stream|Основной логотип для приложения. Значение null не допускается. |
|orgRestrictions|Коллекция String| Организационные tenantIds, к которому ограничен приложения.  Если коллекции пустое, приложение несколькими клиентами (не ограничено). Если коллекция содержит tenantIds, приложение ограничивается организационной tenantIds в коллекции. Указание других клиентов, но не tenantid расположения, где приложение регистрируется при значении tenantId приложения косвенно включен. |
|passwordCredentials|[passwordCredential](../resources/passwordcredential.md) коллекции|Коллекция пароль учетных данных, связанных с приложением. Значение null не допускается.|
|preAuthorizedApplications|[preAuthorizedApplication](../resources/preauthorizedapplication.md) коллекции| Содержит список приложений и запрошенные разрешения для явного согласия пользователя. Требуется администраторам предоставляются разрешения для приложения. preAuthorizedApplications пользователя согласие на запрошенные разрешения не требуются. Разрешения, перечисленные в preAuthorizedApplications не требуют согласия пользователя. Тем не менее любые дополнительные запрошенные разрешения, не указанные в preAuthorizedApplications требуется согласия пользователя. |
|requiredResourceAccess|[requiredResourceAccess](../resources/requiredresourceaccess.md) коллекции|Указывает ресурсы, которые этого приложения требуется доступ к и набор области разрешений OAuth и роли приложений, которые требуется в каждом из этих ресурсов. В этом предварительной настройки доступа к необходимых ресурсов дисков на взаимодействие с согласия пользователя. Значение null не допускается.|
|tags|Коллекция String| Настраиваемых строк, которые можно использовать для классификации и определения приложения. |
|web|[веб-приложения](../resources/web.md)| Задает параметры для веб-приложения. |

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
