---
title: Настройка синхронизации с атрибутами расширения каталога
description: Настройте схему синхронизации, чтобы Azure Active Directory атрибуты расширения каталога Azure AD.
ms.localizationpriority: medium
doc_type: conceptualPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: b3379502f1bf5354d4f53e863f4924c5f251bd4a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "60976819"
---
# <a name="configure-synchronization-with-directory-extension-attributes"></a>Настройка синхронизации с атрибутами расширения каталога

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Схему синхронизации можно настроить так, чтобы Azure Active Directory атрибуты расширения каталога Azure AD. В этой статье описывается использование атрибута расширения каталога **(extension_9d98asdfl15980a_Nickname)** для заполнения значения User.CommunityNickname в Salesforce. В этом сценарии Подключение Azure AD для предоставления ряда атрибутов расширения каталогов от Windows Server Active Directory локального до Azure AD. 

В этой статье предполагается, что вы уже добавили приложение, поддерживаюное синхронизацию с клиентом через портал [Azure,](https://portal.azure.com)что вы знаете имя отображения приложения и что у вас есть маркер авторизации для Microsoft Graph. Сведения о том, как получить маркер авторизации, см. в сайте [Get access tokens to call Microsoft Graph.](/graph/auth/)

## <a name="find-the-service-principal-object-by-display-name"></a>Поиск основного объекта службы по имени отображения

В следующем примере показано, как найти основной объект службы с отображаемой именем "Песочница Salesforce".

```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=startswith(displayName, 'salesforce')
Authorization: Bearer {Token}
```

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#servicePrincipals(id,appId,displayName)",
    "value": [
    {
        "id": "167e33e9-f80e-490e-b4d8-698d4a80fb3e",
        "appId": "cd3ed3de-93ee-400b-8b19-b61ef44a0f29",
        "displayName": "Salesforce"
    },
    {
        "id": "8cbbb70b-7290-42da-83ee-89fa3517a977",
        "appId": "b0f2e3b1-fe31-4658-b216-44dcaeabb63a",
        "displayName": "salesforce 1"
    },
    {
        "id": "60443998-8cf7-4e61-b05c-a53b658cb5e1",
        "appId": "79079396-c301-405d-900f-e2e0c2439a90",
        "displayName": "Salesforce Sandbox"
    }
    ]
}
```

The `{servicePrincipalId}` is `60443998-8cf7-4e61-b05c-a53b658cb5e1` .

## <a name="list-synchronization-jobs-in-the-context-of-the-service-principal"></a>Задания синхронизации списков в контексте основного задания службы 

В следующем примере показано, как получить необходимое `jobId` для работы. Как правило, ответ возвращает только одну работу.

```http
GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs
Authorization: Bearer {Token}
```

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#servicePrincipals('60443998-8cf7-4e61-b05c-a53b658cb5e1')/synchronization/jobs",
    "value": [
        {
            "id": "SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa",
            "templateId": "SfSandboxOutDelta",
            "schedule": {},
            "status": {}
    }
    ]
}
```

The `{jobId}` is `SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa` .

## <a name="find-the-name-of-the-directory-extension-attribute-you-need"></a>Найдите имя необходимого атрибута расширения каталога

Вам потребуется полное имя атрибута расширения. Если вы не знаете полное имя (которое должно выглядеть аналогично **extension_9d98asdfl15980a_Nickname),** см. следующие сведения о атрибутах расширения каталогов и о том, как их проверять: 

* [Расширение схемы каталога Azure AD с пользовательскими свойствами](/graph/extensibility-overview)
* [Расширения схемы каталогов | Graph API](/previous-versions/azure/ad/graph/howto/azure-ad-graph-api-directory-schema-extensions)


