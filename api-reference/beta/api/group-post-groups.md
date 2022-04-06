---
title: Создание группы
description: Создание группы Microsoft 365 или группы безопасности.
author: psaffaie
ms.localizationpriority: high
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 346c19c28e9e30b196c87b9fdca48d50e9e7bd01
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64587149"
---
# <a name="create-group"></a>Создание группы

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте новую [группу](../resources/group.md) согласно инструкциям в тексте запроса. Можно создать одну из следующих групп.

- Группа Microsoft 365 (единая группа)
- Группа безопасности

Эта операция по умолчанию возвращает только подмножество свойств для каждой группы. Эти свойства по умолчанию указаны в разделе [Свойства](../resources/group.md#properties). Чтобы получить свойства, которые _не_ возвращаются по умолчанию, выполните [операцию GET](group-get.md) и укажите их в параметре запроса OData `$select`.

**Примечание.** Чтобы создать [команду](../resources/team.md), сначала создайте группу и добавьте команду в нее, см. раздел [Создание команды](../api/team-put-teams.md).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий)                |
| :------------------------------------- | :--------------------------------------------------------- |
| Делегированные (рабочая или учебная учетная запись)     | Group.ReadWrite.All, Directory.ReadWrite.All               |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                                             |
| Приложение                            | Group.Create, Group.ReadWrite.All, Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /groups
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание               |
| :------------ | :------------------------ |
| Авторизация | Bearer {token}. Обязательный. |

## <a name="request-body"></a>Текст запроса

В тексте запроса предоставьте описание объекта [group](../resources/group.md) в формате JSON.

В приведенной ниже таблице указаны свойства, необходимые при создании объекта [group](../resources/group.md). При необходимости укажите другие записываемые свойства для своей группы.

| Свойство        | Тип    | Описание                                                                                                                                                                                                                                                                                                                                |
| :-------------- | :------ | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| displayName     | string  | Имя, которое следует отобразить в адресной книге для группы. Максимальная длина: 256 символов. Обязательно.                                                                                                                                                                                                                                         |
| mailEnabled     | boolean | Установите значение `true` для групп с включенной поддержкой почты. Обязательное поле.                                                                                                                                                                                                                                                                                           |
| mailNickname    | string  | Почтовый псевдоним для группы, уникальный для групп Microsoft 365 в организации. Максимальная длина: 64 символа. Это свойство может содержать только символы из [набора символов ASCII от 0 до 127](/office/vba/language/reference/user-interface-help/character-set-0127), за исключением следующих: ` @ () \ [] " ; : . <> , SPACE`. Обязательный. |
| securityEnabled | boolean | Установите значение `true` для групп с поддержкой безопасности, включая группы Microsoft 365. Обязательно. **Примечание.** В группах, созданных с помощью портала Microsoft Azure, для свойства **securityEnabled** всегда устанавливается значение `true`.                                                                                                                                    |

> [!IMPORTANT]
>
> - Создание группы с помощью разрешения приложения **Group.Create** без указания владельцев анонимно создает группу, которая не будет изменяться. Добавьте владельцев в группу при ее создании, чтобы указать владельцев, которые могут изменять группу.
>
> - Создание группы Microsoft 365 программным путем с контекстом только для приложений, а также без указания владельцев будет анонимным. Это может привести к тому, что связанный с ней сайт SharePoint Online не будет создан автоматически, пока дальнейшие действия не будут выполнены вручную.
>
> - Следующие свойства невозможно настроить в исходном запросе POST и необходимо настраивать в последующем запросе PATCH: **allowExternalSenders**, **autoSubscribeNewMembers**, **hideFromAddressLists**, **hideFromOutlookClients**, **isSubscribedByMail**, **unseenCount**.

Так как ресурс **group** поддерживает [расширения](/graph/extensibility-overview), вы можете добавлять настраиваемые свойства с собственными данными к группе при ее создании.

### <a name="grouptypes-options"></a>Параметры groupTypes

Свойство **groupTypes** используется для управления типом группы и участием в ней, как показано ниже.

| Тип группы                     | Назначенное участие | Динамическое членство                |
| :-------------------------------- | :------------------ | :-------------------------------- |
| Microsoft 365 (как единая группа) | `["Unified"]`       | `["Unified","DynamicMembership"]` |
| Динамический                           | `[]` (_null_)       | `["DynamicMembership"]`           |

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [group](../resources/group.md) в теле отклика. Отклик включает в себя только свойства по умолчанию для группы.

## <a name="examples"></a>Примеры

### <a name="example-1-create-a-microsoft-365-group"></a>Пример 1. Создание группы Microsoft 365

В следующем примере создается группа Microsoft 365. Так как владельцы не указаны, вызывающий пользователь автоматически добавляется в качестве владельца группы.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "create_group"
}-->

```http
POST https://graph.microsoft.com/beta/groups
Content-type: application/json

{
  "description": "Self help community for golf",
  "displayName": "Golf Assist",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "golfassist",
  "securityEnabled": false
}
```

# <a name="c"></a>[C#](#tab/csharp)

