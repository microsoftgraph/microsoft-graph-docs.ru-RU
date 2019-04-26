---
title: Настройка синхронизации с атрибутами расширения каталога
description: 'Вы можете настроить схему синхронизации, включив в нее атрибуты расширения каталога Azure Active Directory (Azure AD). В этой статье описывается, как использовать атрибут расширения каталога (**extension_9d98asdfl15980a_Nickname**) для заполнения значения User. Коммунитиниккнаме в Salesforce. В этом сценарии у вас есть Azure AD Connect, настроенный на подготовку ряда атрибутов расширения каталогов из локальной среды Windows Server Active Directory в Azure AD. '
localization_priority: Normal
ms.openlocfilehash: 4160a95acfc6b23f5d5a9d880f36d9ca6a1f3362
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582163"
---
# <a name="configure-synchronization-with-directory-extension-attributes"></a><span data-ttu-id="0ea36-105">Настройка синхронизации с атрибутами расширения каталога</span><span class="sxs-lookup"><span data-stu-id="0ea36-105">Configure synchronization with directory extension attributes</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ea36-106">Вы можете настроить схему синхронизации, включив в нее атрибуты расширения каталога Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="0ea36-106">You can customize your synchronization schema to include Azure Active Directory (Azure AD) directory extension attributes.</span></span> <span data-ttu-id="0ea36-107">В этой статье описывается, как использовать атрибут расширения каталога (**extension_9d98asdfl15980a_Nickname**) для заполнения значения User. Коммунитиниккнаме в Salesforce.</span><span class="sxs-lookup"><span data-stu-id="0ea36-107">This article describes how to use a directory extension attribute (**extension_9d98asdfl15980a_Nickname**) to populate the value of User.CommunityNickname in Salesforce.</span></span> <span data-ttu-id="0ea36-108">В этом сценарии у вас есть Azure AD Connect, настроенный на подготовку ряда атрибутов расширения каталогов из локальной среды Windows Server Active Directory в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0ea36-108">In this scenario, you have Azure AD Connect set up to provision a number of directory extension attributes from Windows Server Active Directory on-premises to Azure AD.</span></span> 

