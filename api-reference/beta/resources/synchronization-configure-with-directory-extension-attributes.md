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
# <a name="configure-synchronization-with-directory-extension-attributes"></a><span data-ttu-id="076cb-105">Настройка синхронизации с расширением атрибутов каталога</span><span class="sxs-lookup"><span data-stu-id="076cb-105">Configure synchronization with directory extension attributes</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="076cb-106">Можно настроить параметры синхронизации схемы для включения атрибутов каталога расширения Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="076cb-106">You can customize your synchronization schema to include Azure Active Directory (Azure AD) directory extension attributes.</span></span> <span data-ttu-id="076cb-107">В этой статье описывается, как использовать атрибут расширения каталога (**extension_9d98asdfl15980a_Nickname**) для заполнения значение User.CommunityNickname в Salesforce.</span><span class="sxs-lookup"><span data-stu-id="076cb-107">This article describes how to use a directory extension attribute (**extension_9d98asdfl15980a_Nickname**) to populate the value of User.CommunityNickname in Salesforce.</span></span> <span data-ttu-id="076cb-108">В этом сценарии у вас есть Azure AD подключить настроить для подготовки число атрибуты расширения каталогов Windows Server Active Directory локально для Azure AD.</span><span class="sxs-lookup"><span data-stu-id="076cb-108">In this scenario, you have Azure AD Connect set up to provision a number of directory extension attributes from Windows Server Active Directory on-premises to Azure AD.</span></span> 

