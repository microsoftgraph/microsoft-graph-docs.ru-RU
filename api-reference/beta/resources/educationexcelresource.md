---
title: Тип ресурса Едукатионексцелресаурце
description: 'Подкласс объекта Едукатионресаурце. Этот тип ресурса представляет документ Excel.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ef85a92b2629e8a652ce59210018725d6afecb9a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972749"
---
# <a name="educationexcelresource-resource-type"></a><span data-ttu-id="78d20-104">Тип ресурса Едукатионексцелресаурце</span><span class="sxs-lookup"><span data-stu-id="78d20-104">educationExcelResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78d20-105">Подкласс объекта [едукатионресаурце](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="78d20-105">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="78d20-106">Этот тип ресурса представляет документ Excel.</span><span class="sxs-lookup"><span data-stu-id="78d20-106">This resource type represents an Excel document.</span></span>  
 
><span data-ttu-id="78d20-107">**Примечание:** Файл Excel должен находиться в папке ресурсов, связанной с назначением или объектом отправки, к которому принадлежит ресурс.</span><span class="sxs-lookup"><span data-stu-id="78d20-107">**Note:** The Excel file must be in the resource folder associated with the assignment or submission object to which this resource belongs.</span></span>


## <a name="properties"></a><span data-ttu-id="78d20-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="78d20-108">Properties</span></span>
| <span data-ttu-id="78d20-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="78d20-109">Property</span></span>     | <span data-ttu-id="78d20-110">Тип</span><span class="sxs-lookup"><span data-stu-id="78d20-110">Type</span></span>   |<span data-ttu-id="78d20-111">Описание</span><span class="sxs-lookup"><span data-stu-id="78d20-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="78d20-112">fileUrl</span><span class="sxs-lookup"><span data-stu-id="78d20-112">fileUrl</span></span>|<span data-ttu-id="78d20-113">String</span><span class="sxs-lookup"><span data-stu-id="78d20-113">String</span></span>|<span data-ttu-id="78d20-114">Указатель на объект файла Excel.</span><span class="sxs-lookup"><span data-stu-id="78d20-114">Pointer to the Excel file object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="78d20-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="78d20-115">JSON representation</span></span>

<span data-ttu-id="78d20-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="78d20-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationExcelResource"
}-->

```json
{
  "fileUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationExcelResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
