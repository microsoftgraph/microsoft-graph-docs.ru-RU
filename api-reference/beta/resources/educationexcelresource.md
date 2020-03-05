---
title: Тип ресурса Едукатионексцелресаурце
description: 'Подкласс объекта Едукатионресаурце. Этот тип ресурса представляет документ Excel.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b533d5072ab9a4e880b14b64e96f4791db399e09
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502167"
---
# <a name="educationexcelresource-resource-type"></a><span data-ttu-id="b931d-104">Тип ресурса Едукатионексцелресаурце</span><span class="sxs-lookup"><span data-stu-id="b931d-104">educationExcelResource resource type</span></span>

<span data-ttu-id="b931d-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b931d-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b931d-106">Подкласс объекта [едукатионресаурце](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="b931d-106">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="b931d-107">Этот тип ресурса представляет документ Excel.</span><span class="sxs-lookup"><span data-stu-id="b931d-107">This resource type represents an Excel document.</span></span>  
 
><span data-ttu-id="b931d-108">**Примечание:** Файл Excel должен находиться в папке ресурсов, связанной с назначением или объектом отправки, к которому принадлежит ресурс.</span><span class="sxs-lookup"><span data-stu-id="b931d-108">**Note:** The Excel file must be in the resource folder associated with the assignment or submission object to which this resource belongs.</span></span>


## <a name="properties"></a><span data-ttu-id="b931d-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="b931d-109">Properties</span></span>
| <span data-ttu-id="b931d-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="b931d-110">Property</span></span>     | <span data-ttu-id="b931d-111">Тип</span><span class="sxs-lookup"><span data-stu-id="b931d-111">Type</span></span>   |<span data-ttu-id="b931d-112">Описание</span><span class="sxs-lookup"><span data-stu-id="b931d-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b931d-113">fileUrl</span><span class="sxs-lookup"><span data-stu-id="b931d-113">fileUrl</span></span>|<span data-ttu-id="b931d-114">String</span><span class="sxs-lookup"><span data-stu-id="b931d-114">String</span></span>|<span data-ttu-id="b931d-115">Указатель на объект файла Excel.</span><span class="sxs-lookup"><span data-stu-id="b931d-115">Pointer to the Excel file object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b931d-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b931d-116">JSON representation</span></span>

<span data-ttu-id="b931d-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b931d-117">The following is a JSON representation of the resource.</span></span>

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
