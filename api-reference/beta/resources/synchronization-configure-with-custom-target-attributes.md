---
title: Настройка синхронизации с помощью настраиваемого конечного атрибутов
description: Можно настроить параметры синхронизации схемы для включения настраиваемые атрибуты, которые определены в целевой каталог. В этой статье описывается настройка Salesforce подписки, добавив новое поле под названием `officeCode`. Вы настроили синхронизацию с Azure Active Directory (Azure AD) для Salesforce, и для каждого пользователя будет заполнения `officeCode` поля в Salesforce со значением из `extensionAttribute10` в Azure AD.
ms.openlocfilehash: e043fa5e458a56312871567bb14598f9232e97eb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077974"
---
# <a name="configure-synchronization-with-custom-target-attributes"></a><span data-ttu-id="4dea5-105">Настройка синхронизации с помощью настраиваемого конечного атрибутов</span><span class="sxs-lookup"><span data-stu-id="4dea5-105">Configure synchronization with custom target attributes</span></span>

> <span data-ttu-id="4dea5-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4dea5-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4dea5-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4dea5-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4dea5-108">Можно настроить параметры синхронизации схемы для включения настраиваемые атрибуты, которые определены в целевой каталог.</span><span class="sxs-lookup"><span data-stu-id="4dea5-108">You can customize your synchronization schema to include custom attributes that are defined in the target directory.</span></span> <span data-ttu-id="4dea5-109">В этой статье описывается настройка Salesforce подписки, добавив новое поле под названием `officeCode`.</span><span class="sxs-lookup"><span data-stu-id="4dea5-109">This article describes how to customize a Salesforce subscription by adding a new field called `officeCode`.</span></span> <span data-ttu-id="4dea5-110">Вы настроили синхронизацию с Azure Active Directory (Azure AD) для Salesforce, и для каждого пользователя будет заполнения `officeCode` поля в Salesforce со значением из `extensionAttribute10` в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4dea5-110">You set up synchronization from Azure Active Directory (Azure AD) to Salesforce, and for each user, you will populate the `officeCode` field in Salesforce with the value from the `extensionAttribute10` field in Azure AD.</span></span>

