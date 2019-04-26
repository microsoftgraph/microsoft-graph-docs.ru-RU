---
title: Тип ресурса Едукатионексцелресаурце
description: 'Подкласс объекта Едукатионресаурце. Этот тип ресурса представляет документ Excel.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: be9ea1d08575ad9dc07ac9fe538a597da8db2803
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334429"
---
# <a name="educationexcelresource-resource-type"></a><span data-ttu-id="cff5f-104">Тип ресурса Едукатионексцелресаурце</span><span class="sxs-lookup"><span data-stu-id="cff5f-104">educationExcelResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cff5f-105">Подкласс объекта [едукатионресаурце](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="cff5f-105">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="cff5f-106">Этот тип ресурса представляет документ Excel.</span><span class="sxs-lookup"><span data-stu-id="cff5f-106">This resource type represents an Excel document.</span></span>  
 
><span data-ttu-id="cff5f-107">**Примечание:** Файл Excel должен находиться в папке ресурсов, связанной с назначением или объектом отправки, к которому принадлежит ресурс.</span><span class="sxs-lookup"><span data-stu-id="cff5f-107">**Note:** The Excel file must be in the resource folder associated with the assignment or submission object to which this resource belongs.</span></span>


## <a name="properties"></a><span data-ttu-id="cff5f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="cff5f-108">Properties</span></span>
| <span data-ttu-id="cff5f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="cff5f-109">Property</span></span>     | <span data-ttu-id="cff5f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="cff5f-110">Type</span></span>   |<span data-ttu-id="cff5f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="cff5f-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cff5f-112">fileUrl</span><span class="sxs-lookup"><span data-stu-id="cff5f-112">fileUrl</span></span>|<span data-ttu-id="cff5f-113">String</span><span class="sxs-lookup"><span data-stu-id="cff5f-113">String</span></span>|<span data-ttu-id="cff5f-114">Указатель на объект файла Excel.</span><span class="sxs-lookup"><span data-stu-id="cff5f-114">Pointer to the Excel file object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cff5f-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cff5f-115">JSON representation</span></span>

<span data-ttu-id="cff5f-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cff5f-116">The following is a JSON representation of the resource.</span></span>

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