## <a name="get-the-synchronization-schema"></a>Получить схему синхронизации
В следующем примере показано, как получить схему синхронизации.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema_3"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationschema-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationschema-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationschema-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-synchronizationschema-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-synchronizationschema-3-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости. Все свойства будут возвращены при фактическом вызове.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationSchema"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "directories": [
        {
              "id": "66e4a8cc-1b7b-435e-95f8-f06cea133828",
              "name": "Azure Active Directory",
              "objects": [
                {
                    "attributes": [
                        {
                          "anchor": true,
                          "caseExact": false,
                          "defaultValue": null,
                          "metadata": [],
                          "multivalued": false,
                          "mutability": "ReadWrite",
                          "name": "objectId",
                          "required": false,
                          "referencedObjects": [],
                          "type": "String"
                        },
                        {
                          "anchor": false,
                          "caseExact": false,
                          "defaultValue": null,
                          "metadata": [],
                          "multivalued": false,
                          "mutability": "ReadWrite",
                          "name": "streetAddress",
                          "required": false,
                          "referencedObjects": [],
                          "type": "String"
                        }
                    ],
                    "name": "User"
                }
             ]
        },
        {
              "id": "8ffa6169-f354-4751-9b77-9c00765be92d",
              "name": "salesforce.com",
              "objects": []
        }
  ],
 "synchronizationRules": [
        {
          "editable": true,
          "id": "4c5ecfa1-a072-4460-b1c3-4adde3479854",
          "name": "USER_OUTBOUND_USER",
          "objectMappings": [
                {
                    "attributeMappings": [
                            {
                              "defaultValue": "True",
                              "exportMissingReferences": false,
                              "flowBehavior": "FlowWhenChanged",
                              "flowType": "Always",
                              "matchingPriority": 0,
                              "source": {
                                "expression": "Not([IsSoftDeleted])",
                                "name": "Not",
                                "parameters": [
                                  {
                                    "key": "source",
                                    "value": {
                                      "expression": "[IsSoftDeleted]",
                                      "name": "IsSoftDeleted",
                                      "parameters": [],
                                      "type": "Attribute"
                                    }
                                  }
                                ],
                                "type": "Function"
                              },
                              "targetAttributeName": "IsActive"
                            }
                     ],
                    "enabled": true,
                    "flowTypes": "Add, Update, Delete",
                    "name": "Synchronize Azure Active Directory Users to salesforce.com",
                    "scope": null,
                    "sourceObjectName": "User",
                    "targetObjectName": "User"
            }]
        }]
}
```

## <a name="add-a-definition-for-the-directory-extension-attribute-and-a-mapping-between-the-attributes"></a>Добавьте определение атрибута расширения каталога и сопоставление между атрибутами

Используйте обычный текстовый редактор по вашему выбору [(например, Блокнот++](https://notepad-plus-plus.org/) или [редактор JSON Online),](https://www.jsoneditoronline.org/)чтобы:

1. Добавьте определение [атрибута](synchronization-attributedefinition.md) для `extension_9d98asdfl15980a_Nickname` атрибута. 

    - В каталогах найдите каталог с именем "Azure Active Directory", а в массиве объекта найдите имя **Пользователя**.
    - Добавьте новый атрибут в список, указав имя и тип, как показано в следующем примере.

2. Добавьте [сопоставление атрибутов](synchronization-attributemapping.md) между extension_9d98asdfl15980a_Nickname и CommunityNickname.

    - В [рамках синхронизацииRules](synchronization-synchronizationrule.md)найдите правило, которое указывает Azure AD как исходный каталог, а Salesforce.com в качестве целевого каталога ( `"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"` ).
    - В [objectMappings правила](synchronization-objectmapping.md) найдите сопоставление между пользователями ( `"sourceObjectName": "User",   "targetObjectName": "User"` ).
    - В [массиве attributeMappings](synchronization-attributemapping.md) **объектаMapping** добавьте новую запись, как показано в следующем примере.

    ```json
    {
        "directories": [
            {
                "id": "66e4a8cc-1b7b-435e-95f8-f06cea133828",
                "name": "Azure Active Directory",
                "objects": [
                    {
                        "attributes": [
                                ,{
                                "name": "extension_9d98asdfl15980a_Nickname",
                                "type": "String"
                                }
                        ],
                        "name":"User"
                    }]
            }
        ],
        "synchronizationRules": [
            {
            "editable": true,
            "id": "4c5ecfa1-a072-4460-b1c3-4adde3479854",
            "metadata": [..],
            "name": "USER_OUTBOUND_USER",
            "objectMappings": [
                {
                    "attributeMappings": [
                    ,{
                        "source": {
                            "name": "extension_9d98asdfl15980a_Nickname",
                            "type": "Attribute"
                        },
                        "targetAttributeName": "CommunityNickname"
                        }
                ],
                "name": "Synchronize Azure Active Directory Users to salesforce.com",
                    "scope": null,
                    "sourceObjectName": "User",
                    "targetObjectName": "User"
                }
            ],
            "priority": 1,
            "sourceDirectoryName": "Azure Active Directory",
            "targetDirectoryName": "salesforce.com"
            },
        ]
    }
    ```

## <a name="save-the-modified-synchronization-schema"></a>Сохранение измененной схемы синхронизации

При сохранения обновленной схемы синхронизации убедитесь, что в нее включена вся схема, включая неизменененные части. Этот запрос заменит существующую схему на предоставляемую.

```http
PUT https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
{
    "directories": [],
    "synchronizationRules": []
}

HTTP/1.1 201 No Content
```

Если схема была успешно сохранена, при следующей итерации задания синхронизации она начнет повторно обрабатывать все учетные записи в Azure AD, и новые сопоставления будут применены для всех учетных записей.
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get the synchronization schema",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
