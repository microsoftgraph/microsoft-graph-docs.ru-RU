---
title: тип ресурса educationWordResource
description: Подкласс educationResource.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 1d28d37f34073488f7022d19ae227bb2af2fd306
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912799"
---
# <a name="educationwordresource-resource-type"></a><span data-ttu-id="4c748-103">тип ресурса educationWordResource</span><span class="sxs-lookup"><span data-stu-id="4c748-103">educationWordResource resource type</span></span>

<span data-ttu-id="4c748-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c748-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4c748-105">Подкласс [educationResource](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="4c748-105">A subclass of [educationResource](educationresource.md).</span></span> 

<span data-ttu-id="4c748-106">Это ресурс документа Word.</span><span class="sxs-lookup"><span data-stu-id="4c748-106">This is a Word document resource.</span></span> <span data-ttu-id="4c748-107">Файл Word должен быть загружен в **каталог fileResource,** связанный с назначением или отправкой.</span><span class="sxs-lookup"><span data-stu-id="4c748-107">The Word file must be uploaded in the **fileResource** directory associated with the assignment or submission.</span></span>


## <a name="properties"></a><span data-ttu-id="4c748-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="4c748-108">Properties</span></span>
| <span data-ttu-id="4c748-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c748-109">Property</span></span>     | <span data-ttu-id="4c748-110">Тип</span><span class="sxs-lookup"><span data-stu-id="4c748-110">Type</span></span>   |<span data-ttu-id="4c748-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4c748-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4c748-112">fileUrl</span><span class="sxs-lookup"><span data-stu-id="4c748-112">fileUrl</span></span>|<span data-ttu-id="4c748-113">String</span><span class="sxs-lookup"><span data-stu-id="4c748-113">String</span></span>|<span data-ttu-id="4c748-114">Расположение файла на диске.</span><span class="sxs-lookup"><span data-stu-id="4c748-114">Location of the file on disk.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4c748-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4c748-115">JSON representation</span></span>

<span data-ttu-id="4c748-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4c748-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationWordResource"
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
  "description": "educationWordResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


