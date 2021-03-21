---
title: Настройка синхронизации с атрибутами расширения каталога
description: Настройте схему синхронизации, чтобы включить атрибуты расширения каталога Azure Active Directory (Azure AD).
localization_priority: Normal
doc_type: conceptualPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: db5e2ba4bc715f608d17b8e11067df71141a6142
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957004"
---
# <a name="configure-synchronization-with-directory-extension-attributes"></a><span data-ttu-id="3f134-103">Настройка синхронизации с атрибутами расширения каталога</span><span class="sxs-lookup"><span data-stu-id="3f134-103">Configure synchronization with directory extension attributes</span></span>

<span data-ttu-id="3f134-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f134-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f134-105">Можно настроить схему синхронизации, чтобы включить атрибуты расширения каталога Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="3f134-105">You can customize your synchronization schema to include Azure Active Directory (Azure AD) directory extension attributes.</span></span> <span data-ttu-id="3f134-106">В этой статье описывается использование атрибута расширения каталога **(extension_9d98asdfl15980a_Nickname)** для заполнения значения User.CommunityNickname в Salesforce.</span><span class="sxs-lookup"><span data-stu-id="3f134-106">This article describes how to use a directory extension attribute (**extension_9d98asdfl15980a_Nickname**) to populate the value of User.CommunityNickname in Salesforce.</span></span> <span data-ttu-id="3f134-107">В этом сценарии необходимо настроить Azure AD Connect для предоставления ряда атрибутов расширения каталогов от локального Windows Server Active Directory до Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3f134-107">In this scenario, you have Azure AD Connect set up to provision a number of directory extension attributes from Windows Server Active Directory on-premises to Azure AD.</span></span> 

