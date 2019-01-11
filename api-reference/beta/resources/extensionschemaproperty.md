---
title: Тип ресурса extensionSchemaProperty
description: Ресурс **extensionSchemaProperty** используется для задания имени и типа свойства в качестве части определения schemaExtension.
localization_priority: Normal
ms.openlocfilehash: 44769bab4a4f4b40a80d896bed2311554ea5e8ad
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889861"
---
# <a name="extensionschemaproperty-resource-type"></a><span data-ttu-id="767dd-103">Тип ресурса extensionSchemaProperty</span><span class="sxs-lookup"><span data-stu-id="767dd-103">extensionSchemaProperty resource type</span></span>

> <span data-ttu-id="767dd-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="767dd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="767dd-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="767dd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="767dd-106">Ресурс **extensionSchemaProperty** используется для задания имени и типа свойства в качестве части определения [schemaExtension](schemaextension.md).</span><span class="sxs-lookup"><span data-stu-id="767dd-106">Use the **extensionSchemaProperty** resource to define a property's name and its type, as part of a [schemaExtension](schemaextension.md) definition.</span></span>


## <a name="properties"></a><span data-ttu-id="767dd-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="767dd-107">Properties</span></span>
| <span data-ttu-id="767dd-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="767dd-108">Property</span></span>     | <span data-ttu-id="767dd-109">Тип</span><span class="sxs-lookup"><span data-stu-id="767dd-109">Type</span></span>   |<span data-ttu-id="767dd-110">Описание</span><span class="sxs-lookup"><span data-stu-id="767dd-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="767dd-111">name</span><span class="sxs-lookup"><span data-stu-id="767dd-111">name</span></span>|<span data-ttu-id="767dd-112">Строка</span><span class="sxs-lookup"><span data-stu-id="767dd-112">String</span></span>| <span data-ttu-id="767dd-113">Имя строго типизированные свойства, определенные как часть расширение схемы.</span><span class="sxs-lookup"><span data-stu-id="767dd-113">The name of the strongly typed property defined as part of a schema extension.</span></span>|
|<span data-ttu-id="767dd-114">type</span><span class="sxs-lookup"><span data-stu-id="767dd-114">type</span></span>|<span data-ttu-id="767dd-115">Строка</span><span class="sxs-lookup"><span data-stu-id="767dd-115">String</span></span>| <span data-ttu-id="767dd-p102">Тип свойства, определенного в качестве части расширения схемы.  Разрешенные значения: *Binary, Boolean, DateTime, Integer* или *String*.  Дополнительные сведения см. в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="767dd-p102">The type of the property that is defined as part of a schema extension.  Allowed values are *Binary, Boolean, DateTime, Integer* or *String*.  See the table below for more details.</span></span>|

#### <a name="supported-property-data-types"></a><span data-ttu-id="767dd-119">Поддерживаемые типы данных свойств</span><span class="sxs-lookup"><span data-stu-id="767dd-119">Supported property data types</span></span> 
<span data-ttu-id="767dd-120">При определении свойства в расширении схемы поддерживаются следующие типы данных:</span><span class="sxs-lookup"><span data-stu-id="767dd-120">The following data types are supported when defining a property in a schema extension:</span></span>

| <span data-ttu-id="767dd-121">Тип свойства</span><span class="sxs-lookup"><span data-stu-id="767dd-121">Property Type</span></span> | <span data-ttu-id="767dd-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="767dd-122">Remarks</span></span> |
|-------------|------------|
| <span data-ttu-id="767dd-123">Binary</span><span class="sxs-lookup"><span data-stu-id="767dd-123">Binary</span></span> | <span data-ttu-id="767dd-124">Не более 256 байт.</span><span class="sxs-lookup"><span data-stu-id="767dd-124">256 bytes maximum.</span></span> |
| <span data-ttu-id="767dd-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="767dd-125">Boolean</span></span> | <span data-ttu-id="767dd-126">Не поддерживается для ресурсов message, event и post.</span><span class="sxs-lookup"><span data-stu-id="767dd-126">Not supported for messages, events and posts.</span></span> |
| <span data-ttu-id="767dd-127">DateTime</span><span class="sxs-lookup"><span data-stu-id="767dd-127">DateTime</span></span> | <span data-ttu-id="767dd-p103">Должен быть указан в формате ISO 8601. Данные времени будут храниться в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="767dd-p103">Must be specified in ISO 8601 format. Will be stored in UTC.</span></span> |
| <span data-ttu-id="767dd-130">Целое число</span><span class="sxs-lookup"><span data-stu-id="767dd-130">Integer</span></span> | <span data-ttu-id="767dd-p104">32-разрядное значение. Не поддерживается для ресурсов message, event и post.</span><span class="sxs-lookup"><span data-stu-id="767dd-p104">32-bit value. Not supported for messages, events and posts.</span></span> |
| <span data-ttu-id="767dd-133">String</span><span class="sxs-lookup"><span data-stu-id="767dd-133">String</span></span> | <span data-ttu-id="767dd-134">Не более 256 символов.</span><span class="sxs-lookup"><span data-stu-id="767dd-134">256 characters maximum.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="767dd-135">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="767dd-135">JSON representation</span></span>
<span data-ttu-id="767dd-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="767dd-136">Here is a JSON representation of the resource.</span></span>

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