[!INCLUDE [sample-code](../includes/snippets/csharp/create-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)

[!INCLUDE [sample-code](../includes/snippets/javascript/create-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)

[!INCLUDE [sample-code](../includes/snippets/objc/create-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](../includes/snippets/java/create-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)

[!INCLUDE [sample-code](../includes/snippets/go/create-group-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)

[!INCLUDE [sample-code](../includes/snippets/powershell/create-group-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Отклик

Ниже приведен пример отклика. Значение свойства **preferredDataLocation** наследуется от предпочтительного расположения данных создателя группы.

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "create_group"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
   "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups/$entity",
     "id": "45b7d2e7-b882-4a80-ba97-10b7a63b8fa4",
     "deletedDateTime": null,
     "classification": null,
     "createdDateTime": "2018-12-22T02:21:05Z",
     "description": "Self help community for golf",
     "displayName": "Golf Assist",
     "expirationDateTime": null,
     "groupTypes": [
         "Unified"
     ],
   "isAssignableToRole": null,
     "mail": "golfassist@contoso.com",
     "mailEnabled": true,
     "mailNickname": "golfassist",
     "membershipRule": null,
     "membershipRuleProcessingState": null,
     "onPremisesLastSyncDateTime": null,
     "onPremisesSecurityIdentifier": null,
     "onPremisesSyncEnabled": null,
     "preferredDataLocation": "CAN",
     "preferredLanguage": null,
     "proxyAddresses": [
         "SMTP:golfassist@contoso.onmicrosoft.com"
     ],
     "renewedDateTime": "2018-12-22T02:21:05Z",
     "resourceBehaviorOptions": [],
     "resourceProvisioningOptions": [],
     "securityEnabled": false,
   "securityIdentifier": "S-1-12-1-1753967289-1089268234-832641959-555555555",
     "theme": null,
     "visibility": "Public",
     "onPremisesProvisioningErrors": []
}
```

### <a name="example-2-create-a-security-group-with-an-owner-and-members"></a>Пример 2. Создание группы безопасности с владельцем и участниками

В следующем примере создается группа безопасности с указанным владельцем и участниками. Обратите внимание на то, что в рамках создания группы можно добавить не более 20 отношений, например владельцев и участников. Позже вы можете добавить дополнительных участников с помощью API [добавления участников](/graph/api/group-post-members?view=graph-rest-beta&preserve-view=true) или пакетной обработки JSON.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "create_prepopulated_group"
}-->

```http
POST https://graph.microsoft.com/beta/groups
Content-Type: application/json

{
  "description": "Group with designated owner and members",
  "displayName": "Operations group",
  "groupTypes": [
  ],
  "mailEnabled": false,
  "mailNickname": "operations2019",
  "securityEnabled": true,
  "owners@odata.bind": [
    "https://graph.microsoft.com/beta/users/26be1845-4119-4801-a799-aea79d09f1a2"
  ],
  "members@odata.bind": [
    "https://graph.microsoft.com/beta/users/ff7cb387-6688-423c-8188-3da9532a73cc",
    "https://graph.microsoft.com/beta/users/69456242-0067-49d3-ba96-9de6f2728e14"
  ]
}
```

#### <a name="response"></a>Отклик

Ниже представлен пример успешного отклика. Он включает только свойства по умолчанию. Вы можете получить свойства навигации **owners** или **members** группы, чтобы проверить владельца или участников. Значение свойства **preferredDataLocation** наследуется от предпочтительного расположения данных создателя группы.

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "create_prepopulated_group"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups/$entity",
    "@odata.id": "https://graph.microsoft.com/v2/84841066-274d-4ec0-a5c1-276be684bdd3/directoryObjects/1226170d-83d5-49b8-99ab-d1ab3d91333e/Microsoft.DirectoryServices.Group",
    "id": "1226170d-83d5-49b8-99ab-d1ab3d91333e",
    "deletedDateTime": null,
    "classification": null,
    "createdDateTime": "2021-09-21T07:14:44Z",
    "createdByAppId": "de8bc8b5-d9f9-48b1-a8ad-b748da725064",
    "organizationId": "84841066-274d-4ec0-a5c1-276be684bdd3",
    "description": "Group with designated owner and members",
    "displayName": "Operations group",
    "expirationDateTime": null,
    "groupTypes": [],
    "infoCatalogs": [],
    "isAssignableToRole": null,
    "isManagementRestricted": null,
    "mail": null,
    "mailEnabled": false,
    "mailNickname": "operations2019",
    "membershipRule": null,
    "membershipRuleProcessingState": null,
    "onPremisesDomainName": null,
    "onPremisesLastSyncDateTime": null,
    "onPremisesNetBiosName": null,
    "onPremisesSamAccountName": null,
    "onPremisesSecurityIdentifier": null,
    "onPremisesSyncEnabled": null,
    "preferredDataLocation": null,
    "preferredLanguage": null,
    "proxyAddresses": [],
    "renewedDateTime": "2021-09-21T07:14:44Z",
    "resourceBehaviorOptions": [],
    "resourceProvisioningOptions": [],
    "securityEnabled": true,
    "securityIdentifier": "S-1-12-1-304486157-1236829141-2882644889-1043566909",
    "theme": null,
    "visibility": null,
    "writebackConfiguration": {
        "isEnabled": null,
        "onPremisesGroupType": null
    },
    "onPremisesProvisioningErrors": []
}
```

### <a name="example-3-create-a-microsoft-365-group-that-can-be-assigned-to-an-azure-ad-role"></a>Пример 3. Создание группы Microsoft 365, которую можно назначить роли Azure AD

#### <a name="request"></a>Запрос

Далее приведен пример запроса. Вызывающему пользователю или приложению должно быть назначено разрешение _RoleManagement.ReadWrite.Directory_ для настройки свойства **isAssignableToRole** или обновления участников таких групп.

**ПРИМЕЧАНИЕ.** Группа, свойству **isAssignableToRole** которой присвоено значение `true`, не может относиться к типу с динамическим членством. Дополнительные сведения см. в статье [Использование группы для управления назначениями ролей Azure AD](https://go.microsoft.com/fwlink/?linkid=2103037).

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "create_role_enabled_group"
}-->

```http
POST https://graph.microsoft.com/beta/groups
Content-Type: application/json

{
    "description": "Group assignable to a role",
    "displayName": "Role assignable group",
    "groupTypes": [
        "Unified"
    ],
    "isAssignableToRole": true,
    "mailEnabled": true,
    "securityEnabled": true,
    "mailNickname": "contosohelpdeskadministrators",
    "owners@odata.bind": [
        "https://graph.microsoft.com/beta/users/99e44b05-c10b-4e95-a523-e2732bbaba1e"
    ],
    "members@odata.bind": [
        "https://graph.microsoft.com/beta/users/6ea91a8d-e32e-41a1-b7bd-d2d185eed0e0",
        "https://graph.microsoft.com/beta/users/4562bcc8-c436-4f95-b7c0-4f8ce89dca5e"
    ]
}
```

# <a name="c"></a>[C#](#tab/csharp)

[!INCLUDE [sample-code](../includes/snippets/csharp/create-role-enabled-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)

[!INCLUDE [sample-code](../includes/snippets/javascript/create-role-enabled-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)

[!INCLUDE [sample-code](../includes/snippets/objc/create-role-enabled-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](../includes/snippets/java/create-role-enabled-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)

[!INCLUDE [sample-code](../includes/snippets/go/create-role-enabled-group-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)

[!INCLUDE [sample-code](../includes/snippets/powershell/create-role-enabled-group-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Отклик

Ниже приведен пример отклика. Значение свойства **preferredDataLocation** наследуется от предпочтительного расположения данных создателя группы.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "create_role_enabled_group"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups/$entity",
    "@odata.id": "https://graph.microsoft.com/v2/84841066-274d-4ec0-a5c1-276be684bdd3/directoryObjects/1afc3ca3-b14d-43af-9c70-8ae3a5065454/Microsoft.DirectoryServices.Group",
    "id": "1afc3ca3-b14d-43af-9c70-8ae3a5065454",
    "deletedDateTime": null,
    "classification": null,
    "createdDateTime": "2021-09-21T07:16:21Z",
    "createdByAppId": "de8bc8b5-d9f9-48b1-a8ad-b748da725064",
    "organizationId": "84841066-274d-4ec0-a5c1-276be684bdd3",
    "description": "Group assignable to a role",
    "displayName": "Role assignable group",
    "expirationDateTime": null,
    "groupTypes": [
        "Unified"
    ],
    "infoCatalogs": [],
    "isAssignableToRole": true,
    "isManagementRestricted": null,
    "mail": "contosohelpdeskadministrators@Contoso.com",
    "mailEnabled": true,
    "mailNickname": "contosohelpdeskadministrators",
    "membershipRule": null,
    "membershipRuleProcessingState": null,
    "onPremisesDomainName": null,
    "onPremisesLastSyncDateTime": null,
    "onPremisesNetBiosName": null,
    "onPremisesSamAccountName": null,
    "onPremisesSecurityIdentifier": null,
    "onPremisesSyncEnabled": null,
    "preferredDataLocation": "EU",
    "preferredLanguage": null,
    "proxyAddresses": [
        "SMTP:contosohelpdeskadministrators@Contoso.com"
    ],
    "renewedDateTime": "2021-09-21T07:16:21Z",
    "resourceBehaviorOptions": [],
    "resourceProvisioningOptions": [],
    "securityEnabled": true,
    "securityIdentifier": "S-1-12-1-452738211-1135587661-3817500828-1414792869",
    "theme": null,
    "visibility": "Private",
    "writebackConfiguration": {
        "isEnabled": null,
        "onPremisesGroupType": null
    },
    "onPremisesProvisioningErrors": []
}
```

## <a name="see-also"></a>См. также

- [Добавление пользовательских данных в ресурсы с помощью расширений](/graph/extensibility-overview)
- [Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)](/graph/extensibility-open-users)
- [Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
