---
title: Обновление serviceprincipal
description: Обновление свойства объекта serviceprincipal.
localization_priority: Normal
ms.openlocfilehash: a562bca03881923cfc21d32eadee2a7f7053fa9b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511662"
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
|accountEnabled|Логическое|                **значение true,** Если включена участника учетной записи службы. в противном случае — **false**.            |
|AppDisplayName|String|Отображаемое имя, предоставляемые элементом соответствующего приложения.|
|appId|String|Уникальный идентификатор для соответствующего приложения (его свойство **appId** ).|
|appRoleAssignmentRequired|Логическое|Указывает, будет ли **appRoleAssignment** пользователю или группе требуется перед Azure AD выпустит пользователя или маркер доступа к приложению.                            **Примечания**: требуется версия 1.5 или более новое, не допускает значение NULL.            |
|appRoles|роли приложения|Роли приложений, предоставляемые элементом соответствующего приложения. Дополнительные сведения см в определении свойств **appRoles** на сущность приложения **примечания**: требуется версия 1.5 или более новое, не допускает значение NULL.            |
|displayName|String|Отображаемое имя участника-службы.|
|errorUrl|String|            |
|HomePage|String|URL-адрес домашней страницы соответствующего приложения.|
|keyCredentials|keyCredential|Коллекция ключей учетные данные, связанные со службой участника.                            **Примечание.** Значение NULL не допускается.            |
|logoutUrl|String| Задает URL-адрес, который будет использоваться службой авторизации корпорации Майкрософт для выхода из системы на пользователя, с помощью [канала передний план](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [снова канала](https://openid.net/specs/openid-connect-backchannel-1_0.html) или протоколы выхода SAML. |
|oauth2Permissions|oAuth2Permission|Разрешения OAuth 2.0, предоставляемые элементом соответствующего приложения. Дополнительные сведения см в определении свойств **oauth2Permissions** на сущность приложения.                            **Примечания**: требуется версия 1.5 или более новое, не допускает значение NULL.            |
|passwordCredentials|passwordCredential|Коллекция пароль учетных данных, связанных с участников-служб.                            **Примечание.** Значение NULL не допускается.            |
|preferredTokenSigningKeyThumbprint|String|Зарезервировано для внутреннего пользования. Не записывать или в противном случае использовать это свойство. Могут быть удалены в будущих версиях.                            **Примечания**: требуется версия 1.5 или более поздней версии.            |
|publisherName|String|Отображаемое имя клиента, в котором указаны соответствующего приложения.|
|replyUrls|String|URL-адреса, что маркеры пользователей будут отправлены для входа с ним приложении или перенаправления коды авторизации коды URI, OAuth 2.0, и будут отправлены маркеры доступа для соответствующего приложения.                            **Примечание.** Значение NULL не допускается.            |
|samlMetadataUrl|String|            |
|servicePrincipalNames|String|Коды URI, определение соответствующего приложения. Дополнительные сведения содержатся, [приложения и объекты участников-служб](https://msdn.microsoft.com/library/azure/dn132633.aspx).                            **Примечания**: не допускает значение NULL, **любой** оператор для фильтра выражений на многозначные свойства; Для получения дополнительных сведений см [поддерживается запросов, фильтров и варианты страницы результатов](https://msdn.microsoft.com/library/azure/dn727074.aspx).            |
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
##### <a name="response"></a>Ответ
Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceprincipal"
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
