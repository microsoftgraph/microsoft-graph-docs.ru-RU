---
title: Настройка синхронизации с атрибутами расширения каталога
description: Настройте схему синхронизации, включив в нее атрибуты расширения каталога Azure Active Directory (Azure AD).
localization_priority: Normal
doc_type: conceptualPageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3c66e632e7b573be0d899dfee1704624e826c909
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49521322"
---
# <a name="configure-synchronization-with-directory-extension-attributes"></a><span data-ttu-id="d0b2c-103">Настройка синхронизации с атрибутами расширения каталога</span><span class="sxs-lookup"><span data-stu-id="d0b2c-103">Configure synchronization with directory extension attributes</span></span>

<span data-ttu-id="d0b2c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0b2c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0b2c-105">Вы можете настроить схему синхронизации, включив в нее атрибуты расширения каталога Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="d0b2c-105">You can customize your synchronization schema to include Azure Active Directory (Azure AD) directory extension attributes.</span></span> <span data-ttu-id="d0b2c-106">В этой статье описывается, как использовать атрибут расширения каталога (**extension_9d98asdfl15980a_Nickname**) для заполнения значения User. Коммунитиниккнаме в Salesforce.</span><span class="sxs-lookup"><span data-stu-id="d0b2c-106">This article describes how to use a directory extension attribute (**extension_9d98asdfl15980a_Nickname**) to populate the value of User.CommunityNickname in Salesforce.</span></span> <span data-ttu-id="d0b2c-107">В этом сценарии у вас есть Azure AD Connect, настроенный на подготовку ряда атрибутов расширения каталогов из локальной среды Windows Server Active Directory в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d0b2c-107">In this scenario, you have Azure AD Connect set up to provision a number of directory extension attributes from Windows Server Active Directory on-premises to Azure AD.</span></span> 

