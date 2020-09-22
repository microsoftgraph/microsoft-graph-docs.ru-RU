---
title: Тип ресурса Едукатионфилересаурце
description: Подкласс Едукатионресаурце, представляющий объект File, связанный с назначением или отправкой.  В этом случае файл не является одним из специальных файлов (Word, Excel и т. д.), но это файл, для которого не определена специальная обработка в системе. Файловый ресурс должен храниться в **ресаурцефолдер** , связанном с назначением или отправкой, к которому присоединен этот ресурс.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: cafef836f1e6f6fb4c2e379f9b9ad618f2519f72
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095452"
---
# <a name="educationfileresource-resource-type"></a><span data-ttu-id="b31ef-105">Тип ресурса Едукатионфилересаурце</span><span class="sxs-lookup"><span data-stu-id="b31ef-105">educationFileResource resource type</span></span>

<span data-ttu-id="b31ef-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b31ef-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b31ef-107">Подкласс [едукатионресаурце](educationresource.md) , представляющий объект File, связанный с назначением или отправкой.</span><span class="sxs-lookup"><span data-stu-id="b31ef-107">A subclass of [educationResource](educationresource.md) that represents a file object that is associated with the assignment or submission.</span></span>  <span data-ttu-id="b31ef-108">В этом случае файл не является одним из специальных файлов (Word, Excel и т. д.), но это файл, для которого не определена специальная обработка в системе.</span><span class="sxs-lookup"><span data-stu-id="b31ef-108">In this case, the file is not one of the special files (Word, Excel, and so on) but is a file that does not have special handling within the system.</span></span> <span data-ttu-id="b31ef-109">Файловый ресурс должен храниться в **ресаурцефолдер** , связанном с назначением или отправкой, к которому присоединен этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="b31ef-109">The file resource must be stored in the **resourceFolder** that is associated with the assignment or submission this resource is attached to.</span></span>

## <a name="properties"></a><span data-ttu-id="b31ef-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="b31ef-110">Properties</span></span>
| <span data-ttu-id="b31ef-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="b31ef-111">Property</span></span>     | <span data-ttu-id="b31ef-112">Тип</span><span class="sxs-lookup"><span data-stu-id="b31ef-112">Type</span></span>   |<span data-ttu-id="b31ef-113">Описание</span><span class="sxs-lookup"><span data-stu-id="b31ef-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b31ef-114">fileUrl</span><span class="sxs-lookup"><span data-stu-id="b31ef-114">fileUrl</span></span>|<span data-ttu-id="b31ef-115">Строка</span><span class="sxs-lookup"><span data-stu-id="b31ef-115">String</span></span>|<span data-ttu-id="b31ef-116">Расположение на диске файлового ресурса.</span><span class="sxs-lookup"><span data-stu-id="b31ef-116">Location on disk of the file resource.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b31ef-117">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b31ef-117">JSON representation</span></span>

<span data-ttu-id="b31ef-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b31ef-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFileResource"
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
  "description": "educationFileResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


