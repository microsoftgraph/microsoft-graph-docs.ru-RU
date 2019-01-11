---
title: Тип ресурса educationExcelResource
description: 'Подкласс educationResource. Этот тип ресурсов представляет документа в формате Excel.  '
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 7f772f7911667c76e64c31a856f3a9f8b6f3e6ff
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858102"
---
# <a name="educationexcelresource-resource-type"></a><span data-ttu-id="06019-104">Тип ресурса educationExcelResource</span><span class="sxs-lookup"><span data-stu-id="06019-104">educationExcelResource resource type</span></span>

> <span data-ttu-id="06019-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="06019-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="06019-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06019-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="06019-107">Подкласс [educationResource](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="06019-107">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="06019-108">Этот тип ресурсов представляет документа в формате Excel.</span><span class="sxs-lookup"><span data-stu-id="06019-108">This resource type represents an Excel document.</span></span>  
 
><span data-ttu-id="06019-109">**Примечание:** Файл Excel должен находиться в папку ресурсов, связанного с объектом назначения или отправки, к которой принадлежит ресурс.</span><span class="sxs-lookup"><span data-stu-id="06019-109">**Note:** The Excel file must be in the resource folder associated with the assignment or submission object to which this resource belongs.</span></span>


## <a name="properties"></a><span data-ttu-id="06019-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="06019-110">Properties</span></span>
| <span data-ttu-id="06019-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="06019-111">Property</span></span>     | <span data-ttu-id="06019-112">Тип</span><span class="sxs-lookup"><span data-stu-id="06019-112">Type</span></span>   |<span data-ttu-id="06019-113">Описание</span><span class="sxs-lookup"><span data-stu-id="06019-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="06019-114">fileUrl</span><span class="sxs-lookup"><span data-stu-id="06019-114">fileUrl</span></span>|<span data-ttu-id="06019-115">Строка</span><span class="sxs-lookup"><span data-stu-id="06019-115">String</span></span>|<span data-ttu-id="06019-116">Указатель на объект файла Excel.</span><span class="sxs-lookup"><span data-stu-id="06019-116">Pointer to the Excel file object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="06019-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="06019-117">JSON representation</span></span>

<span data-ttu-id="06019-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="06019-118">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationExcelResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
