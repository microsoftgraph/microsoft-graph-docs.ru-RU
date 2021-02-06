---
title: Настройка синхронизации с атрибутами расширения каталога
description: Настройте схему синхронизации, включив атрибуты расширения каталога Azure Active Directory (Azure AD).
localization_priority: Normal
doc_type: conceptualPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 1a19db23c5797812c41b10ca281efde887da90fc
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131511"
---
# <a name="configure-synchronization-with-directory-extension-attributes"></a><span data-ttu-id="8dc9e-103">Настройка синхронизации с атрибутами расширения каталога</span><span class="sxs-lookup"><span data-stu-id="8dc9e-103">Configure synchronization with directory extension attributes</span></span>

<span data-ttu-id="8dc9e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8dc9e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8dc9e-105">Схему синхронизации можно настроить так, чтобы она включала атрибуты расширения каталога Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="8dc9e-105">You can customize your synchronization schema to include Azure Active Directory (Azure AD) directory extension attributes.</span></span> <span data-ttu-id="8dc9e-106">В этой статье описывается использование атрибута расширения каталога **(extension_9d98asdfl15980a_Nickname)** для заполнения значения User.CommunityNickname в Salesforce.</span><span class="sxs-lookup"><span data-stu-id="8dc9e-106">This article describes how to use a directory extension attribute (**extension_9d98asdfl15980a_Nickname**) to populate the value of User.CommunityNickname in Salesforce.</span></span> <span data-ttu-id="8dc9e-107">В этом сценарии azure AD Connect настроен для предоставления ряда атрибутов расширения каталога из локальной службы Windows Server Active Directory в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8dc9e-107">In this scenario, you have Azure AD Connect set up to provision a number of directory extension attributes from Windows Server Active Directory on-premises to Azure AD.</span></span> 

