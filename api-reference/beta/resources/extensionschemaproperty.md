---
title: Тип ресурса extensionSchemaProperty
description: Ресурс **extensionSchemaProperty** используется для задания имени и типа свойства в качестве части определения schemaExtension.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: keylimesoda
ms.openlocfilehash: 7f938f98c7f6060c41f7a162501ca42a553cace3
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761397"
---
# <a name="extensionschemaproperty-resource-type"></a><span data-ttu-id="f99e0-103">Тип ресурса extensionSchemaProperty</span><span class="sxs-lookup"><span data-stu-id="f99e0-103">extensionSchemaProperty resource type</span></span>

<span data-ttu-id="f99e0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f99e0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f99e0-105">Ресурс **extensionSchemaProperty** используется для задания имени и типа свойства в качестве части определения [schemaExtension](schemaextension.md).</span><span class="sxs-lookup"><span data-stu-id="f99e0-105">Use the **extensionSchemaProperty** resource to define a property's name and its type, as part of a [schemaExtension](schemaextension.md) definition.</span></span>


## <a name="properties"></a><span data-ttu-id="f99e0-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="f99e0-106">Properties</span></span>
| <span data-ttu-id="f99e0-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="f99e0-107">Property</span></span>     | <span data-ttu-id="f99e0-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f99e0-108">Type</span></span>   |<span data-ttu-id="f99e0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f99e0-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f99e0-110">name</span><span class="sxs-lookup"><span data-stu-id="f99e0-110">name</span></span>|<span data-ttu-id="f99e0-111">String</span><span class="sxs-lookup"><span data-stu-id="f99e0-111">String</span></span>| <span data-ttu-id="f99e0-112">Имя строго впечатаемого свойства, определяемого как часть расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="f99e0-112">The name of the strongly typed property defined as part of a schema extension.</span></span>|
|<span data-ttu-id="f99e0-113">type</span><span class="sxs-lookup"><span data-stu-id="f99e0-113">type</span></span>|<span data-ttu-id="f99e0-114">String</span><span class="sxs-lookup"><span data-stu-id="f99e0-114">String</span></span>| <span data-ttu-id="f99e0-p101">Тип свойства, определенного в качестве части расширения схемы.  Разрешенные значения: *Binary, Boolean, DateTime, Integer* или *String*.  Дополнительные сведения см. в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="f99e0-p101">The type of the property that is defined as part of a schema extension.  Allowed values are *Binary, Boolean, DateTime, Integer* or *String*.  See the table below for more details.</span></span>|

#### <a name="supported-property-data-types"></a><span data-ttu-id="f99e0-118">Поддерживаемые типы данных свойств</span><span class="sxs-lookup"><span data-stu-id="f99e0-118">Supported property data types</span></span> 
<span data-ttu-id="f99e0-119">При определении свойства в расширении схемы поддерживаются следующие типы данных:</span><span class="sxs-lookup"><span data-stu-id="f99e0-119">The following data types are supported when defining a property in a schema extension:</span></span>

| <span data-ttu-id="f99e0-120">Тип свойства</span><span class="sxs-lookup"><span data-stu-id="f99e0-120">Property Type</span></span> | <span data-ttu-id="f99e0-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="f99e0-121">Remarks</span></span> |
|-------------|------------|
| <span data-ttu-id="f99e0-122">Binary</span><span class="sxs-lookup"><span data-stu-id="f99e0-122">Binary</span></span> | <span data-ttu-id="f99e0-123">Не более 256 байт.</span><span class="sxs-lookup"><span data-stu-id="f99e0-123">256 bytes maximum.</span></span> |
| <span data-ttu-id="f99e0-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="f99e0-124">Boolean</span></span> | <span data-ttu-id="f99e0-125">Не поддерживается для ресурсов message, event и post.</span><span class="sxs-lookup"><span data-stu-id="f99e0-125">Not supported for messages, events and posts.</span></span> |
| <span data-ttu-id="f99e0-126">DateTime</span><span class="sxs-lookup"><span data-stu-id="f99e0-126">DateTime</span></span> | <span data-ttu-id="f99e0-p102">Должен быть указан в формате ISO 8601. Данные времени будут храниться в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="f99e0-p102">Must be specified in ISO 8601 format. Will be stored in UTC.</span></span> |
| <span data-ttu-id="f99e0-129">Целое число</span><span class="sxs-lookup"><span data-stu-id="f99e0-129">Integer</span></span> | <span data-ttu-id="f99e0-p103">32-разрядное значение. Не поддерживается для ресурсов message, event и post.</span><span class="sxs-lookup"><span data-stu-id="f99e0-p103">32-bit value. Not supported for messages, events and posts.</span></span> |
| <span data-ttu-id="f99e0-132">String</span><span class="sxs-lookup"><span data-stu-id="f99e0-132">String</span></span> | <span data-ttu-id="f99e0-133">Не более 256 символов</span><span class="sxs-lookup"><span data-stu-id="f99e0-133">256 characters maximum.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f99e0-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f99e0-134">JSON representation</span></span>
<span data-ttu-id="f99e0-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f99e0-135">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "extensionSchemaProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


