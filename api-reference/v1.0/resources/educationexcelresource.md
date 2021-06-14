---
title: тип ресурсов educationExcelResource
description: Подкласс educationResource. Этот тип ресурса представляет собой Excel документа.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 9345bb39f16066b4c5eee688d781e99563147ef2
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912628"
---
# <a name="educationexcelresource-resource-type"></a><span data-ttu-id="da710-104">тип ресурсов educationExcelResource</span><span class="sxs-lookup"><span data-stu-id="da710-104">educationExcelResource resource type</span></span>

<span data-ttu-id="da710-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da710-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="da710-106">Подкласс [educationResource](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="da710-106">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="da710-107">Этот тип ресурса представляет собой Excel документа.</span><span class="sxs-lookup"><span data-stu-id="da710-107">This resource type represents an Excel document.</span></span>  
 
><span data-ttu-id="da710-108">**Примечание:** Файл Excel должен быть в папке ресурса, связанной с объектом назначения или отправки, к которому принадлежит этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="da710-108">**Note:** The Excel file must be in the resource folder associated with the assignment or submission object to which this resource belongs.</span></span>


## <a name="properties"></a><span data-ttu-id="da710-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="da710-109">Properties</span></span>
| <span data-ttu-id="da710-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="da710-110">Property</span></span>     | <span data-ttu-id="da710-111">Тип</span><span class="sxs-lookup"><span data-stu-id="da710-111">Type</span></span>   |<span data-ttu-id="da710-112">Описание</span><span class="sxs-lookup"><span data-stu-id="da710-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="da710-113">fileUrl</span><span class="sxs-lookup"><span data-stu-id="da710-113">fileUrl</span></span>|<span data-ttu-id="da710-114">String</span><span class="sxs-lookup"><span data-stu-id="da710-114">String</span></span>|<span data-ttu-id="da710-115">Указатель на объект Excel файла.</span><span class="sxs-lookup"><span data-stu-id="da710-115">Pointer to the Excel file object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="da710-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="da710-116">JSON representation</span></span>

<span data-ttu-id="da710-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="da710-117">The following is a JSON representation of the resource.</span></span>

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