<span data-ttu-id="8dc9e-108">В этой статье предполагается, что вы уже добавили приложение, которое поддерживает синхронизацию с клиентом с помощью портала [Azure,](https://portal.azure.com)что вы знаете отображаемого имени приложения и у вас есть маркер авторизации для Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="8dc9e-108">This article assumes that you have already added an application that supports synchronization to your tenant through the [Azure Portal](https://portal.azure.com), that you know the application display name, and that you have an authorization token for Microsoft Graph.</span></span> <span data-ttu-id="8dc9e-109">Сведения о том, как получить маркер авторизации, см. в подзапуске маркеров доступа [для вызова Microsoft Graph.](/graph/auth/)</span><span class="sxs-lookup"><span data-stu-id="8dc9e-109">For information about how to get the authorization token, see [Get access tokens to call Microsoft Graph](/graph/auth/).</span></span>

## <a name="find-the-service-principal-object-by-display-name"></a><span data-ttu-id="8dc9e-110">Поиск объекта-службы по отображаемой имени</span><span class="sxs-lookup"><span data-stu-id="8dc9e-110">Find the service principal object by display name</span></span>

<span data-ttu-id="8dc9e-111">В следующем примере показано, как найти объект-службу с отображаемой именем "Песочница Salesforce".</span><span class="sxs-lookup"><span data-stu-id="8dc9e-111">The following example shows how to find a service principal object with the display name "Salesforce Sandbox".</span></span>

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

<span data-ttu-id="8dc9e-112">The `{servicePrincipalId}` is `60443998-8cf7-4e61-b05c-a53b658cb5e1` .</span><span class="sxs-lookup"><span data-stu-id="8dc9e-112">The `{servicePrincipalId}` is `60443998-8cf7-4e61-b05c-a53b658cb5e1`.</span></span>

## <a name="list-synchronization-jobs-in-the-context-of-the-service-principal"></a><span data-ttu-id="8dc9e-113">Список заданий синхронизации в контексте основного службы</span><span class="sxs-lookup"><span data-stu-id="8dc9e-113">List synchronization jobs in the context of the service principal</span></span> 

<span data-ttu-id="8dc9e-114">В следующем примере показано, как получить необходимые `jobId` данные.</span><span class="sxs-lookup"><span data-stu-id="8dc9e-114">The following example shows you how to get the `jobId` that you need to work with.</span></span> <span data-ttu-id="8dc9e-115">Как правило, ответ возвращает только одно задание.</span><span class="sxs-lookup"><span data-stu-id="8dc9e-115">Generally, the response returns only one job.</span></span>

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

<span data-ttu-id="8dc9e-116">The `{jobId}` is `SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa` .</span><span class="sxs-lookup"><span data-stu-id="8dc9e-116">The `{jobId}` is `SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa`.</span></span>

## <a name="find-the-name-of-the-directory-extension-attribute-you-need"></a><span data-ttu-id="8dc9e-117">Найдите нужное имя атрибута расширения каталога</span><span class="sxs-lookup"><span data-stu-id="8dc9e-117">Find the name of the directory extension attribute you need</span></span>

<span data-ttu-id="8dc9e-118">Вам потребуется полное имя атрибута расширения.</span><span class="sxs-lookup"><span data-stu-id="8dc9e-118">You'll need the full name of the extension attribute.</span></span> <span data-ttu-id="8dc9e-119">Если вы не знаете полное имя (которое должно выглядеть примерно так же, как **extension_9d98asdfl15980a_Nickname),** см. следующие сведения об атрибутах расширения каталога и о том, как их проверить:</span><span class="sxs-lookup"><span data-stu-id="8dc9e-119">If you don't know the full name (which should look similar to **extension_9d98asdfl15980a_Nickname**), see the following information about directory extension attributes and how to inspect them:</span></span> 

* [<span data-ttu-id="8dc9e-120">Расширение схемы каталога Azure AD с помощью настраиваемой свойства</span><span class="sxs-lookup"><span data-stu-id="8dc9e-120">Extending the Azure AD directory schema with custom properties</span></span>](/graph/extensibility-overview)
* [<span data-ttu-id="8dc9e-121">Расширения схемы каталогов | Концепции API Graph</span><span class="sxs-lookup"><span data-stu-id="8dc9e-121">Directory schema extensions | Graph API concepts</span></span>](/previous-versions/azure/ad/graph/howto/azure-ad-graph-api-directory-schema-extensions)


## <a name="get-the-synchronization-schema"></a><span data-ttu-id="8dc9e-122">Получить схему синхронизации</span><span class="sxs-lookup"><span data-stu-id="8dc9e-122">Get the synchronization schema</span></span>
<span data-ttu-id="8dc9e-123">В следующем примере показано, как получить схему синхронизации.</span><span class="sxs-lookup"><span data-stu-id="8dc9e-123">The following example shows how to get the synchronization schema.</span></span>


# <a name="http"></a>[<span data-ttu-id="8dc9e-124">HTTP</span><span class="sxs-lookup"><span data-stu-id="8dc9e-124">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
```
# <a name="c"></a>[<span data-ttu-id="8dc9e-125">C#</span><span class="sxs-lookup"><span data-stu-id="8dc9e-125">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationschema-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8dc9e-126">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8dc9e-126">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationschema-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8dc9e-127">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8dc9e-127">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationschema-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8dc9e-128">Java</span><span class="sxs-lookup"><span data-stu-id="8dc9e-128">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-synchronizationschema-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


><span data-ttu-id="8dc9e-129">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8dc9e-129">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8dc9e-130">Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8dc9e-130">All the properties will be returned in an actual call.</span></span>

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

## <a name="add-a-definition-for-the-directory-extension-attribute-and-a-mapping-between-the-attributes"></a><span data-ttu-id="8dc9e-131">Добавление определения для атрибута расширения каталога и сопоставления между атрибутами</span><span class="sxs-lookup"><span data-stu-id="8dc9e-131">Add a definition for the directory extension attribute, and a mapping between the attributes</span></span>

<span data-ttu-id="8dc9e-132">Используйте обычный текстовый редактор (например, [Блокнот++](https://notepad-plus-plus.org/) или [JSON Editor Online),](https://www.jsoneditoronline.org/)чтобы:</span><span class="sxs-lookup"><span data-stu-id="8dc9e-132">Use a plain text editor of your choice (for example, [Notepad++](https://notepad-plus-plus.org/) or [JSON Editor Online](https://www.jsoneditoronline.org/)) to:</span></span>

1. <span data-ttu-id="8dc9e-133">Добавьте определение [атрибута](synchronization-attributedefinition.md) `extension_9d98asdfl15980a_Nickname` для атрибута.</span><span class="sxs-lookup"><span data-stu-id="8dc9e-133">Add an [attribute definition](synchronization-attributedefinition.md) for the `extension_9d98asdfl15980a_Nickname` attribute.</span></span> 

    - <span data-ttu-id="8dc9e-134">В каталогах найдите каталог с именем "Azure Active Directory", а в массиве объекта найдите каталог с именем **User.**</span><span class="sxs-lookup"><span data-stu-id="8dc9e-134">Under directories, find the directory with the name "Azure Active Directory", and in the object's array, find the one named **User**.</span></span>
    - <span data-ttu-id="8dc9e-135">Добавьте новый атрибут в список, указав имя и тип, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="8dc9e-135">Add the new attribute to the list, specifying the name and type, as shown in the following example.</span></span>

2. <span data-ttu-id="8dc9e-136">Добавьте [сопоставление атрибутов](synchronization-attributemapping.md) между extension_9d98asdfl15980a_Nickname и CommunityNickname.</span><span class="sxs-lookup"><span data-stu-id="8dc9e-136">Add an [attribute mapping](synchronization-attributemapping.md) between extension_9d98asdfl15980a_Nickname and CommunityNickname.</span></span>

    - <span data-ttu-id="8dc9e-137">В [synchronizationRules](synchronization-synchronizationrule.md)найдите правило, которое указывает Azure AD как исходный каталог, и Salesforce.com в качестве целевого каталога ( `"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"` ).</span><span class="sxs-lookup"><span data-stu-id="8dc9e-137">Under [synchronizationRules](synchronization-synchronizationrule.md), find the rule that specifies Azure AD as source directory, and Salesforce.com as the target directory (`"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"`).</span></span>
    - <span data-ttu-id="8dc9e-138">В [объектахmappings](synchronization-objectmapping.md) правила найдите сопоставление между пользователями ( `"sourceObjectName": "User",   "targetObjectName": "User"` ).</span><span class="sxs-lookup"><span data-stu-id="8dc9e-138">In the [objectMappings](synchronization-objectmapping.md) of the rule, find the mapping between users (`"sourceObjectName": "User",   "targetObjectName": "User"`).</span></span>
    - <span data-ttu-id="8dc9e-139">В массив [attributeMappings](synchronization-attributemapping.md) **объектаMapping** добавьте новую запись, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="8dc9e-139">In the [attributeMappings](synchronization-attributemapping.md) array of the **objectMapping**, add a new entry, as shown in the following example.</span></span>

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

## <a name="save-the-modified-synchronization-schema"></a><span data-ttu-id="8dc9e-140">Сохранение измененной схемы синхронизации</span><span class="sxs-lookup"><span data-stu-id="8dc9e-140">Save the modified synchronization schema</span></span>

<span data-ttu-id="8dc9e-141">При экономии обновленной схемы синхронизации убедитесь, что включена вся схема, включая неизмененые части.</span><span class="sxs-lookup"><span data-stu-id="8dc9e-141">When you save the updated synchronization schema, make sure that you include the entire schema, including the unmodified parts.</span></span> <span data-ttu-id="8dc9e-142">Этот запрос заменит существующую схему на предоставляемую.</span><span class="sxs-lookup"><span data-stu-id="8dc9e-142">This request will replace the existing schema with the one that you provide.</span></span>

```http
PUT https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
{
    "directories": [],
    "synchronizationRules": []
}

HTTP/1.1 201 No Content
```

<span data-ttu-id="8dc9e-143">Если схема успешно сохранена, при следующей итерации задания синхронизации она начнет повторно обрабатывать все учетные записи в Azure AD, и новые сопоставления будут применены для всех учетных записей, которые были готовы.</span><span class="sxs-lookup"><span data-stu-id="8dc9e-143">If the schema was saved successfully, on the next iteration of the synchronization job, it will start re-processing all the accounts in your Azure AD, and the new mappings will be applied to all provisioned accounts.</span></span>
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
