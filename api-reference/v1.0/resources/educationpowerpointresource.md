---
title: тип ресурсов educationPowerPointResource
description: Подкласс educationResource.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 860387ea966061077929781f667a9cac5d3d2107
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912805"
---
# <a name="educationpowerpointresource-resource-type"></a><span data-ttu-id="5f186-103">тип ресурсов educationPowerPointResource</span><span class="sxs-lookup"><span data-stu-id="5f186-103">educationPowerPointResource resource type</span></span>

<span data-ttu-id="5f186-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f186-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5f186-105">Подкласс [educationResource](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="5f186-105">A subclass of [educationResource](educationresource.md).</span></span> 

<span data-ttu-id="5f186-106">Это ресурс PowerPoint.</span><span class="sxs-lookup"><span data-stu-id="5f186-106">This is a PowerPoint resource.</span></span> <span data-ttu-id="5f186-107">Файл PowerPoint должен быть загружен в **каталог fileResource,** связанный с назначением или отправкой.</span><span class="sxs-lookup"><span data-stu-id="5f186-107">The PowerPoint file must be uploaded in the **fileResource** directory associated with the assignment or submission.</span></span>


## <a name="properties"></a><span data-ttu-id="5f186-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="5f186-108">Properties</span></span>
| <span data-ttu-id="5f186-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="5f186-109">Property</span></span>     | <span data-ttu-id="5f186-110">Тип</span><span class="sxs-lookup"><span data-stu-id="5f186-110">Type</span></span>   |<span data-ttu-id="5f186-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5f186-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5f186-112">fileUrl</span><span class="sxs-lookup"><span data-stu-id="5f186-112">fileUrl</span></span>|<span data-ttu-id="5f186-113">String</span><span class="sxs-lookup"><span data-stu-id="5f186-113">String</span></span>|<span data-ttu-id="5f186-114">Расположение файла на диске.</span><span class="sxs-lookup"><span data-stu-id="5f186-114">Location of the file on disk.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5f186-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5f186-115">JSON representation</span></span>

<span data-ttu-id="5f186-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5f186-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationPowerPointResource"
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
  "description": "educationPowerPointResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


