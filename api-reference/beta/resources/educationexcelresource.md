---
title: Тип ресурса Едукатионексцелресаурце
description: 'Подкласс объекта Едукатионресаурце. Этот тип ресурса представляет документ Excel.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 96fc84227bc7c8e5140ef06ce62ea2d485badab7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095529"
---
# <a name="educationexcelresource-resource-type"></a><span data-ttu-id="377e9-104">Тип ресурса Едукатионексцелресаурце</span><span class="sxs-lookup"><span data-stu-id="377e9-104">educationExcelResource resource type</span></span>

<span data-ttu-id="377e9-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="377e9-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="377e9-106">Подкласс объекта [едукатионресаурце](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="377e9-106">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="377e9-107">Этот тип ресурса представляет документ Excel.</span><span class="sxs-lookup"><span data-stu-id="377e9-107">This resource type represents an Excel document.</span></span>  
 
><span data-ttu-id="377e9-108">**Примечание:** Файл Excel должен находиться в папке ресурсов, связанной с назначением или объектом отправки, к которому принадлежит ресурс.</span><span class="sxs-lookup"><span data-stu-id="377e9-108">**Note:** The Excel file must be in the resource folder associated with the assignment or submission object to which this resource belongs.</span></span>


## <a name="properties"></a><span data-ttu-id="377e9-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="377e9-109">Properties</span></span>
| <span data-ttu-id="377e9-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="377e9-110">Property</span></span>     | <span data-ttu-id="377e9-111">Тип</span><span class="sxs-lookup"><span data-stu-id="377e9-111">Type</span></span>   |<span data-ttu-id="377e9-112">Описание</span><span class="sxs-lookup"><span data-stu-id="377e9-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="377e9-113">fileUrl</span><span class="sxs-lookup"><span data-stu-id="377e9-113">fileUrl</span></span>|<span data-ttu-id="377e9-114">Строка</span><span class="sxs-lookup"><span data-stu-id="377e9-114">String</span></span>|<span data-ttu-id="377e9-115">Указатель на объект файла Excel.</span><span class="sxs-lookup"><span data-stu-id="377e9-115">Pointer to the Excel file object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="377e9-116">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="377e9-116">JSON representation</span></span>

<span data-ttu-id="377e9-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="377e9-117">The following is a JSON representation of the resource.</span></span>

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


