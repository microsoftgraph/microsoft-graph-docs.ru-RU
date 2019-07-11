---
title: Тип ресурса Обжектмаппинг
description: Определяет способ синхронизации данного объекта из исходного каталога в конечный каталог. В частности, он определяет, как объект в исходном каталоге должен сопоставляться с объектом в целевом каталоге, какие фильтры области (если они есть) следует использовать, чтобы определить, нужно ли подготовить заданный объект, и как будут преобразованы атрибуты объекта. Источник с целевым каталогом.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 667a58f299847188d193a5b50bb9883721d191e9
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620516"
---
# <a name="objectmapping-resource-type"></a><span data-ttu-id="00cc5-104">Тип ресурса Обжектмаппинг</span><span class="sxs-lookup"><span data-stu-id="00cc5-104">objectMapping resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00cc5-105">Определяет способ синхронизации данного объекта из исходного каталога в конечный каталог.</span><span class="sxs-lookup"><span data-stu-id="00cc5-105">Defines how a given object should be synchronized from source directory to target directory.</span></span> <span data-ttu-id="00cc5-106">В частности, он определяет, как объект в исходном каталоге должен сопоставляться с объектом в целевом каталоге, какие фильтры области (если они есть) следует использовать, чтобы определить, нужно ли подготовить заданный объект, и как будут преобразованы атрибуты объекта. Источник с целевым каталогом.</span><span class="sxs-lookup"><span data-stu-id="00cc5-106">In particular, it defines how object in source directory should be matched with an object in target directory, what (if any) scoping filters should be used to decide if we want to provision a given object, and how object attributes should be transformed going from source to target directory.</span></span>

