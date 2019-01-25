---
title: Настройка синхронизации с расширением атрибутов каталога
description: 'Можно настроить параметры синхронизации схемы для включения атрибутов каталога расширения Azure Active Directory (Azure AD). В этой статье описывается, как использовать атрибут расширения каталога (**extension_9d98asdfl15980a_Nickname**) для заполнения значение User.CommunityNickname в Salesforce. В этом сценарии у вас есть Azure AD подключить настроить для подготовки число атрибуты расширения каталогов Windows Server Active Directory локально для Azure AD. '
localization_priority: Normal
ms.openlocfilehash: 4160a95acfc6b23f5d5a9d880f36d9ca6a1f3362
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523864"
---
# <a name="configure-synchronization-with-directory-extension-attributes"></a>Настройка синхронизации с расширением атрибутов каталога

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Можно настроить параметры синхронизации схемы для включения атрибутов каталога расширения Azure Active Directory (Azure AD). В этой статье описывается, как использовать атрибут расширения каталога (**extension_9d98asdfl15980a_Nickname**) для заполнения значение User.CommunityNickname в Salesforce. В этом сценарии у вас есть Azure AD подключить настроить для подготовки число атрибуты расширения каталогов Windows Server Active Directory локально для Azure AD. 

В этой статье предполагается, что уже содержит приложение, которое поддерживает синхронизацию к клиенту через [Портал Azure](https://portal.azure.com), что вы знаете отображаемое имя приложения и имеют маркер авторизации для Microsoft Graph. Сведения о том, как получить маркер авторизации содержатся [маркеры доступа Get для вызова Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).

## <a name="find-the-service-principal-object-by-display-name"></a>Найдите объект участника службы по отображаемому имени

Следующий пример демонстрирует найдите объект участника службы с отображаемым именем «Изолированной среды Salesforce».

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

`{servicePrincipalId}` — Это `60443998-8cf7-4e61-b05c-a53b658cb5e1`.

## <a name="list-synchronization-jobs-in-the-context-of-the-service-principal"></a>Список заданий синхронизации в контексте участников-служб 

Следующий пример показывает, как получить `jobId` , необходимые для работы с. Как правило ответ возвращается только одно задание.

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

`{jobId}` — Это `SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa`.

## <a name="find-the-name-of-the-directory-extension-attribute-you-need"></a>Найдите имя атрибута расширения каталогов, вы должны

Вам понадобится полное имя атрибута расширения. Если вы не знаете полное имя (который должен выглядеть **extension_9d98asdfl15980a_Nickname**), просмотрите следующие сведения о атрибуты расширения каталогов, а также для их проверки: 

* [Расширение схемы directory Azure AD с помощью настраиваемых свойств](https://azure.microsoft.com/en-us/resources/samples/active-directory-dotnet-graphapi-directoryextensions-web/)
* [Расширения схемы Directory | Основные понятия графике API](https://msdn.microsoft.com/library/azure/ad/graph/howto/azure-ad-graph-api-directory-schema-extensions)


## <a name="get-the-synchronization-schema"></a>Получение схемы синхронизации
Следующем примере показано, как получить схему синхронизации.

<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
```

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости. Будут возвращены все свойства в фактический вызов.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationSchema"
} -->
```http
HTTP/1.1 200 OK

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

## <a name="add-a-definition-for-the-directory-extension-attribute-and-a-mapping-between-the-attributes"></a>Добавьте определение для атрибута расширения каталогов и сопоставление атрибутов

Используйте редактор обычного текста по выбору (например, ["Блокнот" ++](https://notepad-plus-plus.org/) или [Редактора JSON Online](https://www.jsoneditoronline.org/)) для:

1. Добавьте [Определение атрибута](synchronization-attributedefinition.md) для `extension_9d98asdfl15980a_Nickname` атрибут. 

    - В разделе каталоги найти каталог с именем «Azure Active Directory» и найдите один с именем **пользователя**в массив объектов.
    - Добавьте новый атрибут в список, укажите имя и тип, как показано в следующем примере.

2. Добавьте [атрибут сопоставления](synchronization-attributemapping.md) между extension_9d98asdfl15980a_Nickname и CommunityNickname.

    - В разделе [synchronizationRules](synchronization-synchronizationrule.md)найти правило, которое задает в качестве исходного каталога и Salesforce.com как в целевом каталоге Azure AD (`"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"`).
    - Найдите в [objectMappings](synchronization-objectmapping.md) правила сопоставления между пользователями (`"sourceObjectName": "User",   "targetObjectName": "User"`).
    - В массиве [attributeMappings](synchronization-attributemapping.md) **objectMapping**добавьте новую запись, как показано в следующем примере.

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

## <a name="save-the-modified-synchronization-schema"></a>Сохранение измененного синхронизации схемы

При сохранении схемы обновленные синхронизации убедитесь, что включение всей схемы, включая части без изменений. Этот запрос будет заменить существующую схему, предоставленные.

```http
PUT https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
{
    "directories": [],
    "synchronizationRules": []
}

HTTP/1.1 201 No Content
```

Схема была сохранена успешно, в следующей итерации задание синхронизации, начнется повторно обработки всех учетных записей в Azure AD и новые сопоставления будет применяться ко всем подготовленные учетные записи.
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-configure-with-directory-extension-attributes.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
