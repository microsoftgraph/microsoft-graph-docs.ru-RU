---
title: Тип ресурса Директоридефинитион
description: Предоставляет сведения о модуле синхронизации для каталога и его объектов. Этот ресурс сообщает обработчику синхронизации, например, что каталог содержит объекты с именем **User** и **Group**, какие атрибуты поддерживаются для этих объектов, и типы этих атрибутов. Чтобы объект и атрибут участвовали в правилах синхронизации и сопоставлениях объектов, они должны быть определены как часть определения каталога.
localization_priority: Normal
ms.openlocfilehash: 8e622edef39eec5476015ef5e22c5fe9697e0daa
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342932"
---
# <a name="directorydefinition-resource-type"></a><span data-ttu-id="bc283-105">Тип ресурса Директоридефинитион</span><span class="sxs-lookup"><span data-stu-id="bc283-105">directoryDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc283-106">Предоставляет сведения о модуле синхронизации для каталога и его объектов.</span><span class="sxs-lookup"><span data-stu-id="bc283-106">Provides the synchronization engine information about a directory and its objects.</span></span> <span data-ttu-id="bc283-107">Этот ресурс сообщает обработчику синхронизации, например, что каталог содержит объекты с именем **User** и **Group**, какие атрибуты поддерживаются для этих объектов, и типы этих атрибутов.</span><span class="sxs-lookup"><span data-stu-id="bc283-107">This resource tells the synchronization engine, for example, that the directory has objects named **user** and **group**, which attributes are supported for those objects, and the types for those attributes.</span></span> <span data-ttu-id="bc283-108">Чтобы объект и атрибут участвовали в [правилах синхронизации](synchronization-synchronizationrule.md) и сопоставлениях [объектов](synchronization-objectmapping.md), они должны быть определены как часть определения каталога.</span><span class="sxs-lookup"><span data-stu-id="bc283-108">In order for the object and attribute to participate in [synchronization rules](synchronization-synchronizationrule.md) and [object mappings](synchronization-objectmapping.md), they must be defined as part of the directory definition.</span></span>

<span data-ttu-id="bc283-109">Как правило, [схема синхронизации](synchronization-synchronizationschema.md) по умолчанию, предоставляемая как часть [шаблона синхронизации](synchronization-synchronizationtemplate.md) , определяет наиболее часто используемые объекты и атрибуты для этого каталога.</span><span class="sxs-lookup"><span data-stu-id="bc283-109">In general, the default [synchronization schema](synchronization-synchronizationschema.md) provided as part of the [synchronization template](synchronization-synchronizationtemplate.md) will define most commonly used objects and attributes for that directory.</span></span> <span data-ttu-id="bc283-110">Тем не менее, если каталог поддерживает добавление настраиваемых атрибутов, можно расширить определение DEFAULT с использованием собственных настраиваемых объектов или атрибутов.</span><span class="sxs-lookup"><span data-stu-id="bc283-110">However, if the directory supports the addition of custom attributes, you might want to expand the default definition with your own custom objects or attributes.</span></span> <span data-ttu-id="bc283-111">Дополнительные сведения см. в статье [Настройка синхронизации с настраиваемыми атрибутами](synchronization-configure-with-custom-target-attributes.md) и [Настройка синхронизации с атрибутами расширения каталога](synchronization-configure-with-directory-extension-attributes.md).</span><span class="sxs-lookup"><span data-stu-id="bc283-111">For more information, see [Configure synchronization with custom attributes](synchronization-configure-with-custom-target-attributes.md) and [Configure synchronization with directory extension attributes](synchronization-configure-with-directory-extension-attributes.md).</span></span>

<span data-ttu-id="bc283-112">Определения каталогов обновляются в составе [схемы синхронизации](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="bc283-112">Directory definitions are updated as part of the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="bc283-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="bc283-113">Properties</span></span>

| <span data-ttu-id="bc283-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="bc283-114">Property</span></span>      | <span data-ttu-id="bc283-115">Тип</span><span class="sxs-lookup"><span data-stu-id="bc283-115">Type</span></span>      | <span data-ttu-id="bc283-116">Описание</span><span class="sxs-lookup"><span data-stu-id="bc283-116">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="bc283-117">id</span><span class="sxs-lookup"><span data-stu-id="bc283-117">id</span></span>           |<span data-ttu-id="bc283-118">Строка</span><span class="sxs-lookup"><span data-stu-id="bc283-118">String</span></span>     |<span data-ttu-id="bc283-119">Идентификатор каталога.</span><span class="sxs-lookup"><span data-stu-id="bc283-119">Directory identifier.</span></span> <span data-ttu-id="bc283-120">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="bc283-120">Not nullable.</span></span>|
|<span data-ttu-id="bc283-121">метаданных</span><span class="sxs-lookup"><span data-stu-id="bc283-121">metadata</span></span>       |<span data-ttu-id="bc283-122">Коллекция Метадатаентри</span><span class="sxs-lookup"><span data-stu-id="bc283-122">metadataEntry collection</span></span>    |<span data-ttu-id="bc283-123">Дополнительные свойства расширения.</span><span class="sxs-lookup"><span data-stu-id="bc283-123">Additional extension properties.</span></span> <span data-ttu-id="bc283-124">Если явно не указано иное, значения метаданных не должны изменяться.</span><span class="sxs-lookup"><span data-stu-id="bc283-124">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="bc283-125">name</span><span class="sxs-lookup"><span data-stu-id="bc283-125">name</span></span>           |<span data-ttu-id="bc283-126">String</span><span class="sxs-lookup"><span data-stu-id="bc283-126">String</span></span>     |<span data-ttu-id="bc283-127">Имя каталога.</span><span class="sxs-lookup"><span data-stu-id="bc283-127">Name of the directory.</span></span> <span data-ttu-id="bc283-128">Должно быть уникальным в пределах [схемы синхронизации](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="bc283-128">Must be unique within the [synchronization schema](synchronization-synchronizationschema.md).</span></span> <span data-ttu-id="bc283-129">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="bc283-129">Not nullable.</span></span>|
|<span data-ttu-id="bc283-130">см</span><span class="sxs-lookup"><span data-stu-id="bc283-130">objects</span></span>        |<span data-ttu-id="bc283-131">Коллекция [обжектдефинитион](synchronization-objectdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="bc283-131">[objectDefinition](synchronization-objectdefinition.md) collection</span></span>    |<span data-ttu-id="bc283-132">Коллекция объектов, поддерживаемая каталогом.</span><span class="sxs-lookup"><span data-stu-id="bc283-132">Collection of objects supported by the directory.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bc283-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bc283-133">JSON representation</span></span>

<span data-ttu-id="bc283-134">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bc283-134">The following is a JSON representation of the resource.</span></span>

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

## <a name="json-example"></a><span data-ttu-id="bc283-135">Пример JSON</span><span class="sxs-lookup"><span data-stu-id="bc283-135">JSON Example</span></span>

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
  "suppressions": []
}
-->
