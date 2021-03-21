---
title: Настройка синхронизации с настраиваемых целевых атрибутов
description: Настройте схему синхронизации, чтобы включить настраиваемые атрибуты, определенные в целевом каталоге.
localization_priority: Normal
doc_type: conceptualPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 865cde06cded24f9f2920e63535e037a2b477330
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956913"
---
# <a name="configure-synchronization-with-custom-target-attributes"></a><span data-ttu-id="2bcd2-103">Настройка синхронизации с настраиваемых целевых атрибутов</span><span class="sxs-lookup"><span data-stu-id="2bcd2-103">Configure synchronization with custom target attributes</span></span>

<span data-ttu-id="2bcd2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2bcd2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2bcd2-105">Можно настроить схему синхронизации, чтобы включить настраиваемые атрибуты, определенные в целевом каталоге.</span><span class="sxs-lookup"><span data-stu-id="2bcd2-105">You can customize your synchronization schema to include custom attributes that are defined in the target directory.</span></span> <span data-ttu-id="2bcd2-106">В этой статье описывается настройка подписки Salesforce путем добавления нового поля под названием `officeCode` .</span><span class="sxs-lookup"><span data-stu-id="2bcd2-106">This article describes how to customize a Salesforce subscription by adding a new field called `officeCode`.</span></span> <span data-ttu-id="2bcd2-107">Вы настроили синхронизацию из Azure Active Directory (Azure AD) в Salesforce, и для каждого пользователя поле Salesforce будет заполнено значением из поля `officeCode` `extensionAttribute10` Azure AD.</span><span class="sxs-lookup"><span data-stu-id="2bcd2-107">You set up synchronization from Azure Active Directory (Azure AD) to Salesforce, and for each user, you will populate the `officeCode` field in Salesforce with the value from the `extensionAttribute10` field in Azure AD.</span></span>

