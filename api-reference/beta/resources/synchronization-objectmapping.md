---
title: Тип ресурса objectMapping
description: Определяет, как того или иного объекта должны быть синхронизированы из исходного каталога в конечный каталог. В частности, определяются как объект в исходный каталог должны совпадать с помощью объекта в целевой каталог, что (если они имеются) области Фильтры следует использовать в том, если его нужно подготовить к данному объекту, и как атрибуты объектов должен быть преобразован переход от Источник конечный каталог.
localization_priority: Normal
ms.openlocfilehash: 274d401c28abc25d904c259b00a673f3c0a53888
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526916"
---
# <a name="objectmapping-resource-type"></a><span data-ttu-id="85dbb-104">Тип ресурса objectMapping</span><span class="sxs-lookup"><span data-stu-id="85dbb-104">objectMapping resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85dbb-105">Определяет, как того или иного объекта должны быть синхронизированы из исходного каталога в конечный каталог.</span><span class="sxs-lookup"><span data-stu-id="85dbb-105">Defines how a given object should be synchronized from source directory to target directory.</span></span> <span data-ttu-id="85dbb-106">В частности, определяются как объект в исходный каталог должны совпадать с помощью объекта в целевой каталог, что (если они имеются) области Фильтры следует использовать в том, если его нужно подготовить к данному объекту, и как атрибуты объектов должен быть преобразован переход от Источник конечный каталог.</span><span class="sxs-lookup"><span data-stu-id="85dbb-106">In particular, it defines how object in source directory should be matched with an object in target directory, what (if any) scoping filters should be used to decide if we want to provision a given object, and how object attributes should be transformed going from source to target directory.</span></span>