<span data-ttu-id="00cc5-107">Сопоставления объектов являются основной частью [правила синхронизации](synchronization-synchronizationrule.md) и обновляются в составе [схемы синхронизации](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="00cc5-107">Object mappings are the main part of the [synchronization rule](synchronization-synchronizationrule.md) and are updated as part of [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="00cc5-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="00cc5-108">Properties</span></span>

| <span data-ttu-id="00cc5-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="00cc5-109">Property</span></span>      | <span data-ttu-id="00cc5-110">Тип</span><span class="sxs-lookup"><span data-stu-id="00cc5-110">Type</span></span>      | <span data-ttu-id="00cc5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="00cc5-111">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="00cc5-112">Аттрибутемаппингс</span><span class="sxs-lookup"><span data-stu-id="00cc5-112">attributeMappings</span></span>  |<span data-ttu-id="00cc5-113">Коллекция [аттрибутемаппинг](synchronization-attributemapping.md)</span><span class="sxs-lookup"><span data-stu-id="00cc5-113">[attributeMapping](synchronization-attributemapping.md) collection</span></span>    | <span data-ttu-id="00cc5-114">Сопоставления атрибутов определяют, какие атрибуты необходимо сопоставить из исходного объекта в целевом объекте и как они будут передаваться.</span><span class="sxs-lookup"><span data-stu-id="00cc5-114">Attribute mappings define which attributes to map from the source object into the target object and how they should flow.</span></span> <span data-ttu-id="00cc5-115">Для поддержки преобразования исходных значений источника доступны некоторые функции.</span><span class="sxs-lookup"><span data-stu-id="00cc5-115">A number of functions are available to support the transformation of the original source values.</span></span>|
|<span data-ttu-id="00cc5-116">enabled</span><span class="sxs-lookup"><span data-stu-id="00cc5-116">enabled</span></span>        |<span data-ttu-id="00cc5-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="00cc5-117">Boolean</span></span>    |<span data-ttu-id="00cc5-118">Когда `true`сопоставление этого объекта будет обработано во время синхронизации.</span><span class="sxs-lookup"><span data-stu-id="00cc5-118">When `true`, this object mapping will be processed during synchronization.</span></span> <span data-ttu-id="00cc5-119">Когда `false`сопоставление этого объекта будет пропущено.</span><span class="sxs-lookup"><span data-stu-id="00cc5-119">When `false`, this object mapping will be skipped.</span></span>|
|<span data-ttu-id="00cc5-120">Фловтипес</span><span class="sxs-lookup"><span data-stu-id="00cc5-120">flowTypes</span></span>      |<span data-ttu-id="00cc5-121">Обжектфловтипес</span><span class="sxs-lookup"><span data-stu-id="00cc5-121">objectFlowTypes</span></span>    |<span data-ttu-id="00cc5-122">Какие типы Flow включены для этого сопоставления объектов.</span><span class="sxs-lookup"><span data-stu-id="00cc5-122">Which flow types are enabled for this object mapping.</span></span> <span data-ttu-id="00cc5-123">`Add`создает новые объекты в целевом каталоге, `Update` изменяет существующие объекты и `Delete` разменяет существующие.</span><span class="sxs-lookup"><span data-stu-id="00cc5-123">`Add` creates new objects in the target directory, `Update` modifies existing objects, and `Delete` deprovisions existing users.</span></span> <span data-ttu-id="00cc5-124">Значение по умолчанию: `Add, Update, Delete`.</span><span class="sxs-lookup"><span data-stu-id="00cc5-124">The default is `Add, Update, Delete`.</span></span> |
|<span data-ttu-id="00cc5-125">метаданных</span><span class="sxs-lookup"><span data-stu-id="00cc5-125">metadata</span></span>       |<span data-ttu-id="00cc5-126">Коллекция Метадатаентри</span><span class="sxs-lookup"><span data-stu-id="00cc5-126">metadataEntry collection</span></span>    |<span data-ttu-id="00cc5-127">Дополнительные свойства расширения.</span><span class="sxs-lookup"><span data-stu-id="00cc5-127">Additional extension properties.</span></span> <span data-ttu-id="00cc5-128">Если явно не указано иное, значения метаданных не должны изменяться.</span><span class="sxs-lookup"><span data-stu-id="00cc5-128">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="00cc5-129">name</span><span class="sxs-lookup"><span data-stu-id="00cc5-129">name</span></span>           |<span data-ttu-id="00cc5-130">String</span><span class="sxs-lookup"><span data-stu-id="00cc5-130">String</span></span>     |<span data-ttu-id="00cc5-131">Понятное имя сопоставления объектов.</span><span class="sxs-lookup"><span data-stu-id="00cc5-131">Human-friendly name of the object mapping.</span></span>|
|<span data-ttu-id="00cc5-132">scope</span><span class="sxs-lookup"><span data-stu-id="00cc5-132">scope</span></span>          |[<span data-ttu-id="00cc5-133">filter</span><span class="sxs-lookup"><span data-stu-id="00cc5-133">filter</span></span>](synchronization-filter.md)     |<span data-ttu-id="00cc5-134">Определяет фильтр, который будет использоваться при принятии решения о подготовке данного объекта.</span><span class="sxs-lookup"><span data-stu-id="00cc5-134">Defines a filter to be used when deciding whether a given object should be provisioned.</span></span> <span data-ttu-id="00cc5-135">Например, вам может потребоваться предоставить только пользователей, которые находятся в США.</span><span class="sxs-lookup"><span data-stu-id="00cc5-135">For example, you might want to only provision users that are located in the US.</span></span>|
|<span data-ttu-id="00cc5-136">Саурцеобжектнаме</span><span class="sxs-lookup"><span data-stu-id="00cc5-136">sourceObjectName</span></span>           |<span data-ttu-id="00cc5-137">String</span><span class="sxs-lookup"><span data-stu-id="00cc5-137">String</span></span>     |<span data-ttu-id="00cc5-138">Имя объекта в исходном каталоге.</span><span class="sxs-lookup"><span data-stu-id="00cc5-138">Name of the object in the source directory.</span></span> <span data-ttu-id="00cc5-139">Должно сопоставлять имя объекта из исходного [определения каталога](synchronization-directorydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="00cc5-139">Must match the object name from the source [directory definition](synchronization-directorydefinition.md).</span></span>|
|<span data-ttu-id="00cc5-140">Таржетобжектнаме</span><span class="sxs-lookup"><span data-stu-id="00cc5-140">targetObjectName</span></span>           |<span data-ttu-id="00cc5-141">String</span><span class="sxs-lookup"><span data-stu-id="00cc5-141">String</span></span>     |<span data-ttu-id="00cc5-142">Имя объекта в целевом каталоге.</span><span class="sxs-lookup"><span data-stu-id="00cc5-142">Name of the object in target directory.</span></span> <span data-ttu-id="00cc5-143">Должно сопоставлять имя объекта из [определения целевого каталога](synchronization-directorydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="00cc5-143">Must match the object name from the target [directory definition](synchronization-directorydefinition.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="00cc5-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="00cc5-144">JSON representation</span></span>

<span data-ttu-id="00cc5-145">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="00cc5-145">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.objectMapping"
}-->

```json
{
  "attributeMappings": [{"@odata.type": "microsoft.graph.attributeMapping"}],
  "enabled": true,
  "flowTypes": "String",
  "metadata": [{"@odata.type": "microsoft.graph.metadataEntry"}],
  "name": "String",
  "scope": {"@odata.type": "microsoft.graph.filter"},
  "sourceObjectName": "String",
  "targetObjectName": "String"
}
```

## <a name="json-example"></a><span data-ttu-id="00cc5-146">Пример JSON</span><span class="sxs-lookup"><span data-stu-id="00cc5-146">JSON Example</span></span>

<!-- {
  "blockType": "example",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.objectMapping"
}-->

```json
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
        },
        {
            "defaultValue": null,
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": {
                "expression": "Mid([userPrincipalName], 1, 8)",
                "name": "Mid",
                "parameters": [
                    {
                        "key": "source",
                        "value": {
                            "expression": "[userPrincipalName]",
                            "name": "userPrincipalName",
                            "parameters": [],
                            "type": "Attribute"
                        }
                    },
                    {
                        "key": "start",
                        "value": {
                            "expression": "\"1\"",
                            "name": "1",
                            "parameters": [],
                            "type": "Constant"
                        }
                    },
                    {
                        "key": "length",
                        "value": {
                            "expression": "\"8\"",
                            "name": "8",
                            "parameters": [],
                            "type": "Constant"
                        }
                    }
                ],
                "type": "Function"
            },
            "targetAttributeName": "Alias"
        },
        {
            "defaultValue": null,
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": {
                "expression": "[mail]",
                "name": "mail",
                "parameters": [],
                "type": "Attribute"
            },
            "targetAttributeName": "Email"
        },
        {
            "defaultValue": "ISO-8859-1",
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": null,
            "targetAttributeName": "EmailEncodingKey"
        },
        {
            "defaultValue": "en_US",
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": null,
            "targetAttributeName": "LanguageLocaleKey"
        },
        {
            "defaultValue": null,
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": {
                "expression": "[givenName]",
                "name": "givenName",
                "parameters": [],
                "type": "Attribute"
            },
            "targetAttributeName": "FirstName"
        },
        {
            "defaultValue": ".",
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": {
                "expression": "[surname]",
                "name": "surname",
                "parameters": [],
                "type": "Attribute"
            },
            "targetAttributeName": "LastName"
        },
        {
            "defaultValue": "en_US",
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": {
                "expression": "Replace([preferredLanguage], \"-\", , , \"_\", , )",
                "name": "Replace",
                "parameters": [
                    {
                        "key": "source",
                        "value": {
                            "expression": "[preferredLanguage]",
                            "name": "preferredLanguage",
                            "parameters": [],
                            "type": "Attribute"
                        }
                    },
                    {
                        "key": "Find",
                        "value": {
                            "expression": "\"-\"",
                            "name": "-",
                            "parameters": [],
                            "type": "Constant"
                        }
                    },
                    {
                        "key": "Replacement",
                        "value": {
                            "expression": "\"_\"",
                            "name": "_",
                            "parameters": [],
                            "type": "Constant"
                        }
                    }
                ],
                "type": "Function"
            },
            "targetAttributeName": "LocaleSidKey"
        },
        {
            "defaultValue": "Chatter Free User",
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": {
                "expression": "SingleAppRoleAssignment([appRoleAssignments])",
                "name": "SingleAppRoleAssignment",
                "parameters": [
                    {
                        "key": "source",
                        "value": {
                            "expression": "[appRoleAssignments]",
                            "name": "appRoleAssignments",
                            "parameters": [],
                            "type": "Attribute"
                        }
                    }
                ],
                "type": "Function"
            },
            "targetAttributeName": "ProfileName"
        },
        {
            "defaultValue": "America/Los_Angeles",
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": null,
            "targetAttributeName": "TimeZoneSidKey"
        },
        {
            "defaultValue": null,
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 1,
            "source": {
                "expression": "[userPrincipalName]",
                "name": "userPrincipalName",
                "parameters": [],
                "type": "Attribute"
            },
            "targetAttributeName": "Username"
        },
        {
            "defaultValue": "False",
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": null,
            "targetAttributeName": "UserPermissionsCallCenterAutoLogin"
        },
        {
            "defaultValue": "False",
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": null,
            "targetAttributeName": "UserPermissionsMarketingUser"
        },
        {
            "defaultValue": "False",
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": null,
            "targetAttributeName": "UserPermissionsOfflineUser"
        }
    ],
    "enabled": true,
    "flowTypes": "Add, Update, Delete",
    "metadata": [
        {
            "key": "IsCustomerDefined",
            "value": "false"
        },
        {
            "key": "DisableMonitoringForChanges",
            "value": "false"
        },
        {
            "key": "Disposition",
            "value": "\"Normal\""
        },
        {
            "key": "ExcludeFromReporting",
            "value": "false"
        },
        {
            "key": "EscrowBehavior",
            "value": "\"Default\""
        },
        {
            "key": "Unsynchronized",
            "value": "false"
        }
    ],
    "name": "Synchronize Azure Active Directory Users to salesforce.com",
    "scope": null,
    "sourceObjectName": "User",
    "targetObjectName": "User"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "objectMapping resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
