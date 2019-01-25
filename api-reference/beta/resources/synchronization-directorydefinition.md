---
title: Тип ресурса directoryDefinition
description: Предоставляет синхронизации сведения о каталоге и его объекты. Этот ресурс сообщает о том, обработчик синхронизации, например, что папка содержит объекты с именами **пользователей** и **группы**, какие атрибуты поддерживаются для этих объектов и типы для этих атрибутов. Чтобы объектов и атрибутов для участия в объект сопоставления и правила синхронизации они должны быть определены как часть определения каталогов.
localization_priority: Normal
ms.openlocfilehash: 22ba4a7f3b5b5d3154ec6b3f5d42bd6f1b8f09d7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508127"
---
# <a name="directorydefinition-resource-type"></a><span data-ttu-id="12f35-105">Тип ресурса directoryDefinition</span><span class="sxs-lookup"><span data-stu-id="12f35-105">directoryDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12f35-106">Предоставляет синхронизации сведения о каталоге и его объекты.</span><span class="sxs-lookup"><span data-stu-id="12f35-106">Provides the synchronization engine information about a directory and its objects.</span></span> <span data-ttu-id="12f35-107">Этот ресурс сообщает о том, обработчик синхронизации, например, что папка содержит объекты с именами **пользователей** и **группы**, какие атрибуты поддерживаются для этих объектов и типы для этих атрибутов.</span><span class="sxs-lookup"><span data-stu-id="12f35-107">This resource tells the synchronization engine, for example, that the directory has objects named **user** and **group**, which attributes are supported for those objects, and the types for those attributes.</span></span> <span data-ttu-id="12f35-108">Чтобы объектов и атрибутов для участия в [объект сопоставления](synchronization-objectmapping.md)и [правила синхронизации](synchronization-synchronizationrule.md) они должны быть определены как часть определения каталогов.</span><span class="sxs-lookup"><span data-stu-id="12f35-108">In order for the object and attribute to participate in [synchronization rules](synchronization-synchronizationrule.md) and [object mappings](synchronization-objectmapping.md), they must be defined as part of the directory definition.</span></span>

<span data-ttu-id="12f35-109">Как правило, по умолчанию [схемы синхронизации](synchronization-synchronizationschema.md) , поставляемые как часть [шаблона синхронизации](synchronization-synchronizationtemplate.md) будет определить наиболее часто используемые объекты и атрибуты для этого каталога.</span><span class="sxs-lookup"><span data-stu-id="12f35-109">In general, the default [synchronization schema](synchronization-synchronizationschema.md) provided as part of the [synchronization template](synchronization-synchronizationtemplate.md) will define most commonly used objects and attributes for that directory.</span></span> <span data-ttu-id="12f35-110">Тем не менее если каталог поддерживает добавление настраиваемых атрибутов, может потребоваться расширить определение по умолчанию в настраиваемых объектов и атрибутов.</span><span class="sxs-lookup"><span data-stu-id="12f35-110">However, if the directory supports the addition of custom attributes, you might want to expand the default definition with your own custom objects or attributes.</span></span> <span data-ttu-id="12f35-111">Для получения дополнительных сведений см. [Настройка синхронизации с помощью настраиваемых атрибутов](synchronization-configure-with-custom-target-attributes.md) и [Настройка синхронизации с расширением атрибутов каталога](synchronization-configure-with-directory-extension-attributes.md).</span><span class="sxs-lookup"><span data-stu-id="12f35-111">For more information, see [Configure synchronization with custom attributes](synchronization-configure-with-custom-target-attributes.md) and [Configure synchronization with directory extension attributes](synchronization-configure-with-directory-extension-attributes.md).</span></span>

<span data-ttu-id="12f35-112">Каталог определения обновляются в процессе [синхронизации схемы](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="12f35-112">Directory definitions are updated as part of the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="12f35-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="12f35-113">Properties</span></span>

| <span data-ttu-id="12f35-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="12f35-114">Property</span></span>      | <span data-ttu-id="12f35-115">Тип</span><span class="sxs-lookup"><span data-stu-id="12f35-115">Type</span></span>      | <span data-ttu-id="12f35-116">Описание</span><span class="sxs-lookup"><span data-stu-id="12f35-116">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="12f35-117">id</span><span class="sxs-lookup"><span data-stu-id="12f35-117">id</span></span>           |<span data-ttu-id="12f35-118">String</span><span class="sxs-lookup"><span data-stu-id="12f35-118">String</span></span>     |<span data-ttu-id="12f35-119">Идентификатор папки.</span><span class="sxs-lookup"><span data-stu-id="12f35-119">Directory identifier.</span></span> <span data-ttu-id="12f35-120">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="12f35-120">Not nullable.</span></span>|
|<span data-ttu-id="12f35-121">Метаданные</span><span class="sxs-lookup"><span data-stu-id="12f35-121">metadata</span></span>       |<span data-ttu-id="12f35-122">metadataEntry коллекции</span><span class="sxs-lookup"><span data-stu-id="12f35-122">metadataEntry collection</span></span>    |<span data-ttu-id="12f35-123">Расширение дополнительные свойства.</span><span class="sxs-lookup"><span data-stu-id="12f35-123">Additional extension properties.</span></span> <span data-ttu-id="12f35-124">Если не указан явно, значения метаданных не должно изменяться.</span><span class="sxs-lookup"><span data-stu-id="12f35-124">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="12f35-125">name</span><span class="sxs-lookup"><span data-stu-id="12f35-125">name</span></span>           |<span data-ttu-id="12f35-126">String</span><span class="sxs-lookup"><span data-stu-id="12f35-126">String</span></span>     |<span data-ttu-id="12f35-127">Имя каталога.</span><span class="sxs-lookup"><span data-stu-id="12f35-127">Name of the directory.</span></span> <span data-ttu-id="12f35-128">Должно быть уникальным в рамках [схемы синхронизации](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="12f35-128">Must be unique within the [synchronization schema](synchronization-synchronizationschema.md).</span></span> <span data-ttu-id="12f35-129">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="12f35-129">Not nullable.</span></span>|
|<span data-ttu-id="12f35-130">Объекты</span><span class="sxs-lookup"><span data-stu-id="12f35-130">objects</span></span>        |<span data-ttu-id="12f35-131">[objectDefinition](synchronization-objectdefinition.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="12f35-131">[objectDefinition](synchronization-objectdefinition.md) collection</span></span>    |<span data-ttu-id="12f35-132">Коллекция объектов, поддерживаемых в каталоге.</span><span class="sxs-lookup"><span data-stu-id="12f35-132">Collection of objects supported by the directory.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="12f35-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="12f35-133">JSON representation</span></span>

<span data-ttu-id="12f35-134">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="12f35-134">The following is a JSON representation of the resource.</span></span>

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

## <a name="json-example"></a><span data-ttu-id="12f35-135">Пример JSON</span><span class="sxs-lookup"><span data-stu-id="12f35-135">JSON Example</span></span>

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
