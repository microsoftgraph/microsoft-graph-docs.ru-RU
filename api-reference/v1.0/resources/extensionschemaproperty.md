---
title: Тип ресурса extensionSchemaProperty
description: Ресурс **extensionSchemaProperty** используется для задания имени и типа свойства в качестве части определения schemaExtension.
localization_priority: Normal
author: keylimesoda
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 623dd4fa92036a3c542bebf791dc802ce0d53520
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812339"
---
# <a name="extensionschemaproperty-resource-type"></a><span data-ttu-id="6c9ed-103">Тип ресурса extensionSchemaProperty</span><span class="sxs-lookup"><span data-stu-id="6c9ed-103">extensionSchemaProperty resource type</span></span>

<span data-ttu-id="6c9ed-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c9ed-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6c9ed-105">Ресурс **extensionSchemaProperty** используется для задания имени и типа свойства в качестве части определения [schemaExtension](schemaextension.md).</span><span class="sxs-lookup"><span data-stu-id="6c9ed-105">Use the **extensionSchemaProperty** resource to define a property's name and its type, as part of a [schemaExtension](schemaextension.md) definition.</span></span>


## <a name="properties"></a><span data-ttu-id="6c9ed-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="6c9ed-106">Properties</span></span>
| <span data-ttu-id="6c9ed-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="6c9ed-107">Property</span></span>     | <span data-ttu-id="6c9ed-108">Тип</span><span class="sxs-lookup"><span data-stu-id="6c9ed-108">Type</span></span>   |<span data-ttu-id="6c9ed-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6c9ed-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6c9ed-110">name</span><span class="sxs-lookup"><span data-stu-id="6c9ed-110">name</span></span>|<span data-ttu-id="6c9ed-111">String</span><span class="sxs-lookup"><span data-stu-id="6c9ed-111">String</span></span>| <span data-ttu-id="6c9ed-112">Имя строго типизированного свойства, определенного в качестве части расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="6c9ed-112">The name of the strongly-typed property defined as part of a schema extension.</span></span>|
|<span data-ttu-id="6c9ed-113">type</span><span class="sxs-lookup"><span data-stu-id="6c9ed-113">type</span></span>|<span data-ttu-id="6c9ed-114">String</span><span class="sxs-lookup"><span data-stu-id="6c9ed-114">String</span></span>| <span data-ttu-id="6c9ed-p101">Тип свойства, определенного в качестве части расширения схемы.  Разрешенные значения: *Binary, Boolean, DateTime, Integer* или *String*.  Дополнительные сведения см. в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="6c9ed-p101">The type of the property that is defined as part of a schema extension.  Allowed values are *Binary, Boolean, DateTime, Integer* or *String*.  See the table below for more details.</span></span>|

#### <a name="supported-property-data-types"></a><span data-ttu-id="6c9ed-118">Поддерживаемые типы данных свойств</span><span class="sxs-lookup"><span data-stu-id="6c9ed-118">Supported property data types</span></span>
<span data-ttu-id="6c9ed-119">При определении свойства в расширении схемы поддерживаются следующие типы данных:</span><span class="sxs-lookup"><span data-stu-id="6c9ed-119">The following data types are supported when defining a property in a schema extension:</span></span>

| <span data-ttu-id="6c9ed-120">Тип свойства</span><span class="sxs-lookup"><span data-stu-id="6c9ed-120">Property Type</span></span> | <span data-ttu-id="6c9ed-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="6c9ed-121">Remarks</span></span> |
|-------------|------------|
| <span data-ttu-id="6c9ed-122">Binary</span><span class="sxs-lookup"><span data-stu-id="6c9ed-122">Binary</span></span> | <span data-ttu-id="6c9ed-123">Не более 256 байт.</span><span class="sxs-lookup"><span data-stu-id="6c9ed-123">256 bytes maximum.</span></span> |
| <span data-ttu-id="6c9ed-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c9ed-124">Boolean</span></span> | <span data-ttu-id="6c9ed-125">Не поддерживается для ресурсов contact, message, event и post.</span><span class="sxs-lookup"><span data-stu-id="6c9ed-125">Not supported for contacts, messages, events and posts.</span></span> |
| <span data-ttu-id="6c9ed-126">DateTime</span><span class="sxs-lookup"><span data-stu-id="6c9ed-126">DateTime</span></span> | <span data-ttu-id="6c9ed-p102">Должен быть указан в формате ISO 8601. Данные времени будут храниться в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="6c9ed-p102">Must be specified in ISO 8601 format. Will be stored in UTC.</span></span> |
| <span data-ttu-id="6c9ed-129">Целое число</span><span class="sxs-lookup"><span data-stu-id="6c9ed-129">Integer</span></span> | <span data-ttu-id="6c9ed-130">32-разрядное значение.</span><span class="sxs-lookup"><span data-stu-id="6c9ed-130">32-bit value.</span></span> <span data-ttu-id="6c9ed-131">Не поддерживается для ресурсов contact, message, event и post.</span><span class="sxs-lookup"><span data-stu-id="6c9ed-131">Not supported for contacts, messages, events and posts.</span></span> |
| <span data-ttu-id="6c9ed-132">String</span><span class="sxs-lookup"><span data-stu-id="6c9ed-132">String</span></span> | <span data-ttu-id="6c9ed-133">Не более 256 символов</span><span class="sxs-lookup"><span data-stu-id="6c9ed-133">256 characters maximum.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6c9ed-134">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="6c9ed-134">JSON representation</span></span>
<span data-ttu-id="6c9ed-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6c9ed-135">Here is a JSON representation of the resource.</span></span>

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
