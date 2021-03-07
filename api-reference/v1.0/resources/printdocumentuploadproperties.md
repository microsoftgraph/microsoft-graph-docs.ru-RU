---
author: nilakhan
description: Представляет сведения для отправки документов для печати
title: тип ресурса printDocumentUploadProperties
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-printing
ms.openlocfilehash: e877901b842670e09cb283b40613a1185aabaafe
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517945"
---
# <a name="printdocumentuploadproperties-resource-type"></a><span data-ttu-id="6732c-103">тип ресурса printDocumentUploadProperties</span><span class="sxs-lookup"><span data-stu-id="6732c-103">printDocumentUploadProperties resource type</span></span>

<span data-ttu-id="6732c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6732c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="6732c-105">Описание загружаемой документации</span><span class="sxs-lookup"><span data-stu-id="6732c-105">Describes the document that is being uploaded</span></span>

## <a name="properties"></a><span data-ttu-id="6732c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="6732c-106">Properties</span></span>
|<span data-ttu-id="6732c-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="6732c-107">Property</span></span>|<span data-ttu-id="6732c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="6732c-108">Type</span></span>|<span data-ttu-id="6732c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6732c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6732c-110">contentType</span><span class="sxs-lookup"><span data-stu-id="6732c-110">contentType</span></span>|<span data-ttu-id="6732c-111">String</span><span class="sxs-lookup"><span data-stu-id="6732c-111">String</span></span>|<span data-ttu-id="6732c-112">Тип контента документа (MIME).</span><span class="sxs-lookup"><span data-stu-id="6732c-112">The document's content (MIME) type.</span></span>|
|<span data-ttu-id="6732c-113">documentName</span><span class="sxs-lookup"><span data-stu-id="6732c-113">documentName</span></span>|<span data-ttu-id="6732c-114">Строка</span><span class="sxs-lookup"><span data-stu-id="6732c-114">String</span></span>|<span data-ttu-id="6732c-115">Имя документа.</span><span class="sxs-lookup"><span data-stu-id="6732c-115">The document's name.</span></span>|
|<span data-ttu-id="6732c-116">size</span><span class="sxs-lookup"><span data-stu-id="6732c-116">size</span></span>|<span data-ttu-id="6732c-117">Int64</span><span class="sxs-lookup"><span data-stu-id="6732c-117">Int64</span></span>|<span data-ttu-id="6732c-118">Размер документа в bytes.</span><span class="sxs-lookup"><span data-stu-id="6732c-118">The document's size in bytes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6732c-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="6732c-119">Relationships</span></span>
<span data-ttu-id="6732c-120">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="6732c-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6732c-121">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="6732c-121">JSON representation</span></span>
<span data-ttu-id="6732c-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6732c-122">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printDocumentUploadProperties"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printDocumentUploadProperties",
  "contentType": "String",
  "documentName": "String",
  "size": "Integer"
}
```

