---
title: Тип ресурса directoryDefinition
description: Предоставляет синхронизации сведения о каталоге и его объекты. Этот ресурс сообщает о том, обработчик синхронизации, например, что папка содержит объекты с именами **пользователей** и **группы**, какие атрибуты поддерживаются для этих объектов и типы для этих атрибутов. Чтобы объектов и атрибутов для участия в объект сопоставления и правила синхронизации они должны быть определены как часть определения каталогов.
localization_priority: Normal
ms.openlocfilehash: e6b2b55fb9e9e7963b01403c6aed2f0997e2318b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874524"
---
# <a name="directorydefinition-resource-type"></a><span data-ttu-id="7ac0a-105">Тип ресурса directoryDefinition</span><span class="sxs-lookup"><span data-stu-id="7ac0a-105">directoryDefinition resource type</span></span>

> <span data-ttu-id="7ac0a-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7ac0a-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7ac0a-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ac0a-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7ac0a-108">Предоставляет синхронизации сведения о каталоге и его объекты.</span><span class="sxs-lookup"><span data-stu-id="7ac0a-108">Provides the synchronization engine information about a directory and its objects.</span></span> <span data-ttu-id="7ac0a-109">Этот ресурс сообщает о том, обработчик синхронизации, например, что папка содержит объекты с именами **пользователей** и **группы**, какие атрибуты поддерживаются для этих объектов и типы для этих атрибутов.</span><span class="sxs-lookup"><span data-stu-id="7ac0a-109">This resource tells the synchronization engine, for example, that the directory has objects named **user** and **group**, which attributes are supported for those objects, and the types for those attributes.</span></span> <span data-ttu-id="7ac0a-110">Чтобы объектов и атрибутов для участия в [объект сопоставления](synchronization-objectmapping.md)и [правила синхронизации](synchronization-synchronizationrule.md) они должны быть определены как часть определения каталогов.</span><span class="sxs-lookup"><span data-stu-id="7ac0a-110">In order for the object and attribute to participate in [synchronization rules](synchronization-synchronizationrule.md) and [object mappings](synchronization-objectmapping.md), they must be defined as part of the directory definition.</span></span>

<span data-ttu-id="7ac0a-111">Как правило, по умолчанию [схемы синхронизации](synchronization-synchronizationschema.md) , поставляемые как часть [шаблона синхронизации](synchronization-synchronizationtemplate.md) будет определить наиболее часто используемые объекты и атрибуты для этого каталога.</span><span class="sxs-lookup"><span data-stu-id="7ac0a-111">In general, the default [synchronization schema](synchronization-synchronizationschema.md) provided as part of the [synchronization template](synchronization-synchronizationtemplate.md) will define most commonly used objects and attributes for that directory.</span></span> <span data-ttu-id="7ac0a-112">Тем не менее если каталог поддерживает добавление настраиваемых атрибутов, может потребоваться расширить определение по умолчанию в настраиваемых объектов и атрибутов.</span><span class="sxs-lookup"><span data-stu-id="7ac0a-112">However, if the directory supports the addition of custom attributes, you might want to expand the default definition with your own custom objects or attributes.</span></span> <span data-ttu-id="7ac0a-113">Для получения дополнительных сведений см. [Настройка синхронизации с помощью настраиваемых атрибутов](synchronization-configure-with-custom-target-attributes.md) и [Настройка синхронизации с расширением атрибутов каталога](synchronization-configure-with-directory-extension-attributes.md).</span><span class="sxs-lookup"><span data-stu-id="7ac0a-113">For more information, see [Configure synchronization with custom attributes](synchronization-configure-with-custom-target-attributes.md) and [Configure synchronization with directory extension attributes](synchronization-configure-with-directory-extension-attributes.md).</span></span>

<span data-ttu-id="7ac0a-114">Каталог определения обновляются в процессе [синхронизации схемы](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="7ac0a-114">Directory definitions are updated as part of the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7ac0a-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="7ac0a-115">Properties</span></span>

| <span data-ttu-id="7ac0a-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="7ac0a-116">Property</span></span>      | <span data-ttu-id="7ac0a-117">Тип</span><span class="sxs-lookup"><span data-stu-id="7ac0a-117">Type</span></span>      | <span data-ttu-id="7ac0a-118">Описание</span><span class="sxs-lookup"><span data-stu-id="7ac0a-118">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="7ac0a-119">id</span><span class="sxs-lookup"><span data-stu-id="7ac0a-119">id</span></span>           |<span data-ttu-id="7ac0a-120">Строка</span><span class="sxs-lookup"><span data-stu-id="7ac0a-120">String</span></span>     |<span data-ttu-id="7ac0a-121">Идентификатор папки.</span><span class="sxs-lookup"><span data-stu-id="7ac0a-121">Directory identifier.</span></span> <span data-ttu-id="7ac0a-122">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="7ac0a-122">Not nullable.</span></span>|
|<span data-ttu-id="7ac0a-123">метаданные</span><span class="sxs-lookup"><span data-stu-id="7ac0a-123">metadata</span></span>       |<span data-ttu-id="7ac0a-124">metadataEntry коллекции</span><span class="sxs-lookup"><span data-stu-id="7ac0a-124">metadataEntry collection</span></span>    |<span data-ttu-id="7ac0a-125">Расширение дополнительные свойства.</span><span class="sxs-lookup"><span data-stu-id="7ac0a-125">Additional extension properties.</span></span> <span data-ttu-id="7ac0a-126">Если не указан явно, значения метаданных не должно изменяться.</span><span class="sxs-lookup"><span data-stu-id="7ac0a-126">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="7ac0a-127">name</span><span class="sxs-lookup"><span data-stu-id="7ac0a-127">name</span></span>           |<span data-ttu-id="7ac0a-128">Строка</span><span class="sxs-lookup"><span data-stu-id="7ac0a-128">String</span></span>     |<span data-ttu-id="7ac0a-129">Имя каталога.</span><span class="sxs-lookup"><span data-stu-id="7ac0a-129">Name of the directory.</span></span> <span data-ttu-id="7ac0a-130">Должно быть уникальным в рамках [схемы синхронизации](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="7ac0a-130">Must be unique within the [synchronization schema](synchronization-synchronizationschema.md).</span></span> <span data-ttu-id="7ac0a-131">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="7ac0a-131">Not nullable.</span></span>|
|<span data-ttu-id="7ac0a-132">объекты</span><span class="sxs-lookup"><span data-stu-id="7ac0a-132">objects</span></span>        |<span data-ttu-id="7ac0a-133">[objectDefinition](synchronization-objectdefinition.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="7ac0a-133">[objectDefinition](synchronization-objectdefinition.md) collection</span></span>    |<span data-ttu-id="7ac0a-134">Коллекция объектов, поддерживаемых в каталоге.</span><span class="sxs-lookup"><span data-stu-id="7ac0a-134">Collection of objects supported by the directory.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7ac0a-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7ac0a-135">JSON representation</span></span>

<span data-ttu-id="7ac0a-136">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7ac0a-136">The following is a JSON representation of the resource.</span></span>

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

## <a name="json-example"></a><span data-ttu-id="7ac0a-137">Пример JSON</span><span class="sxs-lookup"><span data-stu-id="7ac0a-137">JSON Example</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "directoryDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
