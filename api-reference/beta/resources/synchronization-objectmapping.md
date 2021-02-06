---
title: Тип ресурса objectMapping
description: Определяет, как следует синхронизировать заданный объект из каталога источника в целевой каталог.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 94aa85c198ea67a4c53fc5b56d342188835b0ace
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133186"
---
# <a name="objectmapping-resource-type"></a><span data-ttu-id="c98bc-103">Тип ресурса objectMapping</span><span class="sxs-lookup"><span data-stu-id="c98bc-103">objectMapping resource type</span></span>

<span data-ttu-id="c98bc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c98bc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c98bc-105">Определяет, как следует синхронизировать заданный объект из каталога источника в целевой каталог.</span><span class="sxs-lookup"><span data-stu-id="c98bc-105">Defines how a given object should be synchronized from source directory to target directory.</span></span> <span data-ttu-id="c98bc-106">В частности, он определяет, как объект в каталоге источника должен быть совмедан с объектом в целевом каталоге, какие (при их наряду) фильтры области следует использовать для временного решения о том, нужно ли нам подготовка конкретного объекта, и как следует преобразовывать атрибуты объекта из источника в целевой каталог.</span><span class="sxs-lookup"><span data-stu-id="c98bc-106">In particular, it defines how object in source directory should be matched with an object in target directory, what (if any) scoping filters should be used to decide if we want to provision a given object, and how object attributes should be transformed going from source to target directory.</span></span>

