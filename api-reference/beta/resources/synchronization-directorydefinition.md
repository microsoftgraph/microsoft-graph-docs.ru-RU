---
title: Тип ресурса Директоридефинитион
description: Предоставляет сведения о модуле синхронизации для каталога и его объектов. Этот ресурс сообщает обработчику синхронизации, например, что каталог содержит объекты с именем **User** и **Group**, какие атрибуты поддерживаются для этих объектов, и типы этих атрибутов. Чтобы объект и атрибут участвовали в правилах синхронизации и сопоставлениях объектов, они должны быть определены как часть определения каталога.
localization_priority: Normal
ms.openlocfilehash: 22ba4a7f3b5b5d3154ec6b3f5d42bd6f1b8f09d7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582068"
---
# <a name="directorydefinition-resource-type"></a><span data-ttu-id="5a919-105">Тип ресурса Директоридефинитион</span><span class="sxs-lookup"><span data-stu-id="5a919-105">directoryDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a919-106">Предоставляет сведения о модуле синхронизации для каталога и его объектов.</span><span class="sxs-lookup"><span data-stu-id="5a919-106">Provides the synchronization engine information about a directory and its objects.</span></span> <span data-ttu-id="5a919-107">Этот ресурс сообщает обработчику синхронизации, например, что каталог содержит объекты с именем **User** и **Group**, какие атрибуты поддерживаются для этих объектов, и типы этих атрибутов.</span><span class="sxs-lookup"><span data-stu-id="5a919-107">This resource tells the synchronization engine, for example, that the directory has objects named **user** and **group**, which attributes are supported for those objects, and the types for those attributes.</span></span> <span data-ttu-id="5a919-108">Чтобы объект и атрибут участвовали в [правилах синхронизации](synchronization-synchronizationrule.md) и сопоставлениях [объектов](synchronization-objectmapping.md), они должны быть определены как часть определения каталога.</span><span class="sxs-lookup"><span data-stu-id="5a919-108">In order for the object and attribute to participate in [synchronization rules](synchronization-synchronizationrule.md) and [object mappings](synchronization-objectmapping.md), they must be defined as part of the directory definition.</span></span>

<span data-ttu-id="5a919-109">Как правило, [схема синхронизации](synchronization-synchronizationschema.md) по умолчанию, предоставляемая как часть [шаблона синхронизации](synchronization-synchronizationtemplate.md) , определяет наиболее часто используемые объекты и атрибуты для этого каталога.</span><span class="sxs-lookup"><span data-stu-id="5a919-109">In general, the default [synchronization schema](synchronization-synchronizationschema.md) provided as part of the [synchronization template](synchronization-synchronizationtemplate.md) will define most commonly used objects and attributes for that directory.</span></span> <span data-ttu-id="5a919-110">Тем не менее, если каталог поддерживает добавление настраиваемых атрибутов, можно расширить определение DEFAULT с использованием собственных настраиваемых объектов или атрибутов.</span><span class="sxs-lookup"><span data-stu-id="5a919-110">However, if the directory supports the addition of custom attributes, you might want to expand the default definition with your own custom objects or attributes.</span></span> <span data-ttu-id="5a919-111">Дополнительные сведения см. в статье [Настройка синхронизации с настраиваемыми атрибутами](synchronization-configure-with-custom-target-attributes.md) и [Настройка синхронизации с атрибутами расширения каталога](synchronization-configure-with-directory-extension-attributes.md).</span><span class="sxs-lookup"><span data-stu-id="5a919-111">For more information, see [Configure synchronization with custom attributes](synchronization-configure-with-custom-target-attributes.md) and [Configure synchronization with directory extension attributes](synchronization-configure-with-directory-extension-attributes.md).</span></span>