<span data-ttu-id="076cb-109">В этой статье предполагается, что уже содержит приложение, которое поддерживает синхронизацию к клиенту через [Портал Azure](https://portal.azure.com), что вы знаете отображаемое имя приложения и имеют маркер авторизации для Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="076cb-109">This article assumes that you have already added an application that supports synchronization to your tenant through the [Azure Portal](https://portal.azure.com), that you know the application display name, and that you have an authorization token for Microsoft Graph.</span></span> <span data-ttu-id="076cb-110">Сведения о том, как получить маркер авторизации содержатся [маркеры доступа Get для вызова Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span><span class="sxs-lookup"><span data-stu-id="076cb-110">For information about how to get the authorization token, see [Get access tokens to call Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span></span>

## <a name="find-the-service-principal-object-by-display-name"></a><span data-ttu-id="076cb-111">Найдите объект участника службы по отображаемому имени</span><span class="sxs-lookup"><span data-stu-id="076cb-111">Find the service principal object by display name</span></span>

<span data-ttu-id="076cb-112">Следующий пример демонстрирует найдите объект участника службы с отображаемым именем «Изолированной среды Salesforce».</span><span class="sxs-lookup"><span data-stu-id="076cb-112">The following example shows how to find a service principal object with the display name "Salesforce Sandbox".</span></span>

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

<span data-ttu-id="076cb-113">`{servicePrincipalId}` — Это `60443998-8cf7-4e61-b05c-a53b658cb5e1`.</span><span class="sxs-lookup"><span data-stu-id="076cb-113">The `{servicePrincipalId}` is `60443998-8cf7-4e61-b05c-a53b658cb5e1`.</span></span>

## <a name="list-synchronization-jobs-in-the-context-of-the-service-principal"></a><span data-ttu-id="076cb-114">Список заданий синхронизации в контексте участников-служб</span><span class="sxs-lookup"><span data-stu-id="076cb-114">List synchronization jobs in the context of the service principal</span></span> 

<span data-ttu-id="076cb-115">Следующий пример показывает, как получить `jobId` , необходимые для работы с.</span><span class="sxs-lookup"><span data-stu-id="076cb-115">The following example shows you how to get the `jobId` that you need to work with.</span></span> <span data-ttu-id="076cb-116">Как правило ответ возвращается только одно задание.</span><span class="sxs-lookup"><span data-stu-id="076cb-116">Generally, the response returns only one job.</span></span>

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

<span data-ttu-id="076cb-117">`{jobId}` — Это `SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa`.</span><span class="sxs-lookup"><span data-stu-id="076cb-117">The `{jobId}` is `SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa`.</span></span>

## <a name="find-the-name-of-the-directory-extension-attribute-you-need"></a><span data-ttu-id="076cb-118">Найдите имя атрибута расширения каталогов, вы должны</span><span class="sxs-lookup"><span data-stu-id="076cb-118">Find the name of the directory extension attribute you need</span></span>

<span data-ttu-id="076cb-119">Вам понадобится полное имя атрибута расширения.</span><span class="sxs-lookup"><span data-stu-id="076cb-119">You'll need the full name of the extension attribute.</span></span> <span data-ttu-id="076cb-120">Если вы не знаете полное имя (который должен выглядеть **extension_9d98asdfl15980a_Nickname**), просмотрите следующие сведения о атрибуты расширения каталогов, а также для их проверки:</span><span class="sxs-lookup"><span data-stu-id="076cb-120">If you don't know the full name (which should look similar to **extension_9d98asdfl15980a_Nickname**), see the following information about directory extension attributes and how to inspect them:</span></span> 

* [<span data-ttu-id="076cb-121">Расширение схемы directory Azure AD с помощью настраиваемых свойств</span><span class="sxs-lookup"><span data-stu-id="076cb-121">Extending the Azure AD directory schema with custom properties</span></span>](https://azure.microsoft.com/en-us/resources/samples/active-directory-dotnet-graphapi-directoryextensions-web/)
* [<span data-ttu-id="076cb-122">Расширения схемы Directory | Основные понятия графике API</span><span class="sxs-lookup"><span data-stu-id="076cb-122">Directory schema extensions | Graph API concepts</span></span>](https://msdn.microsoft.com/library/azure/ad/graph/howto/azure-ad-graph-api-directory-schema-extensions)


## <a name="get-the-synchronization-schema"></a><span data-ttu-id="076cb-123">Получение схемы синхронизации</span><span class="sxs-lookup"><span data-stu-id="076cb-123">Get the synchronization schema</span></span>
<span data-ttu-id="076cb-124">Следующем примере показано, как получить схему синхронизации.</span><span class="sxs-lookup"><span data-stu-id="076cb-124">The following example shows how to get the synchronization schema.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
```

><span data-ttu-id="076cb-125">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="076cb-125">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="076cb-126">Будут возвращены все свойства в фактический вызов.</span><span class="sxs-lookup"><span data-stu-id="076cb-126">All the properties will be returned in an actual call.</span></span>

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

## <a name="add-a-definition-for-the-directory-extension-attribute-and-a-mapping-between-the-attributes"></a><span data-ttu-id="076cb-127">Добавьте определение для атрибута расширения каталогов и сопоставление атрибутов</span><span class="sxs-lookup"><span data-stu-id="076cb-127">Add a definition for the directory extension attribute, and a mapping between the attributes</span></span>

<span data-ttu-id="076cb-128">Используйте редактор обычного текста по выбору (например, ["Блокнот" ++](https://notepad-plus-plus.org/) или [Редактора JSON Online](https://www.jsoneditoronline.org/)) для:</span><span class="sxs-lookup"><span data-stu-id="076cb-128">Use a plain text editor of your choice (for example, [Notepad++](https://notepad-plus-plus.org/) or [JSON Editor Online](https://www.jsoneditoronline.org/)) to:</span></span>

1. <span data-ttu-id="076cb-129">Добавьте [Определение атрибута](synchronization-attributedefinition.md) для `extension_9d98asdfl15980a_Nickname` атрибут.</span><span class="sxs-lookup"><span data-stu-id="076cb-129">Add an [attribute definition](synchronization-attributedefinition.md) for the `extension_9d98asdfl15980a_Nickname` attribute.</span></span> 

    - <span data-ttu-id="076cb-130">В разделе каталоги найти каталог с именем «Azure Active Directory» и найдите один с именем **пользователя**в массив объектов.</span><span class="sxs-lookup"><span data-stu-id="076cb-130">Under directories, find the directory with the name "Azure Active Directory", and in the object's array, find the one named **User**.</span></span>
    - <span data-ttu-id="076cb-131">Добавьте новый атрибут в список, укажите имя и тип, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="076cb-131">Add the new attribute to the list, specifying the name and type, as shown in the following example.</span></span>

2. <span data-ttu-id="076cb-132">Добавьте [атрибут сопоставления](synchronization-attributemapping.md) между extension_9d98asdfl15980a_Nickname и CommunityNickname.</span><span class="sxs-lookup"><span data-stu-id="076cb-132">Add an [attribute mapping](synchronization-attributemapping.md) between extension_9d98asdfl15980a_Nickname and CommunityNickname.</span></span>

    - <span data-ttu-id="076cb-133">В разделе [synchronizationRules](synchronization-synchronizationrule.md)найти правило, которое задает в качестве исходного каталога и Salesforce.com как в целевом каталоге Azure AD (`"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"`).</span><span class="sxs-lookup"><span data-stu-id="076cb-133">Under [synchronizationRules](synchronization-synchronizationrule.md), find the rule that specifies Azure AD as source directory, and Salesforce.com as the target directory (`"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"`).</span></span>
    - <span data-ttu-id="076cb-134">Найдите в [objectMappings](synchronization-objectmapping.md) правила сопоставления между пользователями (`"sourceObjectName": "User",   "targetObjectName": "User"`).</span><span class="sxs-lookup"><span data-stu-id="076cb-134">In the [objectMappings](synchronization-objectmapping.md) of the rule, find the mapping between users (`"sourceObjectName": "User",   "targetObjectName": "User"`).</span></span>
    - <span data-ttu-id="076cb-135">В массиве [attributeMappings](synchronization-attributemapping.md) **objectMapping**добавьте новую запись, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="076cb-135">In the [attributeMappings](synchronization-attributemapping.md) array of the **objectMapping**, add a new entry, as shown in the following example.</span></span>

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

## <a name="save-the-modified-synchronization-schema"></a><span data-ttu-id="076cb-136">Сохранение измененного синхронизации схемы</span><span class="sxs-lookup"><span data-stu-id="076cb-136">Save the modified synchronization schema</span></span>

<span data-ttu-id="076cb-137">При сохранении схемы обновленные синхронизации убедитесь, что включение всей схемы, включая части без изменений.</span><span class="sxs-lookup"><span data-stu-id="076cb-137">When you save the updated synchronization schema, make sure that you include the entire schema, including the unmodified parts.</span></span> <span data-ttu-id="076cb-138">Этот запрос будет заменить существующую схему, предоставленные.</span><span class="sxs-lookup"><span data-stu-id="076cb-138">This request will replace the existing schema with the one that you provide.</span></span>

```http
PUT https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
{
    "directories": [],
    "synchronizationRules": []
}

HTTP/1.1 201 No Content
```

<span data-ttu-id="076cb-139">Схема была сохранена успешно, в следующей итерации задание синхронизации, начнется повторно обработки всех учетных записей в Azure AD и новые сопоставления будет применяться ко всем подготовленные учетные записи.</span><span class="sxs-lookup"><span data-stu-id="076cb-139">If the schema was saved successfully, on the next iteration of the synchronization job, it will start re-processing all the accounts in your Azure AD, and the new mappings will be applied to all provisioned accounts.</span></span>
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-configure-with-directory-extension-attributes.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
