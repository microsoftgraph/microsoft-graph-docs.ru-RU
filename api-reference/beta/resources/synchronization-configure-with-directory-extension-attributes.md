---
title: Настройка синхронизации с атрибутами расширения каталога
description: 'Вы можете настроить схему синхронизации, включив в нее атрибуты расширения каталога Azure Active Directory (Azure AD). В этой статье описывается, как использовать атрибут расширения каталога (**extension_9d98asdfl15980a_Nickname**) для заполнения значения User. Коммунитиниккнаме в Salesforce. В этом сценарии у вас есть Azure AD Connect, настроенный на подготовку ряда атрибутов расширения каталогов из локальной среды Windows Server Active Directory в Azure AD. '
localization_priority: Normal
ms.openlocfilehash: 439d70ff4e42513b465b80719be34989c97a810d
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33620952"
---
# <a name="configure-synchronization-with-directory-extension-attributes"></a>Настройка синхронизации с атрибутами расширения каталога

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вы можете настроить схему синхронизации, включив в нее атрибуты расширения каталога Azure Active Directory (Azure AD). В этой статье описывается, как использовать атрибут расширения каталога (**extension_9d98asdfl15980a_Nickname**) для заполнения значения User. Коммунитиниккнаме в Salesforce. В этом сценарии у вас есть Azure AD Connect, настроенный на подготовку ряда атрибутов расширения каталогов из локальной среды Windows Server Active Directory в Azure AD. 

В этой статье предполагается, что вы уже добавили приложение, которое поддерживает синхронизацию с клиентом с помощью [портала Azure](https://portal.azure.com), вы знаете отображаемое имя приложения, и у вас есть маркер авторизации для Microsoft Graph. Сведения о том, как получить маркер авторизации, можно найти [в статье получение маркеров доступа для вызова Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).

## <a name="find-the-service-principal-object-by-display-name"></a>Поиск объекта субъекта службы по отображаемому имени

В приведенном ниже примере показано, как найти объект участника службы с отображаемым именем "песочницы Salesforce".

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

Параметр `{servicePrincipalId}` имеет `60443998-8cf7-4e61-b05c-a53b658cb5e1`значение.

## <a name="list-synchronization-jobs-in-the-context-of-the-service-principal"></a>Перечисление заданий синхронизации в контексте субъекта-службы 

В приведенном ниже примере показано `jobId` , как получить сведения о том, что необходимо для работы. Как правило, ответ возвращает только одно задание.

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

Параметр `{jobId}` имеет `SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa`значение.

## <a name="find-the-name-of-the-directory-extension-attribute-you-need"></a>Найдите имя необходимого атрибута расширения каталога

Вам потребуется полное имя атрибута расширения. Если полное имя (которое должно выглядеть аналогично **extension_9d98asdfl15980a_Nickname**), ознакомьтесь со следующими сведениями о атрибутах расширения каталогов и способах их проверки: 

* [Расширение схемы каталога Azure AD с помощью настраиваемых свойств](https://azure.microsoft.com/en-us/resources/samples/active-directory-dotnet-graphapi-directoryextensions-web/)
* [Расширения схемы каталогов | Основные понятия API Graph](https://msdn.microsoft.com/library/azure/ad/graph/howto/azure-ad-graph-api-directory-schema-extensions)


## <a name="get-the-synchronization-schema"></a>Получение схемы синхронизации
В приведенном ниже примере показано, как получить схему синхронизации.

<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
```

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

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
#### <a name="sdk-sample-code"></a>Пример кода для SDK
# <a name="ctabcs"></a>[Языках](#tab/cs)
[!INCLUDE [sample-code](../includes/get_synchronizationschema-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Язык](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_synchronizationschema-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="add-a-definition-for-the-directory-extension-attribute-and-a-mapping-between-the-attributes"></a>Добавление определения атрибута расширения каталога и сопоставления между атрибутами

Используйте простой текстовый редактор (например, [Notepad + +](https://notepad-plus-plus.org/) или [Редактор JSON Online](https://www.jsoneditoronline.org/)), чтобы:

1. Добавьте `extension_9d98asdfl15980a_Nickname` [Определение атрибута](synchronization-attributedefinition.md) . 

    - В разделе Каталоги найдите каталог с именем "Azure Active Directory" и в массиве объекта найдите одного пользователя с именем **User**.
    - Добавьте новый атрибут в список, указав имя и тип, как показано в следующем примере.

2. Добавьте [сопоставление атрибутов](synchronization-attributemapping.md) между Extension_9d98asdfl15980a_Nickname и коммунитиниккнаме.

    - В разделе [синчронизатионрулес](synchronization-synchronizationrule.md)найдите правило, задающее Azure AD в качестве исходного каталога, и Salesforce.com в качестве целевого каталога`"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"`().
    - В [обжектмаппингс](synchronization-objectmapping.md) правила найдите сопоставление между пользователями (`"sourceObjectName": "User",   "targetObjectName": "User"`).
    - В массиве [аттрибутемаппингс](synchronization-attributemapping.md) объекта **обжектмаппинг**добавьте новую запись, как показано в следующем примере.

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

При сохранении обновленной схемы синхронизации убедитесь, что включается вся схема, включая неизмененные части. Этот запрос заменит существующую схему на предоставленную вами.

```http
PUT https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
{
    "directories": [],
    "synchronizationRules": []
}

HTTP/1.1 201 No Content
```

Если схема была успешно сохранена, в следующей итерации задания синхронизации начнется повторная обработка всех учетных записей в Azure AD, а новые сопоставления будут применены ко всем подготовленным учетным записям.
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get the synchronization schema",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-configure-with-directory-extension-attributes.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/resources/synchronization-configure-with-directory-extension-attributes.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
