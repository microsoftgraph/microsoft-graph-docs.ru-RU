---
title: Обновление serviceprincipal
description: Обновление свойства объекта serviceprincipal.
localization_priority: Normal
ms.openlocfilehash: 946db869863d74a94e2e9adc04a66c8d9a50e4f5
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573860"
---
# <a name="update-serviceprincipal"></a>Обновление serviceprincipal

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойства объекта serviceprincipal.
## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Directory.AccessAsUser.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Application.ReadWrite.OwnedBy Application.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
PATCH /servicePrincipals/{id}
```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса
В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|accountEnabled|Логический|                **значение true,** Если включена участника учетной записи службы. в противном случае — **false**.            |
|appDisplayName|Строка|Отображаемое имя, предоставляемые элементом соответствующего приложения.|
|appId|String|Уникальный идентификатор для соответствующего приложения (его свойство **appId** ).|
|appRoleAssignmentRequired|Boolean|Указывает, будет ли **appRoleAssignment** пользователю или группе требуется перед Azure AD выпустит пользователя или маркер доступа к приложению.                            **Примечания**: требуется версия 1.5 или более новое, не допускает значение NULL.            |
|appRoles| [microsoft.graph.appRole](../resources/approle.md) коллекции|Роли приложений, предоставляемые элементом соответствующего приложения. Дополнительные сведения см в определении свойств **appRoles** на сущность приложения **примечания**: требуется версия 1.5 или более новое, не допускает значение NULL.            |
|displayName|Строка|Отображаемое имя участника-службы.|
|errorUrl|Строка|            |
|Домашняя страница|Строка|URL-адрес домашней страницы соответствующего приложения.|
|keyCredentials|microsoft.graph.keyCredential|Коллекция ключей учетные данные, связанные со службой участника.                            **Примечание.** Значение NULL не допускается.            |
|logoutUrl|Строка| Задает URL-адрес, который будет использоваться службой авторизации корпорации Майкрософт для выхода из системы на пользователя, с помощью [канала передний план](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [снова канала](https://openid.net/specs/openid-connect-backchannel-1_0.html) или протоколы выхода SAML. |
|oauth2Permissions|microsoft.graph.oAuth2Permission|Разрешения OAuth 2.0, предоставляемые элементом соответствующего приложения. Дополнительные сведения см в определении свойств **oauth2Permissions** на сущность приложения.                            **Примечания**: требуется версия 1.5 или более новое, не допускает значение NULL.            |
|passwordCredentials|microsoft.graph.passwordCredential|Коллекция пароль учетных данных, связанных с участников-служб.                            **Примечание.** Значение NULL не допускается.            |
|preferredTokenSigningKeyThumbprint|Строка|Зарезервировано для внутреннего пользования. Не записывать или в противном случае использовать это свойство. Могут быть удалены в будущих версиях.                            **Примечания**: требуется версия 1.5 или более поздней версии.            |
|publisherName|String|Отображаемое имя клиента, в котором указаны соответствующего приложения.|
|replyUrls|Строка|URL-адреса, что маркеры пользователей будут отправлены для входа с ним приложении или перенаправления коды авторизации коды URI, OAuth 2.0, и будут отправлены маркеры доступа для соответствующего приложения.                            **Примечание.** Значение NULL не допускается.            |
|samlMetadataUrl|Строка|            |
|servicePrincipalNames|Строка|Коды URI, определение соответствующего приложения. Дополнительные сведения содержатся, [приложения и объекты участников-служб](https://msdn.microsoft.com/library/azure/dn132633.aspx).                            **Примечания**: не допускает значение NULL, **любой** оператор для фильтра выражений на многозначные свойства; Для получения дополнительных сведений см [поддерживается запросов, фильтров и варианты страницы результатов](https://msdn.microsoft.com/library/azure/dn727074.aspx).            |
|tags|String|                                        **Примечание.** Значение null не допускается.            |

## <a name="response"></a>Отклик

Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [servicePrincipal](../resources/serviceprincipal.md) объект в теле ответа.
## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "update_serviceprincipal"
}-->
```http
PATCH https://graph.microsoft.com/beta/servicePrincipals/{id}
Content-type: application/json
Content-length: 391

{
  "accountEnabled": true,
  "addIns": [
    {
      "id": "id-value",
      "type": "type-value",
      "properties": [
        {
          "key": "key-value",
          "value": "value-value"
        }
      ]
    }
  ],
  "appDisplayName": "appDisplayName-value",
  "appId": "appId-value",
  "appOwnerOrganizationId": "appOwnerOrganizationId-value",
  "appRoleAssignmentRequired": true
}
```
##### <a name="response"></a>Отклик
Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 391

{
  "accountEnabled": true,
  "addIns": [
    {
      "id": "id-value",
      "type": "type-value",
      "properties": [
        {
          "key": "key-value",
          "value": "value-value"
        }
      ]
    }
  ],
  "appDisplayName": "appDisplayName-value",
  "appId": "appId-value",
  "appOwnerOrganizationId": "appOwnerOrganizationId-value",
  "appRoleAssignmentRequired": true
}
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
    "Error: /api-reference/beta/api/serviceprincipal-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