<span data-ttu-id="c98bc-107">Сопоставления объектов являются основной [](synchronization-synchronizationrule.md) частью правила синхронизации и обновляются в рамках [схемы синхронизации.](synchronization-synchronizationschema.md)</span><span class="sxs-lookup"><span data-stu-id="c98bc-107">Object mappings are the main part of the [synchronization rule](synchronization-synchronizationrule.md) and are updated as part of [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c98bc-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c98bc-108">Properties</span></span>

| <span data-ttu-id="c98bc-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c98bc-109">Property</span></span>      | <span data-ttu-id="c98bc-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c98bc-110">Type</span></span>      | <span data-ttu-id="c98bc-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c98bc-111">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="c98bc-112">attributeMappings</span><span class="sxs-lookup"><span data-stu-id="c98bc-112">attributeMappings</span></span>  |<span data-ttu-id="c98bc-113">[Коллекция attributeMapping](synchronization-attributemapping.md)</span><span class="sxs-lookup"><span data-stu-id="c98bc-113">[attributeMapping](synchronization-attributemapping.md) collection</span></span>    | <span data-ttu-id="c98bc-114">Сопоставления атрибутов определяют, какие атрибуты соотнося из объекта-источника в целевой объект и как они должны поступать.</span><span class="sxs-lookup"><span data-stu-id="c98bc-114">Attribute mappings define which attributes to map from the source object into the target object and how they should flow.</span></span> <span data-ttu-id="c98bc-115">Для поддержки преобразования исходных исходных значений доступно несколько функций.</span><span class="sxs-lookup"><span data-stu-id="c98bc-115">A number of functions are available to support the transformation of the original source values.</span></span>|
|<span data-ttu-id="c98bc-116">enabled</span><span class="sxs-lookup"><span data-stu-id="c98bc-116">enabled</span></span>        |<span data-ttu-id="c98bc-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="c98bc-117">Boolean</span></span>    |<span data-ttu-id="c98bc-118">Когда `true` это сопоставление объектов будет обработано во время синхронизации.</span><span class="sxs-lookup"><span data-stu-id="c98bc-118">When `true`, this object mapping will be processed during synchronization.</span></span> <span data-ttu-id="c98bc-119">Когда `false` это сопоставление объектов будет пропущено.</span><span class="sxs-lookup"><span data-stu-id="c98bc-119">When `false`, this object mapping will be skipped.</span></span>|
|<span data-ttu-id="c98bc-120">flowTypes</span><span class="sxs-lookup"><span data-stu-id="c98bc-120">flowTypes</span></span>      |<span data-ttu-id="c98bc-121">objectFlowTypes</span><span class="sxs-lookup"><span data-stu-id="c98bc-121">objectFlowTypes</span></span>    |<span data-ttu-id="c98bc-122">Типы потоков, которые включены для этого сопоставления объектов.</span><span class="sxs-lookup"><span data-stu-id="c98bc-122">Which flow types are enabled for this object mapping.</span></span> <span data-ttu-id="c98bc-123">`Add` создает новые объекты в целевом каталоге, изменяет существующие объекты `Update` и отгвоирует `Delete` существующих пользователей.</span><span class="sxs-lookup"><span data-stu-id="c98bc-123">`Add` creates new objects in the target directory, `Update` modifies existing objects, and `Delete` deprovisions existing users.</span></span> <span data-ttu-id="c98bc-124">Значение по `Add, Update, Delete` умолчанию: .</span><span class="sxs-lookup"><span data-stu-id="c98bc-124">The default is `Add, Update, Delete`.</span></span> |
|<span data-ttu-id="c98bc-125">метаданные</span><span class="sxs-lookup"><span data-stu-id="c98bc-125">metadata</span></span>       |<span data-ttu-id="c98bc-126">Коллекция metadataEntry</span><span class="sxs-lookup"><span data-stu-id="c98bc-126">metadataEntry collection</span></span>    |<span data-ttu-id="c98bc-127">Дополнительные свойства расширения.</span><span class="sxs-lookup"><span data-stu-id="c98bc-127">Additional extension properties.</span></span> <span data-ttu-id="c98bc-128">Если не было явно упомянуто, значения метаданных не следует менять.</span><span class="sxs-lookup"><span data-stu-id="c98bc-128">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="c98bc-129">name</span><span class="sxs-lookup"><span data-stu-id="c98bc-129">name</span></span>           |<span data-ttu-id="c98bc-130">String</span><span class="sxs-lookup"><span data-stu-id="c98bc-130">String</span></span>     |<span data-ttu-id="c98bc-131">Удобное для человека имя сопоставления объектов.</span><span class="sxs-lookup"><span data-stu-id="c98bc-131">Human-friendly name of the object mapping.</span></span>|
|<span data-ttu-id="c98bc-132">scope</span><span class="sxs-lookup"><span data-stu-id="c98bc-132">scope</span></span>          |[<span data-ttu-id="c98bc-133">filter</span><span class="sxs-lookup"><span data-stu-id="c98bc-133">filter</span></span>](synchronization-filter.md)     |<span data-ttu-id="c98bc-134">Определяет фильтр, который будет использоваться при принятии решения о том, следует ли подготовка данного объекта.</span><span class="sxs-lookup"><span data-stu-id="c98bc-134">Defines a filter to be used when deciding whether a given object should be provisioned.</span></span> <span data-ttu-id="c98bc-135">Например, может потребоваться только подготовка пользователей, расположенных в США.</span><span class="sxs-lookup"><span data-stu-id="c98bc-135">For example, you might want to only provision users that are located in the US.</span></span>|
|<span data-ttu-id="c98bc-136">sourceObjectName</span><span class="sxs-lookup"><span data-stu-id="c98bc-136">sourceObjectName</span></span>           |<span data-ttu-id="c98bc-137">Строка</span><span class="sxs-lookup"><span data-stu-id="c98bc-137">String</span></span>     |<span data-ttu-id="c98bc-138">Имя объекта в каталоге источника.</span><span class="sxs-lookup"><span data-stu-id="c98bc-138">Name of the object in the source directory.</span></span> <span data-ttu-id="c98bc-139">Должен соответствовать имени объекта из определения [источника каталога.](synchronization-directorydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c98bc-139">Must match the object name from the source [directory definition](synchronization-directorydefinition.md).</span></span>|
|<span data-ttu-id="c98bc-140">targetObjectName</span><span class="sxs-lookup"><span data-stu-id="c98bc-140">targetObjectName</span></span>           |<span data-ttu-id="c98bc-141">Строка</span><span class="sxs-lookup"><span data-stu-id="c98bc-141">String</span></span>     |<span data-ttu-id="c98bc-142">Имя объекта в целевом каталоге.</span><span class="sxs-lookup"><span data-stu-id="c98bc-142">Name of the object in target directory.</span></span> <span data-ttu-id="c98bc-143">Должен соответствовать имени объекта из определения [целевого каталога.](synchronization-directorydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c98bc-143">Must match the object name from the target [directory definition](synchronization-directorydefinition.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c98bc-144">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c98bc-144">JSON representation</span></span>

<span data-ttu-id="c98bc-145">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c98bc-145">The following is a JSON representation of the resource.</span></span>

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

## <a name="json-example"></a><span data-ttu-id="c98bc-146">Пример JSON</span><span class="sxs-lookup"><span data-stu-id="c98bc-146">JSON Example</span></span>

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


