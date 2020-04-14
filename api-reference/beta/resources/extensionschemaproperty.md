---
title: Тип ресурса extensionSchemaProperty
description: Ресурс **extensionSchemaProperty** используется для задания имени и типа свойства в качестве части определения schemaExtension.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: keylimesoda
ms.openlocfilehash: e28642e12e7c9bb52b16c21e775e91562de1ebdb
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43423680"
---
# <a name="extensionschemaproperty-resource-type"></a><span data-ttu-id="fd6a6-103">Тип ресурса extensionSchemaProperty</span><span class="sxs-lookup"><span data-stu-id="fd6a6-103">extensionSchemaProperty resource type</span></span>

<span data-ttu-id="fd6a6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd6a6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd6a6-105">Ресурс **extensionSchemaProperty** используется для задания имени и типа свойства в качестве части определения [schemaExtension](schemaextension.md).</span><span class="sxs-lookup"><span data-stu-id="fd6a6-105">Use the **extensionSchemaProperty** resource to define a property's name and its type, as part of a [schemaExtension](schemaextension.md) definition.</span></span>


## <a name="properties"></a><span data-ttu-id="fd6a6-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="fd6a6-106">Properties</span></span>
| <span data-ttu-id="fd6a6-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="fd6a6-107">Property</span></span>     | <span data-ttu-id="fd6a6-108">Тип</span><span class="sxs-lookup"><span data-stu-id="fd6a6-108">Type</span></span>   |<span data-ttu-id="fd6a6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="fd6a6-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fd6a6-110">name</span><span class="sxs-lookup"><span data-stu-id="fd6a6-110">name</span></span>|<span data-ttu-id="fd6a6-111">Строка</span><span class="sxs-lookup"><span data-stu-id="fd6a6-111">String</span></span>| <span data-ttu-id="fd6a6-112">Имя строго типизированного свойства, определенного как часть расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="fd6a6-112">The name of the strongly typed property defined as part of a schema extension.</span></span>|
|<span data-ttu-id="fd6a6-113">type</span><span class="sxs-lookup"><span data-stu-id="fd6a6-113">type</span></span>|<span data-ttu-id="fd6a6-114">String</span><span class="sxs-lookup"><span data-stu-id="fd6a6-114">String</span></span>| <span data-ttu-id="fd6a6-p101">Тип свойства, определенного в качестве части расширения схемы.  Разрешенные значения: *Binary, Boolean, DateTime, Integer* или *String*.  Дополнительные сведения см. в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="fd6a6-p101">The type of the property that is defined as part of a schema extension.  Allowed values are *Binary, Boolean, DateTime, Integer* or *String*.  See the table below for more details.</span></span>|

#### <a name="supported-property-data-types"></a><span data-ttu-id="fd6a6-118">Поддерживаемые типы данных свойств</span><span class="sxs-lookup"><span data-stu-id="fd6a6-118">Supported property data types</span></span> 
<span data-ttu-id="fd6a6-119">При определении свойства в расширении схемы поддерживаются следующие типы данных:</span><span class="sxs-lookup"><span data-stu-id="fd6a6-119">The following data types are supported when defining a property in a schema extension:</span></span>

| <span data-ttu-id="fd6a6-120">Тип свойства</span><span class="sxs-lookup"><span data-stu-id="fd6a6-120">Property Type</span></span> | <span data-ttu-id="fd6a6-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="fd6a6-121">Remarks</span></span> |
|-------------|------------|
| <span data-ttu-id="fd6a6-122">Binary</span><span class="sxs-lookup"><span data-stu-id="fd6a6-122">Binary</span></span> | <span data-ttu-id="fd6a6-123">Не более 256 байт.</span><span class="sxs-lookup"><span data-stu-id="fd6a6-123">256 bytes maximum.</span></span> |
| <span data-ttu-id="fd6a6-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="fd6a6-124">Boolean</span></span> | <span data-ttu-id="fd6a6-125">Не поддерживается для ресурсов message, event и post.</span><span class="sxs-lookup"><span data-stu-id="fd6a6-125">Not supported for messages, events and posts.</span></span> |
| <span data-ttu-id="fd6a6-126">DateTime</span><span class="sxs-lookup"><span data-stu-id="fd6a6-126">DateTime</span></span> | <span data-ttu-id="fd6a6-p102">Должен быть указан в формате ISO 8601. Данные времени будут храниться в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="fd6a6-p102">Must be specified in ISO 8601 format. Will be stored in UTC.</span></span> |
| <span data-ttu-id="fd6a6-129">Целое число</span><span class="sxs-lookup"><span data-stu-id="fd6a6-129">Integer</span></span> | <span data-ttu-id="fd6a6-p103">32-разрядное значение. Не поддерживается для ресурсов message, event и post.</span><span class="sxs-lookup"><span data-stu-id="fd6a6-p103">32-bit value. Not supported for messages, events and posts.</span></span> |
| <span data-ttu-id="fd6a6-132">String</span><span class="sxs-lookup"><span data-stu-id="fd6a6-132">String</span></span> | <span data-ttu-id="fd6a6-133">Не более 256 символов</span><span class="sxs-lookup"><span data-stu-id="fd6a6-133">256 characters maximum.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fd6a6-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fd6a6-134">JSON representation</span></span>
<span data-ttu-id="fd6a6-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fd6a6-135">Here is a JSON representation of the resource.</span></span>

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
