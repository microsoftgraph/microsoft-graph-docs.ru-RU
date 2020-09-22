---
title: Тип ресурса extensionSchemaProperty
description: Ресурс **extensionSchemaProperty** используется для задания имени и типа свойства в качестве части определения schemaExtension.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: keylimesoda
ms.openlocfilehash: c0bb3a423983b70066e2451a5029f4eaf2acaebd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026945"
---
# <a name="extensionschemaproperty-resource-type"></a><span data-ttu-id="24642-103">Тип ресурса extensionSchemaProperty</span><span class="sxs-lookup"><span data-stu-id="24642-103">extensionSchemaProperty resource type</span></span>

<span data-ttu-id="24642-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24642-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24642-105">Ресурс **extensionSchemaProperty** используется для задания имени и типа свойства в качестве части определения [schemaExtension](schemaextension.md).</span><span class="sxs-lookup"><span data-stu-id="24642-105">Use the **extensionSchemaProperty** resource to define a property's name and its type, as part of a [schemaExtension](schemaextension.md) definition.</span></span>


## <a name="properties"></a><span data-ttu-id="24642-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="24642-106">Properties</span></span>
| <span data-ttu-id="24642-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="24642-107">Property</span></span>     | <span data-ttu-id="24642-108">Тип</span><span class="sxs-lookup"><span data-stu-id="24642-108">Type</span></span>   |<span data-ttu-id="24642-109">Описание</span><span class="sxs-lookup"><span data-stu-id="24642-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="24642-110">name</span><span class="sxs-lookup"><span data-stu-id="24642-110">name</span></span>|<span data-ttu-id="24642-111">String</span><span class="sxs-lookup"><span data-stu-id="24642-111">String</span></span>| <span data-ttu-id="24642-112">Имя строго типизированного свойства, определенного как часть расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="24642-112">The name of the strongly typed property defined as part of a schema extension.</span></span>|
|<span data-ttu-id="24642-113">type</span><span class="sxs-lookup"><span data-stu-id="24642-113">type</span></span>|<span data-ttu-id="24642-114">String</span><span class="sxs-lookup"><span data-stu-id="24642-114">String</span></span>| <span data-ttu-id="24642-p101">Тип свойства, определенного в качестве части расширения схемы.  Разрешенные значения: *Binary, Boolean, DateTime, Integer* или *String*.  Дополнительные сведения см. в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="24642-p101">The type of the property that is defined as part of a schema extension.  Allowed values are *Binary, Boolean, DateTime, Integer* or *String*.  See the table below for more details.</span></span>|

#### <a name="supported-property-data-types"></a><span data-ttu-id="24642-118">Поддерживаемые типы данных свойств</span><span class="sxs-lookup"><span data-stu-id="24642-118">Supported property data types</span></span> 
<span data-ttu-id="24642-119">При определении свойства в расширении схемы поддерживаются следующие типы данных:</span><span class="sxs-lookup"><span data-stu-id="24642-119">The following data types are supported when defining a property in a schema extension:</span></span>

| <span data-ttu-id="24642-120">Тип свойства</span><span class="sxs-lookup"><span data-stu-id="24642-120">Property Type</span></span> | <span data-ttu-id="24642-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="24642-121">Remarks</span></span> |
|-------------|------------|
| <span data-ttu-id="24642-122">Binary</span><span class="sxs-lookup"><span data-stu-id="24642-122">Binary</span></span> | <span data-ttu-id="24642-123">Не более 256 байт.</span><span class="sxs-lookup"><span data-stu-id="24642-123">256 bytes maximum.</span></span> |
| <span data-ttu-id="24642-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="24642-124">Boolean</span></span> | <span data-ttu-id="24642-125">Не поддерживается для ресурсов message, event и post.</span><span class="sxs-lookup"><span data-stu-id="24642-125">Not supported for messages, events and posts.</span></span> |
| <span data-ttu-id="24642-126">DateTime</span><span class="sxs-lookup"><span data-stu-id="24642-126">DateTime</span></span> | <span data-ttu-id="24642-p102">Должен быть указан в формате ISO 8601. Данные времени будут храниться в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="24642-p102">Must be specified in ISO 8601 format. Will be stored in UTC.</span></span> |
| <span data-ttu-id="24642-129">Целое число</span><span class="sxs-lookup"><span data-stu-id="24642-129">Integer</span></span> | <span data-ttu-id="24642-p103">32-разрядное значение. Не поддерживается для ресурсов message, event и post.</span><span class="sxs-lookup"><span data-stu-id="24642-p103">32-bit value. Not supported for messages, events and posts.</span></span> |
| <span data-ttu-id="24642-132">String</span><span class="sxs-lookup"><span data-stu-id="24642-132">String</span></span> | <span data-ttu-id="24642-133">Не более 256 символов</span><span class="sxs-lookup"><span data-stu-id="24642-133">256 characters maximum.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="24642-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="24642-134">JSON representation</span></span>
<span data-ttu-id="24642-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="24642-135">Here is a JSON representation of the resource.</span></span>

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