<span data-ttu-id="4dea5-111">В этой статье предполагается, что уже содержит приложение, которое поддерживает синхронизацию к клиенту через [Портал Azure](https://portal.azure.com), что вы знаете отображаемое имя приложения и имеют маркер авторизации для Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="4dea5-111">This article assumes that you have already added an application that supports synchronization to your tenant through the [Azure Portal](https://portal.azure.com), that you know the application display name, and that you have an authorization token for Microsoft Graph.</span></span> <span data-ttu-id="4dea5-112">Сведения о том, как получить маркер авторизации содержатся [маркеры доступа Get для вызова Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span><span class="sxs-lookup"><span data-stu-id="4dea5-112">For information about how to get the authorization token, see [Get access tokens to call Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span></span>

## <a name="find-the-service-principal-object-by-display-name"></a><span data-ttu-id="4dea5-113">Найдите объект участника службы по отображаемому имени</span><span class="sxs-lookup"><span data-stu-id="4dea5-113">Find the service principal object by display name</span></span>

<span data-ttu-id="4dea5-114">Следующий пример демонстрирует найдите объект участника службы с отображаемым именем Salesforce.</span><span class="sxs-lookup"><span data-stu-id="4dea5-114">The following example shows how to find a service principal object with the display name Salesforce.</span></span>

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

<span data-ttu-id="4dea5-115">`{servicePrincipalId}` — Это `167e33e9-f80e-490e-b4d8-698d4a80fb3e`.</span><span class="sxs-lookup"><span data-stu-id="4dea5-115">The `{servicePrincipalId}` is `167e33e9-f80e-490e-b4d8-698d4a80fb3e`.</span></span>


## <a name="list-synchronization-jobs-in-the-context-of-the-service-principal"></a><span data-ttu-id="4dea5-116">Список заданий синхронизации в контексте участников-служб</span><span class="sxs-lookup"><span data-stu-id="4dea5-116">List synchronization jobs in the context of the service principal</span></span> 

<span data-ttu-id="4dea5-117">Следующий пример показывает, как получить `jobId` , необходимые для работы с.</span><span class="sxs-lookup"><span data-stu-id="4dea5-117">The following example shows you how to get the `jobId` that you need to work with.</span></span> <span data-ttu-id="4dea5-118">Как правило ответ возвращается только одно задание.</span><span class="sxs-lookup"><span data-stu-id="4dea5-118">Generally, the response returns only one job.</span></span>

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

<span data-ttu-id="4dea5-119">`{jobId}` — Это `SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa`.</span><span class="sxs-lookup"><span data-stu-id="4dea5-119">The `{jobId}` is `SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa`.</span></span>


## <a name="get-the-synchronization-schema"></a><span data-ttu-id="4dea5-120">Получение схемы синхронизации</span><span class="sxs-lookup"><span data-stu-id="4dea5-120">Get the synchronization schema</span></span>
<span data-ttu-id="4dea5-121">Следующем примере показано, как получить схему синхронизации.</span><span class="sxs-lookup"><span data-stu-id="4dea5-121">The following example shows how to get the synchronization schema.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
```

><span data-ttu-id="4dea5-122">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4dea5-122">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4dea5-123">Будут возвращены все свойства в фактический вызов.</span><span class="sxs-lookup"><span data-stu-id="4dea5-123">All the properties will be returned in an actual call.</span></span>

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

## <a name="add-a-definition-for-the-officecode-attribute-and-a-mapping-between-attributes"></a><span data-ttu-id="4dea5-124">Добавьте определение для атрибута officeCode и сопоставление атрибутов</span><span class="sxs-lookup"><span data-stu-id="4dea5-124">Add a definition for the officeCode attribute and a mapping between attributes</span></span>

<span data-ttu-id="4dea5-125">Используйте редактор обычного текста по выбору (например, ["Блокнот" ++](https://notepad-plus-plus.org/) или [Редактора JSON Online](https://www.jsoneditoronline.org/)) для:</span><span class="sxs-lookup"><span data-stu-id="4dea5-125">Use a plain text editor of your choice (for example, [Notepad++](https://notepad-plus-plus.org/) or [JSON Editor Online](https://www.jsoneditoronline.org/)) to:</span></span>

1. <span data-ttu-id="4dea5-126">Добавьте [Определение атрибута](synchronization-attributedefinition.md) для `officeCode` атрибут.</span><span class="sxs-lookup"><span data-stu-id="4dea5-126">Add an [attribute definition](synchronization-attributedefinition.md) for the `officeCode` attribute.</span></span> 

    - <span data-ttu-id="4dea5-127">В разделе каталоги определить каталог с именем salesforce.com и в массив объектов, один с именем **пользователя**.</span><span class="sxs-lookup"><span data-stu-id="4dea5-127">Under directories, find the directory with the name salesforce.com, and in the object's array, find the one named **User**.</span></span>
    - <span data-ttu-id="4dea5-128">Добавьте новый атрибут в список, укажите имя и тип, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="4dea5-128">Add the new attribute to the list, specifying the name and type, as shown in the following example.</span></span>

2. <span data-ttu-id="4dea5-129">Добавьте [атрибут сопоставления](synchronization-attributemapping.md) между `officeCode` и `extensionAttribute10`.</span><span class="sxs-lookup"><span data-stu-id="4dea5-129">Add an [attribute mapping](synchronization-attributemapping.md) between `officeCode` and `extensionAttribute10`.</span></span>

    - <span data-ttu-id="4dea5-130">В разделе [synchronizationRules](synchronization-synchronizationrule.md)найти правило, которое задает в качестве исходного каталога и Salesforce.com как в целевом каталоге Azure AD (`"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"`).</span><span class="sxs-lookup"><span data-stu-id="4dea5-130">Under [synchronizationRules](synchronization-synchronizationrule.md), find the rule that specifies Azure AD as the source directory, and Salesforce.com as the target directory (`"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"`).</span></span>
    - <span data-ttu-id="4dea5-131">Найдите в [objectMappings](synchronization-objectmapping.md) правила сопоставления между пользователями (`"sourceObjectName": "User",   "targetObjectName": "User"`).</span><span class="sxs-lookup"><span data-stu-id="4dea5-131">In the [objectMappings](synchronization-objectmapping.md) of the rule, find the mapping between users (`"sourceObjectName": "User",   "targetObjectName": "User"`).</span></span>
    - <span data-ttu-id="4dea5-132">В массиве [attributeMappings](synchronization-attributemapping.md) **objectMapping**добавьте новую запись, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="4dea5-132">In the [attributeMappings](synchronization-attributemapping.md) array of the **objectMapping**, add a new entry, as shown in the following example.</span></span>

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

## <a name="save-the-modified-synchronization-schema"></a><span data-ttu-id="4dea5-133">Сохранение измененного синхронизации схемы</span><span class="sxs-lookup"><span data-stu-id="4dea5-133">Save the modified synchronization schema</span></span>

<span data-ttu-id="4dea5-134">При сохранении схемы обновленные синхронизации убедитесь, что включение всей схемы, включая части без изменений.</span><span class="sxs-lookup"><span data-stu-id="4dea5-134">When you save the updated synchronization schema, make sure that you include the entire schema, including the unmodified parts.</span></span> <span data-ttu-id="4dea5-135">Этот запрос будет заменить существующую схему, предоставленные.</span><span class="sxs-lookup"><span data-stu-id="4dea5-135">This request will replace the existing schema with the one that you provide.</span></span>

```http
PUT https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
{
    "directories": [..],
    "synchronizationRules": [..]
}

HTTP/1.1 201 No Content
```

<span data-ttu-id="4dea5-136">Схема была сохранена успешно, в следующей итерации задание синхронизации, начнется повторно обработки всех учетных записей в Azure AD и новые сопоставления будет применяться ко всем подготовленные учетные записи.</span><span class="sxs-lookup"><span data-stu-id="4dea5-136">If the schema was saved successfully, on the next iteration of the synchronization job, it will start re-processing all the accounts in your Azure AD, and the new mappings will be applied to all provisioned accounts.</span></span>
