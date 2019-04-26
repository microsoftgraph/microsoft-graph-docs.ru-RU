---
title: Тип ресурса Едукатионфилересаурце
description: Подкласс Едукатионресаурце, представляющий объект File, связанный с назначением или отправкой.  В этом случае файл не является одним из специальных файлов (Word, Excel и т. д.), но это файл, для которого не определена специальная обработка в системе. Файловый ресурс должен храниться в **ресаурцефолдер** , связанном с назначением или отправкой, к которому присоединен этот ресурс.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9a851c66e137da1941df9b0268657c9e1b7392b3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334249"
---
# <a name="educationfileresource-resource-type"></a><span data-ttu-id="358b3-105">Тип ресурса Едукатионфилересаурце</span><span class="sxs-lookup"><span data-stu-id="358b3-105">educationFileResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="358b3-106">Подкласс [едукатионресаурце](educationresource.md) , представляющий объект File, связанный с назначением или отправкой.</span><span class="sxs-lookup"><span data-stu-id="358b3-106">A subclass of [educationResource](educationresource.md) that represents a file object that is associated with the assignment or submission.</span></span>  <span data-ttu-id="358b3-107">В этом случае файл не является одним из специальных файлов (Word, Excel и т. д.), но это файл, для которого не определена специальная обработка в системе.</span><span class="sxs-lookup"><span data-stu-id="358b3-107">In this case, the file is not one of the special files (Word, Excel, and so on) but is a file that does not have special handling within the system.</span></span> <span data-ttu-id="358b3-108">Файловый ресурс должен храниться в **ресаурцефолдер** , связанном с назначением или отправкой, к которому присоединен этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="358b3-108">The file resource must be stored in the **resourceFolder** that is associated with the assignment or submission this resource is attached to.</span></span>

## <a name="properties"></a><span data-ttu-id="358b3-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="358b3-109">Properties</span></span>
| <span data-ttu-id="358b3-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="358b3-110">Property</span></span>     | <span data-ttu-id="358b3-111">Тип</span><span class="sxs-lookup"><span data-stu-id="358b3-111">Type</span></span>   |<span data-ttu-id="358b3-112">Описание</span><span class="sxs-lookup"><span data-stu-id="358b3-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="358b3-113">fileUrl</span><span class="sxs-lookup"><span data-stu-id="358b3-113">fileUrl</span></span>|<span data-ttu-id="358b3-114">String</span><span class="sxs-lookup"><span data-stu-id="358b3-114">String</span></span>|<span data-ttu-id="358b3-115">Расположение на диске файлового ресурса.</span><span class="sxs-lookup"><span data-stu-id="358b3-115">Location on disk of the file resource.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="358b3-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="358b3-116">JSON representation</span></span>

<span data-ttu-id="358b3-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="358b3-117">The following is a JSON representation of the resource.</span></span>

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