<span data-ttu-id="0ea36-109">В этой статье предполагается, что вы уже добавили приложение, которое поддерживает синхронизацию с клиентом с помощью [портала Azure](https://portal.azure.com), вы знаете отображаемое имя приложения, и у вас есть маркер авторизации для Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="0ea36-109">This article assumes that you have already added an application that supports synchronization to your tenant through the [Azure Portal](https://portal.azure.com), that you know the application display name, and that you have an authorization token for Microsoft Graph.</span></span> <span data-ttu-id="0ea36-110">Сведения о том, как получить маркер авторизации, можно найти [в статье получение маркеров доступа для вызова Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span><span class="sxs-lookup"><span data-stu-id="0ea36-110">For information about how to get the authorization token, see [Get access tokens to call Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span></span>

## <a name="find-the-service-principal-object-by-display-name"></a><span data-ttu-id="0ea36-111">Поиск объекта субъекта службы по отображаемому имени</span><span class="sxs-lookup"><span data-stu-id="0ea36-111">Find the service principal object by display name</span></span>

<span data-ttu-id="0ea36-112">В приведенном ниже примере показано, как найти объект участника службы с отображаемым именем "песочницы Salesforce".</span><span class="sxs-lookup"><span data-stu-id="0ea36-112">The following example shows how to find a service principal object with the display name "Salesforce Sandbox".</span></span>

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

<span data-ttu-id="0ea36-113">Параметр `{servicePrincipalId}` имеет `60443998-8cf7-4e61-b05c-a53b658cb5e1`значение.</span><span class="sxs-lookup"><span data-stu-id="0ea36-113">The `{servicePrincipalId}` is `60443998-8cf7-4e61-b05c-a53b658cb5e1`.</span></span>

## <a name="list-synchronization-jobs-in-the-context-of-the-service-principal"></a><span data-ttu-id="0ea36-114">ПереЧисление заданий синхронизации в контексте субъекта-службы</span><span class="sxs-lookup"><span data-stu-id="0ea36-114">List synchronization jobs in the context of the service principal</span></span> 

<span data-ttu-id="0ea36-115">В приведенном ниже примере показано `jobId` , как получить сведения о том, что необходимо для работы.</span><span class="sxs-lookup"><span data-stu-id="0ea36-115">The following example shows you how to get the `jobId` that you need to work with.</span></span> <span data-ttu-id="0ea36-116">Как правило, ответ возвращает только одно задание.</span><span class="sxs-lookup"><span data-stu-id="0ea36-116">Generally, the response returns only one job.</span></span>

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

<span data-ttu-id="0ea36-117">Параметр `{jobId}` имеет `SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa`значение.</span><span class="sxs-lookup"><span data-stu-id="0ea36-117">The `{jobId}` is `SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa`.</span></span>

## <a name="find-the-name-of-the-directory-extension-attribute-you-need"></a><span data-ttu-id="0ea36-118">Найдите имя необходимого атрибута расширения каталога</span><span class="sxs-lookup"><span data-stu-id="0ea36-118">Find the name of the directory extension attribute you need</span></span>

<span data-ttu-id="0ea36-119">Вам потребуется полное имя атрибута расширения.</span><span class="sxs-lookup"><span data-stu-id="0ea36-119">You'll need the full name of the extension attribute.</span></span> <span data-ttu-id="0ea36-120">Если полное имя (которое должно выглядеть аналогично **extension_9d98asdfl15980a_Nickname**), ознакомьтесь со следующими сведениями о атрибутах расширения каталогов и способах их проверки:</span><span class="sxs-lookup"><span data-stu-id="0ea36-120">If you don't know the full name (which should look similar to **extension_9d98asdfl15980a_Nickname**), see the following information about directory extension attributes and how to inspect them:</span></span> 

* [<span data-ttu-id="0ea36-121">Расширение схемы каталога Azure AD с помощью настраиваемых свойств</span><span class="sxs-lookup"><span data-stu-id="0ea36-121">Extending the Azure AD directory schema with custom properties</span></span>](https://azure.microsoft.com/en-us/resources/samples/active-directory-dotnet-graphapi-directoryextensions-web/)
* [<span data-ttu-id="0ea36-122">Расширения схемы каталогов | Основные понятия API Graph</span><span class="sxs-lookup"><span data-stu-id="0ea36-122">Directory schema extensions | Graph API concepts</span></span>](https://msdn.microsoft.com/library/azure/ad/graph/howto/azure-ad-graph-api-directory-schema-extensions)


## <a name="get-the-synchronization-schema"></a><span data-ttu-id="0ea36-123">Получение схемы синхронизации</span><span class="sxs-lookup"><span data-stu-id="0ea36-123">Get the synchronization schema</span></span>
<span data-ttu-id="0ea36-124">В приведенном ниже примере показано, как получить схему синхронизации.</span><span class="sxs-lookup"><span data-stu-id="0ea36-124">The following example shows how to get the synchronization schema.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
```

><span data-ttu-id="0ea36-125">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0ea36-125">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0ea36-126">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0ea36-126">All the properties will be returned in an actual call.</span></span>

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

## <a name="add-a-definition-for-the-directory-extension-attribute-and-a-mapping-between-the-attributes"></a><span data-ttu-id="0ea36-127">Добавление определения атрибута расширения каталога и сопоставления между атрибутами</span><span class="sxs-lookup"><span data-stu-id="0ea36-127">Add a definition for the directory extension attribute, and a mapping between the attributes</span></span>

<span data-ttu-id="0ea36-128">Используйте простой текстовый редактор (например, [Notepad + +](https://notepad-plus-plus.org/) или [Редактор JSON Online](https://www.jsoneditoronline.org/)), чтобы:</span><span class="sxs-lookup"><span data-stu-id="0ea36-128">Use a plain text editor of your choice (for example, [Notepad++](https://notepad-plus-plus.org/) or [JSON Editor Online](https://www.jsoneditoronline.org/)) to:</span></span>

1. <span data-ttu-id="0ea36-129">Добавьте `extension_9d98asdfl15980a_Nickname` [Определение атрибута](synchronization-attributedefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="0ea36-129">Add an [attribute definition](synchronization-attributedefinition.md) for the `extension_9d98asdfl15980a_Nickname` attribute.</span></span> 

    - <span data-ttu-id="0ea36-130">В разделе Каталоги найдите каталог с именем "Azure Active Directory" и в массиве объекта найдите одного пользователя с именем **User**.</span><span class="sxs-lookup"><span data-stu-id="0ea36-130">Under directories, find the directory with the name "Azure Active Directory", and in the object's array, find the one named **User**.</span></span>
    - <span data-ttu-id="0ea36-131">Добавьте новый атрибут в список, указав имя и тип, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="0ea36-131">Add the new attribute to the list, specifying the name and type, as shown in the following example.</span></span>

2. <span data-ttu-id="0ea36-132">Добавьте [сопоставление атрибутов](synchronization-attributemapping.md) между Extension_9d98asdfl15980a_Nickname и коммунитиниккнаме.</span><span class="sxs-lookup"><span data-stu-id="0ea36-132">Add an [attribute mapping](synchronization-attributemapping.md) between extension_9d98asdfl15980a_Nickname and CommunityNickname.</span></span>

    - <span data-ttu-id="0ea36-133">В разделе [синчронизатионрулес](synchronization-synchronizationrule.md)найдите правило, задающее Azure AD в качестве исходного каталога, и Salesforce.com в качестве целевого каталога`"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"`().</span><span class="sxs-lookup"><span data-stu-id="0ea36-133">Under [synchronizationRules](synchronization-synchronizationrule.md), find the rule that specifies Azure AD as source directory, and Salesforce.com as the target directory (`"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"`).</span></span>
    - <span data-ttu-id="0ea36-134">В [обжектмаппингс](synchronization-objectmapping.md) правила найдите сопоставление между пользователями (`"sourceObjectName": "User",   "targetObjectName": "User"`).</span><span class="sxs-lookup"><span data-stu-id="0ea36-134">In the [objectMappings](synchronization-objectmapping.md) of the rule, find the mapping between users (`"sourceObjectName": "User",   "targetObjectName": "User"`).</span></span>
    - <span data-ttu-id="0ea36-135">В массиве [аттрибутемаппингс](synchronization-attributemapping.md) объекта **обжектмаппинг**добавьте новую запись, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="0ea36-135">In the [attributeMappings](synchronization-attributemapping.md) array of the **objectMapping**, add a new entry, as shown in the following example.</span></span>

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

## <a name="save-the-modified-synchronization-schema"></a><span data-ttu-id="0ea36-136">Сохранение измененной схемы синхронизации</span><span class="sxs-lookup"><span data-stu-id="0ea36-136">Save the modified synchronization schema</span></span>

<span data-ttu-id="0ea36-137">При сохранении обновленной схемы синхронизации убедитесь, что включается вся схема, включая неизмененные части.</span><span class="sxs-lookup"><span data-stu-id="0ea36-137">When you save the updated synchronization schema, make sure that you include the entire schema, including the unmodified parts.</span></span> <span data-ttu-id="0ea36-138">Этот запрос заменит существующую схему на предоставленную вами.</span><span class="sxs-lookup"><span data-stu-id="0ea36-138">This request will replace the existing schema with the one that you provide.</span></span>

```http
PUT https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
{
    "directories": [],
    "synchronizationRules": []
}

HTTP/1.1 201 No Content
```

<span data-ttu-id="0ea36-139">Если схема была успешно сохранена, в следующей итерации задания синхронизации начнется повторная обработка всех учетных записей в Azure AD, а новые сопоставления будут применены ко всем подготовленным учетным записям.</span><span class="sxs-lookup"><span data-stu-id="0ea36-139">If the schema was saved successfully, on the next iteration of the synchronization job, it will start re-processing all the accounts in your Azure AD, and the new mappings will be applied to all provisioned accounts.</span></span>