<span data-ttu-id="5a919-112">Определения каталогов обновляются в составе [схемы синхронизации](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="5a919-112">Directory definitions are updated as part of the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5a919-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="5a919-113">Properties</span></span>

| <span data-ttu-id="5a919-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="5a919-114">Property</span></span>      | <span data-ttu-id="5a919-115">Тип</span><span class="sxs-lookup"><span data-stu-id="5a919-115">Type</span></span>      | <span data-ttu-id="5a919-116">Описание</span><span class="sxs-lookup"><span data-stu-id="5a919-116">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="5a919-117">id</span><span class="sxs-lookup"><span data-stu-id="5a919-117">id</span></span>           |<span data-ttu-id="5a919-118">Строка</span><span class="sxs-lookup"><span data-stu-id="5a919-118">String</span></span>     |<span data-ttu-id="5a919-119">Идентификатор каталога.</span><span class="sxs-lookup"><span data-stu-id="5a919-119">Directory identifier.</span></span> <span data-ttu-id="5a919-120">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="5a919-120">Not nullable.</span></span>|
|<span data-ttu-id="5a919-121">метаданных</span><span class="sxs-lookup"><span data-stu-id="5a919-121">metadata</span></span>       |<span data-ttu-id="5a919-122">Коллекция Метадатаентри</span><span class="sxs-lookup"><span data-stu-id="5a919-122">metadataEntry collection</span></span>    |<span data-ttu-id="5a919-123">Дополнительные свойства расширения.</span><span class="sxs-lookup"><span data-stu-id="5a919-123">Additional extension properties.</span></span> <span data-ttu-id="5a919-124">Если явно не указано иное, значения метаданных не должны изменяться.</span><span class="sxs-lookup"><span data-stu-id="5a919-124">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="5a919-125">name</span><span class="sxs-lookup"><span data-stu-id="5a919-125">name</span></span>           |<span data-ttu-id="5a919-126">String</span><span class="sxs-lookup"><span data-stu-id="5a919-126">String</span></span>     |<span data-ttu-id="5a919-127">Имя каталога.</span><span class="sxs-lookup"><span data-stu-id="5a919-127">Name of the directory.</span></span> <span data-ttu-id="5a919-128">Должно быть уникальным в пределах [схемы синхронизации](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="5a919-128">Must be unique within the [synchronization schema](synchronization-synchronizationschema.md).</span></span> <span data-ttu-id="5a919-129">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="5a919-129">Not nullable.</span></span>|
|<span data-ttu-id="5a919-130">см</span><span class="sxs-lookup"><span data-stu-id="5a919-130">objects</span></span>        |<span data-ttu-id="5a919-131">Коллекция [обжектдефинитион](synchronization-objectdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5a919-131">[objectDefinition](synchronization-objectdefinition.md) collection</span></span>    |<span data-ttu-id="5a919-132">Коллекция объектов, поддерживаемая каталогом.</span><span class="sxs-lookup"><span data-stu-id="5a919-132">Collection of objects supported by the directory.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5a919-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5a919-133">JSON representation</span></span>

<span data-ttu-id="5a919-134">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5a919-134">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directoryDefinition"
}-->

```json
{
  "id": "String",
  "name": "String",
  "objects": [{"@odata.type": "microsoft.graph.objectDefinition"}]
}

```

## <a name="json-example"></a><span data-ttu-id="5a919-135">Пример JSON</span><span class="sxs-lookup"><span data-stu-id="5a919-135">JSON Example</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directoryDefinition"
}-->

```json
{
    "id": "8ffa6169-f354-4751-9b77-9c00765be92d",
    "name": "salesforce.com",
    "objects": [
        {
            "attributes": [
                {
                    "anchor": true,
                    "name": "Id",
                    "type": "String"
                },
                {
                    "name": "IsActive",
                    "required": true,
                    "type": "Boolean"
                },
                {
                    "mutability": "ReadWrite",
                    "name": "Alias",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "CompanyName",
                    "type": "String"
                },
                {
                    "name": "CommunityNickname",
                    "type": "String"
                },
                {
                    "name": "Email",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "EmailEncodingKey",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "LanguageLocaleKey",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "FirstName",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "LastName",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "LocaleSidKey",
                    "required": true,
                    "type": "String"
                },
                {
                    "metadata": [
                        {
                            "key": "LinkTypeName",
                            "value": "PermissionSetAssignment"
                        },
                        {
                            "key": "LinkPropertyNames",
                            "value": "[\"PermissionSetId\"]"
                        }
                    ],
                    "name": "PermissionSets",
                    "referencedObjects": [
                        {
                            "referencedObjectName": "PermissionSet"
                        }
                    ],
                    "type": "Reference"
                },
                {
                    "name": "ProfileId",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "ProfileName",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "TimeZoneSidKey",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "Username",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "UserPermissionsCallCenterAutoLogin",
                    "required": true,
                    "type": "Boolean"
                },
                {
                    "name": "UserPermissionsMarketingUser",
                    "required": true,
                    "type": "Boolean"
                },
                {
                    "name": "Street",
                    "type": "String"
                },
                {
                    "name": "City",
                    "type": "String"
                },
                {
                    "name": "Division",
                    "type": "String"
                },
                {
                    "name": "EmployeeNumber",
                    "type": "String"
                },
                {
                    "name": "State",
                    "type": "String"
                },
                {
                    "name": "PostalCode",
                    "type": "String"
                },
                {
                    "name": "Country",
                    "type": "String"
                },
                {
                    "name": "Department",
                    "type": "String"
                },
                {
                    "name": "MobilePhone",
                    "type": "String"
                },
                {
                    "name": "Phone",
                    "type": "String"
                },
                {
                    "name": "Title",
                    "type": "String"
                },
                {
                    "name": "FederationIdentifier",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "ManagerId",
                    "referencedObjects": [
                        {
                            "referencedObjectName": "User"
                        }
                    ],
                    "type": "Reference"
                },
                {
                    "name": "UserRoleId",
                    "referencedObjects": [
                        {
                            "referencedObjectName": "UserRole"
                        }
                    ],
                    "type": "Reference"
                }
            ],
            "metadata": [
                {
                    "key": "IsSoftDeletionSupported",
                    "value": "false"
                },
                {
                    "key": "ConnectorDataStorageRequired",
                    "value": "false"
                },
                {
                    "key": "IsSynchronizeAllSupported",
                    "value": "false"
                }
            ],
            "name": "User"
        }
    ],
    "metadata": []
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-directorydefinition.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