<span data-ttu-id="85dbb-107">Объект сопоставления являются основной части [правила синхронизации](synchronization-synchronizationrule.md) и обновляются в процессе [синхронизации схемы](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="85dbb-107">Object mappings are the main part of the [synchronization rule](synchronization-synchronizationrule.md) and are updated as part of [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="85dbb-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="85dbb-108">Properties</span></span>

| <span data-ttu-id="85dbb-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="85dbb-109">Property</span></span>      | <span data-ttu-id="85dbb-110">Тип</span><span class="sxs-lookup"><span data-stu-id="85dbb-110">Type</span></span>      | <span data-ttu-id="85dbb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="85dbb-111">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="85dbb-112">attributeMappings</span><span class="sxs-lookup"><span data-stu-id="85dbb-112">attributeMappings</span></span>  |<span data-ttu-id="85dbb-113">[attributeMapping](synchronization-attributemapping.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="85dbb-113">[attributeMapping](synchronization-attributemapping.md) collection</span></span>    | <span data-ttu-id="85dbb-114">Сопоставление атрибут определяет атрибуты для сопоставления из исходного объекта в целевой объект и как поток.</span><span class="sxs-lookup"><span data-stu-id="85dbb-114">Attribute mappings define which attributes to map from the source object into the target object and how they should flow.</span></span> <span data-ttu-id="85dbb-115">Ряд функций доступны для поддержки преобразования исходных значений источника.</span><span class="sxs-lookup"><span data-stu-id="85dbb-115">A number of functions are available to support the transformation of the original source values.</span></span>|
|<span data-ttu-id="85dbb-116">enabled</span><span class="sxs-lookup"><span data-stu-id="85dbb-116">enabled</span></span>        |<span data-ttu-id="85dbb-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="85dbb-117">Boolean</span></span>    |<span data-ttu-id="85dbb-118">При `true`, это сопоставление объектов будут обрабатываться во время синхронизации.</span><span class="sxs-lookup"><span data-stu-id="85dbb-118">When `true`, this object mapping will be processed during synchronization.</span></span> <span data-ttu-id="85dbb-119">При `false`, это сопоставление объектов будет пропущено.</span><span class="sxs-lookup"><span data-stu-id="85dbb-119">When `false`, this object mapping will be skipped.</span></span>|
|<span data-ttu-id="85dbb-120">flowTypes</span><span class="sxs-lookup"><span data-stu-id="85dbb-120">flowTypes</span></span>      |<span data-ttu-id="85dbb-121">objectFlowType</span><span class="sxs-lookup"><span data-stu-id="85dbb-121">objectFlowType</span></span>    |<span data-ttu-id="85dbb-122">Какие типы потока включены для данного объекта сопоставления.</span><span class="sxs-lookup"><span data-stu-id="85dbb-122">Which flow types are enabled for this object mapping.</span></span> <span data-ttu-id="85dbb-123">`Add`создает новые объекты в целевой каталог `Update` изменяет существующие объекты и `Delete` deprovisions существующих пользователей.</span><span class="sxs-lookup"><span data-stu-id="85dbb-123">`Add` creates new objects in the target directory, `Update` modifies existing objects, and `Delete` deprovisions existing users.</span></span> <span data-ttu-id="85dbb-124">Значение по умолчанию — `Add, Update, Delete`.</span><span class="sxs-lookup"><span data-stu-id="85dbb-124">The default is `Add, Update, Delete`.</span></span> |
|<span data-ttu-id="85dbb-125">Метаданные</span><span class="sxs-lookup"><span data-stu-id="85dbb-125">metadata</span></span>       |<span data-ttu-id="85dbb-126">metadataEntry коллекции</span><span class="sxs-lookup"><span data-stu-id="85dbb-126">metadataEntry collection</span></span>    |<span data-ttu-id="85dbb-127">Расширение дополнительные свойства.</span><span class="sxs-lookup"><span data-stu-id="85dbb-127">Additional extension properties.</span></span> <span data-ttu-id="85dbb-128">Если не указан явно, значения метаданных не должно изменяться.</span><span class="sxs-lookup"><span data-stu-id="85dbb-128">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="85dbb-129">name</span><span class="sxs-lookup"><span data-stu-id="85dbb-129">name</span></span>           |<span data-ttu-id="85dbb-130">String</span><span class="sxs-lookup"><span data-stu-id="85dbb-130">String</span></span>     |<span data-ttu-id="85dbb-131">Отдел понятное имя объекта сопоставления.</span><span class="sxs-lookup"><span data-stu-id="85dbb-131">Human-friendly name of the object mapping.</span></span>|
|<span data-ttu-id="85dbb-132">scope</span><span class="sxs-lookup"><span data-stu-id="85dbb-132">scope</span></span>          |[<span data-ttu-id="85dbb-133">filter</span><span class="sxs-lookup"><span data-stu-id="85dbb-133">filter</span></span>](synchronization-filter.md)     |<span data-ttu-id="85dbb-134">Определяет фильтр для использования при принятии решения должны быть подготовлен того или иного объекта.</span><span class="sxs-lookup"><span data-stu-id="85dbb-134">Defines a filter to be used when deciding whether a given object should be provisioned.</span></span> <span data-ttu-id="85dbb-135">Например может потребоваться только подготовки пользователей, которые расположены в США.</span><span class="sxs-lookup"><span data-stu-id="85dbb-135">For example, you might want to only provision users that are located in the US.</span></span>|
|<span data-ttu-id="85dbb-136">sourceObjectName</span><span class="sxs-lookup"><span data-stu-id="85dbb-136">sourceObjectName</span></span>           |<span data-ttu-id="85dbb-137">String</span><span class="sxs-lookup"><span data-stu-id="85dbb-137">String</span></span>     |<span data-ttu-id="85dbb-138">Имя объекта в исходный каталог.</span><span class="sxs-lookup"><span data-stu-id="85dbb-138">Name of the object in the source directory.</span></span> <span data-ttu-id="85dbb-139">Должно совпадать с именем объекта из исходного [каталога определения](synchronization-directorydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="85dbb-139">Must match the object name from the source [directory definition](synchronization-directorydefinition.md).</span></span>|
|<span data-ttu-id="85dbb-140">targetObjectName</span><span class="sxs-lookup"><span data-stu-id="85dbb-140">targetObjectName</span></span>           |<span data-ttu-id="85dbb-141">String</span><span class="sxs-lookup"><span data-stu-id="85dbb-141">String</span></span>     |<span data-ttu-id="85dbb-142">Имя объекта в целевой каталог.</span><span class="sxs-lookup"><span data-stu-id="85dbb-142">Name of the object in target directory.</span></span> <span data-ttu-id="85dbb-143">Должно совпадать с именем объекта из целевого [каталога определения](synchronization-directorydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="85dbb-143">Must match the object name from the target [directory definition](synchronization-directorydefinition.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="85dbb-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="85dbb-144">JSON representation</span></span>

<span data-ttu-id="85dbb-145">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="85dbb-145">The following is a JSON representation of the resource.</span></span>

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

## <a name="json-example"></a><span data-ttu-id="85dbb-146">Пример JSON</span><span class="sxs-lookup"><span data-stu-id="85dbb-146">JSON Example</span></span>

<!-- {
  "blockType": "resource",
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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-objectmapping.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
