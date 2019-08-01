---
title: Тип ресурса extensionSchemaProperty
description: Ресурс **extensionSchemaProperty** используется для задания имени и типа свойства в качестве части определения schemaExtension.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 362072f8727d82e4b5b5744922d8b819e0eae079
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032538"
---
# <a name="extensionschemaproperty-resource-type"></a><span data-ttu-id="d3ce5-103">Тип ресурса extensionSchemaProperty</span><span class="sxs-lookup"><span data-stu-id="d3ce5-103">extensionSchemaProperty resource type</span></span>

<span data-ttu-id="d3ce5-104">Ресурс **extensionSchemaProperty** используется для задания имени и типа свойства в качестве части определения [schemaExtension](schemaextension.md).</span><span class="sxs-lookup"><span data-stu-id="d3ce5-104">Use the **extensionSchemaProperty** resource to define a property's name and its type, as part of a [schemaExtension](schemaextension.md) definition.</span></span>


## <a name="properties"></a><span data-ttu-id="d3ce5-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="d3ce5-105">Properties</span></span>
| <span data-ttu-id="d3ce5-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="d3ce5-106">Property</span></span>     | <span data-ttu-id="d3ce5-107">Тип</span><span class="sxs-lookup"><span data-stu-id="d3ce5-107">Type</span></span>   |<span data-ttu-id="d3ce5-108">Описание</span><span class="sxs-lookup"><span data-stu-id="d3ce5-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d3ce5-109">name</span><span class="sxs-lookup"><span data-stu-id="d3ce5-109">name</span></span>|<span data-ttu-id="d3ce5-110">String</span><span class="sxs-lookup"><span data-stu-id="d3ce5-110">String</span></span>| <span data-ttu-id="d3ce5-111">Имя строго типизированного свойства, определенного в качестве части расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="d3ce5-111">The name of the strongly-typed property defined as part of a schema extension.</span></span>|
|<span data-ttu-id="d3ce5-112">type</span><span class="sxs-lookup"><span data-stu-id="d3ce5-112">type</span></span>|<span data-ttu-id="d3ce5-113">String</span><span class="sxs-lookup"><span data-stu-id="d3ce5-113">String</span></span>| <span data-ttu-id="d3ce5-p101">Тип свойства, определенного в качестве части расширения схемы.  Разрешенные значения: *Binary, Boolean, DateTime, Integer* или *String*.  Дополнительные сведения см. в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="d3ce5-p101">The type of the property that is defined as part of a schema extension.  Allowed values are *Binary, Boolean, DateTime, Integer* or *String*.  See the table below for more details.</span></span>|

#### <a name="supported-property-data-types"></a><span data-ttu-id="d3ce5-117">Поддерживаемые типы данных свойств</span><span class="sxs-lookup"><span data-stu-id="d3ce5-117">Supported property data types</span></span> 
<span data-ttu-id="d3ce5-118">При определении свойства в расширении схемы поддерживаются следующие типы данных:</span><span class="sxs-lookup"><span data-stu-id="d3ce5-118">The following data types are supported when defining a property in a schema extension:</span></span>

| <span data-ttu-id="d3ce5-119">Тип свойства</span><span class="sxs-lookup"><span data-stu-id="d3ce5-119">Property Type</span></span> | <span data-ttu-id="d3ce5-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="d3ce5-120">Remarks</span></span> |
|-------------|------------|
| <span data-ttu-id="d3ce5-121">Binary</span><span class="sxs-lookup"><span data-stu-id="d3ce5-121">Binary</span></span> | <span data-ttu-id="d3ce5-122">Не более 256 байт.</span><span class="sxs-lookup"><span data-stu-id="d3ce5-122">256 bytes maximum.</span></span> |
| <span data-ttu-id="d3ce5-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="d3ce5-123">Boolean</span></span> | <span data-ttu-id="d3ce5-124">Не поддерживается для ресурсов contact, message, event и post.</span><span class="sxs-lookup"><span data-stu-id="d3ce5-124">Not supported for contacts, messages, events and posts.</span></span> |
| <span data-ttu-id="d3ce5-125">DateTime</span><span class="sxs-lookup"><span data-stu-id="d3ce5-125">DateTime</span></span> | <span data-ttu-id="d3ce5-p102">Должен быть указан в формате ISO 8601. Данные времени будут храниться в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="d3ce5-p102">Must be specified in ISO 8601 format. Will be stored in UTC.</span></span> |
| <span data-ttu-id="d3ce5-128">Целое число</span><span class="sxs-lookup"><span data-stu-id="d3ce5-128">Integer</span></span> | <span data-ttu-id="d3ce5-129">32-разрядное значение.</span><span class="sxs-lookup"><span data-stu-id="d3ce5-129">32-bit value.</span></span> <span data-ttu-id="d3ce5-130">Не поддерживается для ресурсов contact, message, event и post.</span><span class="sxs-lookup"><span data-stu-id="d3ce5-130">Not supported for contacts, messages, events and posts.</span></span> |
| <span data-ttu-id="d3ce5-131">String</span><span class="sxs-lookup"><span data-stu-id="d3ce5-131">String</span></span> | <span data-ttu-id="d3ce5-132">Не более 256 символов</span><span class="sxs-lookup"><span data-stu-id="d3ce5-132">256 characters maximum.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d3ce5-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d3ce5-133">JSON representation</span></span>
<span data-ttu-id="d3ce5-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d3ce5-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.extensionSchemaProperty"
}-->

```json
{
  "name": "String",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "extensionSchemaProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