<span data-ttu-id="2bcd2-108">В этой статье предполагается, что вы уже добавили в клиент приложение, которое поддерживает синхронизацию с клиентом через портал [Azure,](https://portal.azure.com)что вы знаете имя отображения приложения и что у вас есть маркер авторизации для Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2bcd2-108">This article assumes that you have already added an application that supports synchronization to your tenant through the [Azure Portal](https://portal.azure.com), that you know the application display name, and that you have an authorization token for Microsoft Graph.</span></span> <span data-ttu-id="2bcd2-109">Сведения о том, как получить маркер авторизации, см. в записи [Get access tokens to call Microsoft Graph.](/graph/auth/)</span><span class="sxs-lookup"><span data-stu-id="2bcd2-109">For information about how to get the authorization token, see [Get access tokens to call Microsoft Graph](/graph/auth/).</span></span>

## <a name="find-the-service-principal-object-by-display-name"></a><span data-ttu-id="2bcd2-110">Поиск основного объекта службы по имени отображения</span><span class="sxs-lookup"><span data-stu-id="2bcd2-110">Find the service principal object by display name</span></span>

<span data-ttu-id="2bcd2-111">В следующем примере показано, как найти основной объект службы с отображаемой именем Salesforce.</span><span class="sxs-lookup"><span data-stu-id="2bcd2-111">The following example shows how to find a service principal object with the display name Salesforce.</span></span>

```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=startswith(displayName, 'salesforce')
Authorization: Bearer {Token}

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

<span data-ttu-id="2bcd2-112">The `{servicePrincipalId}` is `167e33e9-f80e-490e-b4d8-698d4a80fb3e` .</span><span class="sxs-lookup"><span data-stu-id="2bcd2-112">The `{servicePrincipalId}` is `167e33e9-f80e-490e-b4d8-698d4a80fb3e`.</span></span>


## <a name="list-synchronization-jobs-in-the-context-of-the-service-principal"></a><span data-ttu-id="2bcd2-113">Задания синхронизации списков в контексте основного задания службы</span><span class="sxs-lookup"><span data-stu-id="2bcd2-113">List synchronization jobs in the context of the service principal</span></span> 

<span data-ttu-id="2bcd2-114">В следующем примере показано, как получить необходимое `jobId` для работы.</span><span class="sxs-lookup"><span data-stu-id="2bcd2-114">The following example shows you how to get the `jobId` that you need to work with.</span></span> <span data-ttu-id="2bcd2-115">Как правило, ответ возвращает только одну работу.</span><span class="sxs-lookup"><span data-stu-id="2bcd2-115">Generally, the response returns only one job.</span></span>

```http
GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs
Authorization: Bearer {Token}

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

<span data-ttu-id="2bcd2-116">The `{jobId}` is `SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa` .</span><span class="sxs-lookup"><span data-stu-id="2bcd2-116">The `{jobId}` is `SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa`.</span></span>


## <a name="get-the-synchronization-schema"></a><span data-ttu-id="2bcd2-117">Получить схему синхронизации</span><span class="sxs-lookup"><span data-stu-id="2bcd2-117">Get the synchronization schema</span></span>
<span data-ttu-id="2bcd2-118">В следующем примере показано, как получить схему синхронизации.</span><span class="sxs-lookup"><span data-stu-id="2bcd2-118">The following example shows how to get the synchronization schema.</span></span>


# <a name="http"></a>[<span data-ttu-id="2bcd2-119">HTTP</span><span class="sxs-lookup"><span data-stu-id="2bcd2-119">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
```
# <a name="c"></a>[<span data-ttu-id="2bcd2-120">C#</span><span class="sxs-lookup"><span data-stu-id="2bcd2-120">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationschema-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2bcd2-121">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2bcd2-121">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationschema-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2bcd2-122">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2bcd2-122">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationschema-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2bcd2-123">Java</span><span class="sxs-lookup"><span data-stu-id="2bcd2-123">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-synchronizationschema-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


><span data-ttu-id="2bcd2-124">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2bcd2-124">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2bcd2-125">Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2bcd2-125">All the properties will be returned in an actual call.</span></span>

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

## <a name="add-a-definition-for-the-officecode-attribute-and-a-mapping-between-attributes"></a><span data-ttu-id="2bcd2-126">Добавление определения атрибута OfficeCode и сопоставления между атрибутами</span><span class="sxs-lookup"><span data-stu-id="2bcd2-126">Add a definition for the officeCode attribute and a mapping between attributes</span></span>

<span data-ttu-id="2bcd2-127">Используйте обычный текстовый редактор по вашему выбору (например, [Notepad++](https://notepad-plus-plus.org/) или [JSON Editor Online),](https://www.jsoneditoronline.org/)чтобы:</span><span class="sxs-lookup"><span data-stu-id="2bcd2-127">Use a plain text editor of your choice (for example, [Notepad++](https://notepad-plus-plus.org/) or [JSON Editor Online](https://www.jsoneditoronline.org/)) to:</span></span>

1. <span data-ttu-id="2bcd2-128">Добавьте определение [атрибута](synchronization-attributedefinition.md) для `officeCode` атрибута.</span><span class="sxs-lookup"><span data-stu-id="2bcd2-128">Add an [attribute definition](synchronization-attributedefinition.md) for the `officeCode` attribute.</span></span> 

    - <span data-ttu-id="2bcd2-129">В каталогах найдите каталог с именем salesforce.com, а в массиве объекта найдите имя **Пользователя.**</span><span class="sxs-lookup"><span data-stu-id="2bcd2-129">Under directories, find the directory with the name salesforce.com, and in the object's array, find the one named **User**.</span></span>
    - <span data-ttu-id="2bcd2-130">Добавьте новый атрибут в список, указав имя и тип, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="2bcd2-130">Add the new attribute to the list, specifying the name and type, as shown in the following example.</span></span>

2. <span data-ttu-id="2bcd2-131">Добавьте [сопоставление атрибутов](synchronization-attributemapping.md) между `officeCode` и `extensionAttribute10` .</span><span class="sxs-lookup"><span data-stu-id="2bcd2-131">Add an [attribute mapping](synchronization-attributemapping.md) between `officeCode` and `extensionAttribute10`.</span></span>

    - <span data-ttu-id="2bcd2-132">В [рамках синхронизацииRules](synchronization-synchronizationrule.md)найдите правило, которое указывает Azure AD в качестве источника каталога, а Salesforce.com в качестве целевого каталога ( `"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"` ).</span><span class="sxs-lookup"><span data-stu-id="2bcd2-132">Under [synchronizationRules](synchronization-synchronizationrule.md), find the rule that specifies Azure AD as the source directory, and Salesforce.com as the target directory (`"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"`).</span></span>
    - <span data-ttu-id="2bcd2-133">В [objectMappings правила](synchronization-objectmapping.md) найдите сопоставление между пользователями ( `"sourceObjectName": "User",   "targetObjectName": "User"` ).</span><span class="sxs-lookup"><span data-stu-id="2bcd2-133">In the [objectMappings](synchronization-objectmapping.md) of the rule, find the mapping between users (`"sourceObjectName": "User",   "targetObjectName": "User"`).</span></span>
    - <span data-ttu-id="2bcd2-134">В [массиве attributeMappings](synchronization-attributemapping.md) **объектаMapping** добавьте новую запись, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="2bcd2-134">In the [attributeMappings](synchronization-attributemapping.md) array of the **objectMapping**, add a new entry, as shown in the following example.</span></span>

```json
{  
    "directories": [
    {
        "id": "8ffa6169-f354-4751-9b77-9c00765be92d",
            "name": "salesforce.com",
            "objects": [
            {
                "attributes": [
                        {
                            "name": "officeCode",
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
        "name": "USER_OUTBOUND_USER",
        "objectMappings": [
            {
            "attributeMappings": [
                {
                    "source": {
                            "name": "extensionAttribute10",
                            "type": "Attribute"
                        },
                    "targetAttributeName": "officeCode"
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
    }
    ]
}
```

## <a name="save-the-modified-synchronization-schema"></a><span data-ttu-id="2bcd2-135">Сохранение измененной схемы синхронизации</span><span class="sxs-lookup"><span data-stu-id="2bcd2-135">Save the modified synchronization schema</span></span>

<span data-ttu-id="2bcd2-136">При сохранения обновленной схемы синхронизации убедитесь, что в нее включена вся схема, включая неизменененные части.</span><span class="sxs-lookup"><span data-stu-id="2bcd2-136">When you save the updated synchronization schema, make sure that you include the entire schema, including the unmodified parts.</span></span> <span data-ttu-id="2bcd2-137">Этот запрос заменит существующую схему на предоставляемую.</span><span class="sxs-lookup"><span data-stu-id="2bcd2-137">This request will replace the existing schema with the one that you provide.</span></span>

```http
PUT https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
{
    "directories": [..],
    "synchronizationRules": [..]
}

HTTP/1.1 201 No Content
```

<span data-ttu-id="2bcd2-138">Если схема была успешно сохранена, при следующей итерации задания синхронизации она начнет повторно обрабатывать все учетные записи в Azure AD, и новые сопоставления будут применены для всех учетных записей.</span><span class="sxs-lookup"><span data-stu-id="2bcd2-138">If the schema was saved successfully, on the next iteration of the synchronization job, it will start re-processing all the accounts in your Azure AD, and the new mappings will be applied to all provisioned accounts.</span></span>
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
