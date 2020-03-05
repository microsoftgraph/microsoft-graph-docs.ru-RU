---
title: Тип ресурса Едукатионвордресаурце
description: 'Подкласс объекта Едукатионресаурце. Это ресурс документа Word. Файл Word необходимо отправить в каталоге **филересаурце** , связанном с '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 06b1f097199bbf188c0bc0a538fe471b07cdec91
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42499948"
---
# <a name="educationwordresource-resource-type"></a><span data-ttu-id="c7608-105">Тип ресурса Едукатионвордресаурце</span><span class="sxs-lookup"><span data-stu-id="c7608-105">educationWordResource resource type</span></span>

<span data-ttu-id="c7608-106">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c7608-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7608-107">Подкласс объекта [едукатионресаурце](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="c7608-107">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="c7608-108">Это ресурс документа Word.</span><span class="sxs-lookup"><span data-stu-id="c7608-108">This is a Word document resource.</span></span> <span data-ttu-id="c7608-109">Файл Word необходимо отправить в каталоге **филересаурце** , связанном с назначением или отправкой.</span><span class="sxs-lookup"><span data-stu-id="c7608-109">The Word file must be uploaded in the **fileResource** directory associated with the assignment or submission.</span></span>


## <a name="properties"></a><span data-ttu-id="c7608-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="c7608-110">Properties</span></span>
| <span data-ttu-id="c7608-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="c7608-111">Property</span></span>     | <span data-ttu-id="c7608-112">Тип</span><span class="sxs-lookup"><span data-stu-id="c7608-112">Type</span></span>   |<span data-ttu-id="c7608-113">Описание</span><span class="sxs-lookup"><span data-stu-id="c7608-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c7608-114">fileUrl</span><span class="sxs-lookup"><span data-stu-id="c7608-114">fileUrl</span></span>|<span data-ttu-id="c7608-115">String</span><span class="sxs-lookup"><span data-stu-id="c7608-115">String</span></span>|<span data-ttu-id="c7608-116">Расположение файла на диске.</span><span class="sxs-lookup"><span data-stu-id="c7608-116">Location of the file on disk.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c7608-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c7608-117">JSON representation</span></span>

<span data-ttu-id="c7608-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c7608-118">The following is a JSON representation of the resource.</span></span>

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