<span data-ttu-id="d0b2c-108">В этой статье предполагается, что вы уже добавили приложение, которое поддерживает синхронизацию с клиентом с помощью [портала Azure](https://portal.azure.com), вы знаете отображаемое имя приложения, и у вас есть маркер авторизации для Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d0b2c-108">This article assumes that you have already added an application that supports synchronization to your tenant through the [Azure Portal](https://portal.azure.com), that you know the application display name, and that you have an authorization token for Microsoft Graph.</span></span> <span data-ttu-id="d0b2c-109">Сведения о том, как получить маркер авторизации, можно найти [в статье получение маркеров доступа для вызова Microsoft Graph](/graph/auth/).</span><span class="sxs-lookup"><span data-stu-id="d0b2c-109">For information about how to get the authorization token, see [Get access tokens to call Microsoft Graph](/graph/auth/).</span></span>

## <a name="find-the-service-principal-object-by-display-name"></a><span data-ttu-id="d0b2c-110">Поиск объекта субъекта службы по отображаемому имени</span><span class="sxs-lookup"><span data-stu-id="d0b2c-110">Find the service principal object by display name</span></span>

<span data-ttu-id="d0b2c-111">В приведенном ниже примере показано, как найти объект участника службы с отображаемым именем "песочницы Salesforce".</span><span class="sxs-lookup"><span data-stu-id="d0b2c-111">The following example shows how to find a service principal object with the display name "Salesforce Sandbox".</span></span>

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

<span data-ttu-id="d0b2c-112">Параметр `{servicePrincipalId}` имеет значение `60443998-8cf7-4e61-b05c-a53b658cb5e1` .</span><span class="sxs-lookup"><span data-stu-id="d0b2c-112">The `{servicePrincipalId}` is `60443998-8cf7-4e61-b05c-a53b658cb5e1`.</span></span>

## <a name="list-synchronization-jobs-in-the-context-of-the-service-principal"></a><span data-ttu-id="d0b2c-113">Перечисление заданий синхронизации в контексте субъекта-службы</span><span class="sxs-lookup"><span data-stu-id="d0b2c-113">List synchronization jobs in the context of the service principal</span></span> 

<span data-ttu-id="d0b2c-114">В приведенном ниже примере показано, как получить сведения о том `jobId` , что необходимо для работы.</span><span class="sxs-lookup"><span data-stu-id="d0b2c-114">The following example shows you how to get the `jobId` that you need to work with.</span></span> <span data-ttu-id="d0b2c-115">Как правило, ответ возвращает только одно задание.</span><span class="sxs-lookup"><span data-stu-id="d0b2c-115">Generally, the response returns only one job.</span></span>

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

<span data-ttu-id="d0b2c-116">Параметр `{jobId}` имеет значение `SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa` .</span><span class="sxs-lookup"><span data-stu-id="d0b2c-116">The `{jobId}` is `SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa`.</span></span>

## <a name="find-the-name-of-the-directory-extension-attribute-you-need"></a><span data-ttu-id="d0b2c-117">Найдите имя необходимого атрибута расширения каталога</span><span class="sxs-lookup"><span data-stu-id="d0b2c-117">Find the name of the directory extension attribute you need</span></span>

<span data-ttu-id="d0b2c-118">Вам потребуется полное имя атрибута расширения.</span><span class="sxs-lookup"><span data-stu-id="d0b2c-118">You'll need the full name of the extension attribute.</span></span> <span data-ttu-id="d0b2c-119">Если полное имя (которое должно выглядеть аналогично **extension_9d98asdfl15980a_Nickname**), ознакомьтесь со следующими сведениями о атрибутах расширения каталогов и способах их проверки:</span><span class="sxs-lookup"><span data-stu-id="d0b2c-119">If you don't know the full name (which should look similar to **extension_9d98asdfl15980a_Nickname**), see the following information about directory extension attributes and how to inspect them:</span></span> 

* [<span data-ttu-id="d0b2c-120">Расширение схемы каталога Azure AD с помощью настраиваемых свойств</span><span class="sxs-lookup"><span data-stu-id="d0b2c-120">Extending the Azure AD directory schema with custom properties</span></span>](/graph/extensibility-overview)
* [<span data-ttu-id="d0b2c-121">Расширения схемы каталогов | Основные понятия API Graph</span><span class="sxs-lookup"><span data-stu-id="d0b2c-121">Directory schema extensions | Graph API concepts</span></span>](/previous-versions/azure/ad/graph/howto/azure-ad-graph-api-directory-schema-extensions)


## <a name="get-the-synchronization-schema"></a><span data-ttu-id="d0b2c-122">Получение схемы синхронизации</span><span class="sxs-lookup"><span data-stu-id="d0b2c-122">Get the synchronization schema</span></span>
<span data-ttu-id="d0b2c-123">В приведенном ниже примере показано, как получить схему синхронизации.</span><span class="sxs-lookup"><span data-stu-id="d0b2c-123">The following example shows how to get the synchronization schema.</span></span>


# <a name="http"></a>[<span data-ttu-id="d0b2c-124">HTTP</span><span class="sxs-lookup"><span data-stu-id="d0b2c-124">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
```
# <a name="c"></a>[<span data-ttu-id="d0b2c-125">C#</span><span class="sxs-lookup"><span data-stu-id="d0b2c-125">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationschema-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d0b2c-126">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d0b2c-126">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationschema-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d0b2c-127">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d0b2c-127">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationschema-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d0b2c-128">Java</span><span class="sxs-lookup"><span data-stu-id="d0b2c-128">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-synchronizationschema-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


><span data-ttu-id="d0b2c-129">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d0b2c-129">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d0b2c-130">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d0b2c-130">All the properties will be returned in an actual call.</span></span>

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

## <a name="add-a-definition-for-the-directory-extension-attribute-and-a-mapping-between-the-attributes"></a><span data-ttu-id="d0b2c-131">Добавление определения атрибута расширения каталога и сопоставления между атрибутами</span><span class="sxs-lookup"><span data-stu-id="d0b2c-131">Add a definition for the directory extension attribute, and a mapping between the attributes</span></span>

<span data-ttu-id="d0b2c-132">Используйте простой текстовый редактор (например, [Notepad + +](https://notepad-plus-plus.org/) или [Редактор JSON Online](https://www.jsoneditoronline.org/)), чтобы:</span><span class="sxs-lookup"><span data-stu-id="d0b2c-132">Use a plain text editor of your choice (for example, [Notepad++](https://notepad-plus-plus.org/) or [JSON Editor Online](https://www.jsoneditoronline.org/)) to:</span></span>

1. <span data-ttu-id="d0b2c-133">Добавьте [Определение атрибута](synchronization-attributedefinition.md) `extension_9d98asdfl15980a_Nickname` .</span><span class="sxs-lookup"><span data-stu-id="d0b2c-133">Add an [attribute definition](synchronization-attributedefinition.md) for the `extension_9d98asdfl15980a_Nickname` attribute.</span></span> 

    - <span data-ttu-id="d0b2c-134">В разделе Каталоги найдите каталог с именем "Azure Active Directory" и в массиве объекта найдите одного пользователя с именем **User**.</span><span class="sxs-lookup"><span data-stu-id="d0b2c-134">Under directories, find the directory with the name "Azure Active Directory", and in the object's array, find the one named **User**.</span></span>
    - <span data-ttu-id="d0b2c-135">Добавьте новый атрибут в список, указав имя и тип, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="d0b2c-135">Add the new attribute to the list, specifying the name and type, as shown in the following example.</span></span>

2. <span data-ttu-id="d0b2c-136">Добавьте [сопоставление атрибутов](synchronization-attributemapping.md) между Extension_9d98asdfl15980a_Nickname и коммунитиниккнаме.</span><span class="sxs-lookup"><span data-stu-id="d0b2c-136">Add an [attribute mapping](synchronization-attributemapping.md) between extension_9d98asdfl15980a_Nickname and CommunityNickname.</span></span>

    - <span data-ttu-id="d0b2c-137">В разделе [синчронизатионрулес](synchronization-synchronizationrule.md)найдите правило, задающее Azure AD в качестве исходного каталога, и Salesforce.com в качестве целевого каталога ( `"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"` ).</span><span class="sxs-lookup"><span data-stu-id="d0b2c-137">Under [synchronizationRules](synchronization-synchronizationrule.md), find the rule that specifies Azure AD as source directory, and Salesforce.com as the target directory (`"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"`).</span></span>
    - <span data-ttu-id="d0b2c-138">В [обжектмаппингс](synchronization-objectmapping.md) правила найдите сопоставление между пользователями ( `"sourceObjectName": "User",   "targetObjectName": "User"` ).</span><span class="sxs-lookup"><span data-stu-id="d0b2c-138">In the [objectMappings](synchronization-objectmapping.md) of the rule, find the mapping between users (`"sourceObjectName": "User",   "targetObjectName": "User"`).</span></span>
    - <span data-ttu-id="d0b2c-139">В массиве [аттрибутемаппингс](synchronization-attributemapping.md) объекта **обжектмаппинг** добавьте новую запись, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="d0b2c-139">In the [attributeMappings](synchronization-attributemapping.md) array of the **objectMapping**, add a new entry, as shown in the following example.</span></span>

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

## <a name="save-the-modified-synchronization-schema"></a><span data-ttu-id="d0b2c-140">Сохранение измененной схемы синхронизации</span><span class="sxs-lookup"><span data-stu-id="d0b2c-140">Save the modified synchronization schema</span></span>

<span data-ttu-id="d0b2c-141">При сохранении обновленной схемы синхронизации убедитесь, что включается вся схема, включая неизмененные части.</span><span class="sxs-lookup"><span data-stu-id="d0b2c-141">When you save the updated synchronization schema, make sure that you include the entire schema, including the unmodified parts.</span></span> <span data-ttu-id="d0b2c-142">Этот запрос заменит существующую схему на предоставленную вами.</span><span class="sxs-lookup"><span data-stu-id="d0b2c-142">This request will replace the existing schema with the one that you provide.</span></span>

```http
PUT https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
{
    "directories": [],
    "synchronizationRules": []
}

HTTP/1.1 201 No Content
```

<span data-ttu-id="d0b2c-143">Если схема была успешно сохранена, в следующей итерации задания синхронизации начнется повторная обработка всех учетных записей в Azure AD, а новые сопоставления будут применены ко всем подготовленным учетным записям.</span><span class="sxs-lookup"><span data-stu-id="d0b2c-143">If the schema was saved successfully, on the next iteration of the synchronization job, it will start re-processing all the accounts in your Azure AD, and the new mappings will be applied to all provisioned accounts.</span></span>
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