<span data-ttu-id="3f134-108">В этой статье предполагается, что вы уже добавили в клиент приложение, которое поддерживает синхронизацию с клиентом через портал [Azure,](https://portal.azure.com)что вы знаете имя отображения приложения и что у вас есть маркер авторизации для Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="3f134-108">This article assumes that you have already added an application that supports synchronization to your tenant through the [Azure Portal](https://portal.azure.com), that you know the application display name, and that you have an authorization token for Microsoft Graph.</span></span> <span data-ttu-id="3f134-109">Сведения о том, как получить маркер авторизации, см. в записи [Get access tokens to call Microsoft Graph.](/graph/auth/)</span><span class="sxs-lookup"><span data-stu-id="3f134-109">For information about how to get the authorization token, see [Get access tokens to call Microsoft Graph](/graph/auth/).</span></span>

## <a name="find-the-service-principal-object-by-display-name"></a><span data-ttu-id="3f134-110">Поиск основного объекта службы по имени отображения</span><span class="sxs-lookup"><span data-stu-id="3f134-110">Find the service principal object by display name</span></span>

<span data-ttu-id="3f134-111">В следующем примере показано, как найти основной объект службы с отображаемой именем "Песочница Salesforce".</span><span class="sxs-lookup"><span data-stu-id="3f134-111">The following example shows how to find a service principal object with the display name "Salesforce Sandbox".</span></span>

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

<span data-ttu-id="3f134-112">The `{servicePrincipalId}` is `60443998-8cf7-4e61-b05c-a53b658cb5e1` .</span><span class="sxs-lookup"><span data-stu-id="3f134-112">The `{servicePrincipalId}` is `60443998-8cf7-4e61-b05c-a53b658cb5e1`.</span></span>

## <a name="list-synchronization-jobs-in-the-context-of-the-service-principal"></a><span data-ttu-id="3f134-113">Задания синхронизации списков в контексте основного задания службы</span><span class="sxs-lookup"><span data-stu-id="3f134-113">List synchronization jobs in the context of the service principal</span></span> 

<span data-ttu-id="3f134-114">В следующем примере показано, как получить необходимое `jobId` для работы.</span><span class="sxs-lookup"><span data-stu-id="3f134-114">The following example shows you how to get the `jobId` that you need to work with.</span></span> <span data-ttu-id="3f134-115">Как правило, ответ возвращает только одну работу.</span><span class="sxs-lookup"><span data-stu-id="3f134-115">Generally, the response returns only one job.</span></span>

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

<span data-ttu-id="3f134-116">The `{jobId}` is `SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa` .</span><span class="sxs-lookup"><span data-stu-id="3f134-116">The `{jobId}` is `SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa`.</span></span>

## <a name="find-the-name-of-the-directory-extension-attribute-you-need"></a><span data-ttu-id="3f134-117">Найдите имя необходимого атрибута расширения каталога</span><span class="sxs-lookup"><span data-stu-id="3f134-117">Find the name of the directory extension attribute you need</span></span>

<span data-ttu-id="3f134-118">Вам потребуется полное имя атрибута расширения.</span><span class="sxs-lookup"><span data-stu-id="3f134-118">You'll need the full name of the extension attribute.</span></span> <span data-ttu-id="3f134-119">Если вы не знаете полное имя (которое должно выглядеть аналогично **extension_9d98asdfl15980a_Nickname),** см. следующие сведения о атрибутах расширения каталогов и о том, как их проверять:</span><span class="sxs-lookup"><span data-stu-id="3f134-119">If you don't know the full name (which should look similar to **extension_9d98asdfl15980a_Nickname**), see the following information about directory extension attributes and how to inspect them:</span></span> 

* [<span data-ttu-id="3f134-120">Расширение схемы каталога Azure AD с пользовательскими свойствами</span><span class="sxs-lookup"><span data-stu-id="3f134-120">Extending the Azure AD directory schema with custom properties</span></span>](/graph/extensibility-overview)
* [<span data-ttu-id="3f134-121">Расширения схемы каталогов | Концепции API graph</span><span class="sxs-lookup"><span data-stu-id="3f134-121">Directory schema extensions | Graph API concepts</span></span>](/previous-versions/azure/ad/graph/howto/azure-ad-graph-api-directory-schema-extensions)


## <a name="get-the-synchronization-schema"></a><span data-ttu-id="3f134-122">Получить схему синхронизации</span><span class="sxs-lookup"><span data-stu-id="3f134-122">Get the synchronization schema</span></span>
<span data-ttu-id="3f134-123">В следующем примере показано, как получить схему синхронизации.</span><span class="sxs-lookup"><span data-stu-id="3f134-123">The following example shows how to get the synchronization schema.</span></span>


# <a name="http"></a>[<span data-ttu-id="3f134-124">HTTP</span><span class="sxs-lookup"><span data-stu-id="3f134-124">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema_3"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
```
# <a name="c"></a>[<span data-ttu-id="3f134-125">C#</span><span class="sxs-lookup"><span data-stu-id="3f134-125">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationschema-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3f134-126">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3f134-126">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationschema-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3f134-127">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3f134-127">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationschema-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3f134-128">Java</span><span class="sxs-lookup"><span data-stu-id="3f134-128">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-synchronizationschema-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


><span data-ttu-id="3f134-129">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3f134-129">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3f134-130">Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3f134-130">All the properties will be returned in an actual call.</span></span>

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

## <a name="add-a-definition-for-the-directory-extension-attribute-and-a-mapping-between-the-attributes"></a><span data-ttu-id="3f134-131">Добавьте определение атрибута расширения каталога и сопоставление между атрибутами</span><span class="sxs-lookup"><span data-stu-id="3f134-131">Add a definition for the directory extension attribute, and a mapping between the attributes</span></span>

<span data-ttu-id="3f134-132">Используйте обычный текстовый редактор по вашему выбору (например, [Notepad++](https://notepad-plus-plus.org/) или [JSON Editor Online),](https://www.jsoneditoronline.org/)чтобы:</span><span class="sxs-lookup"><span data-stu-id="3f134-132">Use a plain text editor of your choice (for example, [Notepad++](https://notepad-plus-plus.org/) or [JSON Editor Online](https://www.jsoneditoronline.org/)) to:</span></span>

1. <span data-ttu-id="3f134-133">Добавьте определение [атрибута](synchronization-attributedefinition.md) для `extension_9d98asdfl15980a_Nickname` атрибута.</span><span class="sxs-lookup"><span data-stu-id="3f134-133">Add an [attribute definition](synchronization-attributedefinition.md) for the `extension_9d98asdfl15980a_Nickname` attribute.</span></span> 

    - <span data-ttu-id="3f134-134">В каталогах найдите каталог с именем "Azure Active Directory", а в массиве объекта найдите имя **Пользователя.**</span><span class="sxs-lookup"><span data-stu-id="3f134-134">Under directories, find the directory with the name "Azure Active Directory", and in the object's array, find the one named **User**.</span></span>
    - <span data-ttu-id="3f134-135">Добавьте новый атрибут в список, указав имя и тип, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="3f134-135">Add the new attribute to the list, specifying the name and type, as shown in the following example.</span></span>

2. <span data-ttu-id="3f134-136">Добавьте [сопоставление атрибутов](synchronization-attributemapping.md) между extension_9d98asdfl15980a_Nickname и CommunityNickname.</span><span class="sxs-lookup"><span data-stu-id="3f134-136">Add an [attribute mapping](synchronization-attributemapping.md) between extension_9d98asdfl15980a_Nickname and CommunityNickname.</span></span>

    - <span data-ttu-id="3f134-137">В [рамках синхронизацииRules](synchronization-synchronizationrule.md)найдите правило, которое указывает Azure AD как исходный каталог, а Salesforce.com в качестве целевого каталога ( `"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"` ).</span><span class="sxs-lookup"><span data-stu-id="3f134-137">Under [synchronizationRules](synchronization-synchronizationrule.md), find the rule that specifies Azure AD as source directory, and Salesforce.com as the target directory (`"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"`).</span></span>
    - <span data-ttu-id="3f134-138">В [objectMappings правила](synchronization-objectmapping.md) найдите сопоставление между пользователями ( `"sourceObjectName": "User",   "targetObjectName": "User"` ).</span><span class="sxs-lookup"><span data-stu-id="3f134-138">In the [objectMappings](synchronization-objectmapping.md) of the rule, find the mapping between users (`"sourceObjectName": "User",   "targetObjectName": "User"`).</span></span>
    - <span data-ttu-id="3f134-139">В [массиве attributeMappings](synchronization-attributemapping.md) **объектаMapping** добавьте новую запись, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="3f134-139">In the [attributeMappings](synchronization-attributemapping.md) array of the **objectMapping**, add a new entry, as shown in the following example.</span></span>

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

## <a name="save-the-modified-synchronization-schema"></a><span data-ttu-id="3f134-140">Сохранение измененной схемы синхронизации</span><span class="sxs-lookup"><span data-stu-id="3f134-140">Save the modified synchronization schema</span></span>

<span data-ttu-id="3f134-141">При сохранения обновленной схемы синхронизации убедитесь, что в нее включена вся схема, включая неизменененные части.</span><span class="sxs-lookup"><span data-stu-id="3f134-141">When you save the updated synchronization schema, make sure that you include the entire schema, including the unmodified parts.</span></span> <span data-ttu-id="3f134-142">Этот запрос заменит существующую схему на предоставляемую.</span><span class="sxs-lookup"><span data-stu-id="3f134-142">This request will replace the existing schema with the one that you provide.</span></span>

```http
PUT https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
{
    "directories": [],
    "synchronizationRules": []
}

HTTP/1.1 201 No Content
```

<span data-ttu-id="3f134-143">Если схема была успешно сохранена, при следующей итерации задания синхронизации она начнет повторно обрабатывать все учетные записи в Azure AD, и новые сопоставления будут применены для всех учетных записей.</span><span class="sxs-lookup"><span data-stu-id="3f134-143">If the schema was saved successfully, on the next iteration of the synchronization job, it will start re-processing all the accounts in your Azure AD, and the new mappings will be applied to all provisioned accounts.</span></span>
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
