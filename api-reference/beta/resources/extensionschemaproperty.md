---
title: Тип ресурса extensionSchemaProperty
description: Ресурс **extensionSchemaProperty** используется для задания имени и типа свойства в качестве части определения schemaExtension.
localization_priority: Normal
ms.openlocfilehash: bb044aa2f85ea5accdba4ed43a1a5b1c856a209d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542652"
---
# <a name="extensionschemaproperty-resource-type"></a><span data-ttu-id="9ce6c-103">Тип ресурса extensionSchemaProperty</span><span class="sxs-lookup"><span data-stu-id="9ce6c-103">extensionSchemaProperty resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ce6c-104">Ресурс **extensionSchemaProperty** используется для задания имени и типа свойства в качестве части определения [schemaExtension](schemaextension.md).</span><span class="sxs-lookup"><span data-stu-id="9ce6c-104">Use the **extensionSchemaProperty** resource to define a property's name and its type, as part of a [schemaExtension](schemaextension.md) definition.</span></span>


## <a name="properties"></a><span data-ttu-id="9ce6c-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="9ce6c-105">Properties</span></span>
| <span data-ttu-id="9ce6c-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="9ce6c-106">Property</span></span>     | <span data-ttu-id="9ce6c-107">Тип</span><span class="sxs-lookup"><span data-stu-id="9ce6c-107">Type</span></span>   |<span data-ttu-id="9ce6c-108">Описание</span><span class="sxs-lookup"><span data-stu-id="9ce6c-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9ce6c-109">name</span><span class="sxs-lookup"><span data-stu-id="9ce6c-109">name</span></span>|<span data-ttu-id="9ce6c-110">String</span><span class="sxs-lookup"><span data-stu-id="9ce6c-110">String</span></span>| <span data-ttu-id="9ce6c-111">Имя строго типизированного свойства, определенного как часть расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="9ce6c-111">The name of the strongly typed property defined as part of a schema extension.</span></span>|
|<span data-ttu-id="9ce6c-112">type</span><span class="sxs-lookup"><span data-stu-id="9ce6c-112">type</span></span>|<span data-ttu-id="9ce6c-113">Строка</span><span class="sxs-lookup"><span data-stu-id="9ce6c-113">String</span></span>| <span data-ttu-id="9ce6c-p101">Тип свойства, определенного в качестве части расширения схемы.  Разрешенные значения: *Binary, Boolean, DateTime, Integer* или *String*.  Дополнительные сведения см. в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="9ce6c-p101">The type of the property that is defined as part of a schema extension.  Allowed values are *Binary, Boolean, DateTime, Integer* or *String*.  See the table below for more details.</span></span>|

#### <a name="supported-property-data-types"></a><span data-ttu-id="9ce6c-117">Поддерживаемые типы данных свойств</span><span class="sxs-lookup"><span data-stu-id="9ce6c-117">Supported property data types</span></span> 
<span data-ttu-id="9ce6c-118">При определении свойства в расширении схемы поддерживаются следующие типы данных:</span><span class="sxs-lookup"><span data-stu-id="9ce6c-118">The following data types are supported when defining a property in a schema extension:</span></span>

| <span data-ttu-id="9ce6c-119">Тип свойства</span><span class="sxs-lookup"><span data-stu-id="9ce6c-119">Property Type</span></span> | <span data-ttu-id="9ce6c-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="9ce6c-120">Remarks</span></span> |
|-------------|------------|
| <span data-ttu-id="9ce6c-121">Binary</span><span class="sxs-lookup"><span data-stu-id="9ce6c-121">Binary</span></span> | <span data-ttu-id="9ce6c-122">Не более 256 байт.</span><span class="sxs-lookup"><span data-stu-id="9ce6c-122">256 bytes maximum.</span></span> |
| <span data-ttu-id="9ce6c-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ce6c-123">Boolean</span></span> | <span data-ttu-id="9ce6c-124">Не поддерживается для ресурсов message, event и post.</span><span class="sxs-lookup"><span data-stu-id="9ce6c-124">Not supported for messages, events and posts.</span></span> |
| <span data-ttu-id="9ce6c-125">DateTime</span><span class="sxs-lookup"><span data-stu-id="9ce6c-125">DateTime</span></span> | <span data-ttu-id="9ce6c-p102">Должен быть указан в формате ISO 8601. Данные времени будут храниться в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="9ce6c-p102">Must be specified in ISO 8601 format. Will be stored in UTC.</span></span> |
| <span data-ttu-id="9ce6c-128">Целое число</span><span class="sxs-lookup"><span data-stu-id="9ce6c-128">Integer</span></span> | <span data-ttu-id="9ce6c-p103">32-разрядное значение. Не поддерживается для ресурсов message, event и post.</span><span class="sxs-lookup"><span data-stu-id="9ce6c-p103">32-bit value. Not supported for messages, events and posts.</span></span> |
| <span data-ttu-id="9ce6c-131">String</span><span class="sxs-lookup"><span data-stu-id="9ce6c-131">String</span></span> | <span data-ttu-id="9ce6c-132">Не более 256 символов.</span><span class="sxs-lookup"><span data-stu-id="9ce6c-132">256 characters maximum.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9ce6c-133">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="9ce6c-133">JSON representation</span></span>
<span data-ttu-id="9ce6c-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9ce6c-134">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/extensionschemaproperty.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
