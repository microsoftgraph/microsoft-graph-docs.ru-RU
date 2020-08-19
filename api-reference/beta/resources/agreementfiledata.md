---
title: Тип ресурса Агриментфиледата
description: Представляет большой двоичный объект условий использования файла соглашения Azure Active Directory (Azure AD).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: raprakasMSFT
ms.openlocfilehash: cb982ff8019c4b23c986de6a3c6f61501e56bba7
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807569"
---
# <a name="agreementfiledata-resource-type"></a><span data-ttu-id="ffcc5-103">Тип ресурса Агриментфиледата</span><span class="sxs-lookup"><span data-stu-id="ffcc5-103">agreementFileData resource type</span></span>

<span data-ttu-id="ffcc5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ffcc5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ffcc5-105">Представляет большой двоичный объект условий использования файла соглашения Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="ffcc5-105">Represents the blob of an Azure Active Directory (Azure AD) terms of use agreement file.</span></span>

## <a name="properties"></a><span data-ttu-id="ffcc5-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="ffcc5-106">Properties</span></span>
| <span data-ttu-id="ffcc5-107">Метод</span><span class="sxs-lookup"><span data-stu-id="ffcc5-107">Method</span></span>       | <span data-ttu-id="ffcc5-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ffcc5-108">Return Type</span></span> | <span data-ttu-id="ffcc5-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ffcc5-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ffcc5-110">data</span><span class="sxs-lookup"><span data-stu-id="ffcc5-110">data</span></span>|<span data-ttu-id="ffcc5-111">Binary</span><span class="sxs-lookup"><span data-stu-id="ffcc5-111">Binary</span></span>|<span data-ttu-id="ffcc5-112">Данные, представляющие условия использования PDF-документа.</span><span class="sxs-lookup"><span data-stu-id="ffcc5-112">Data representing the terms of use PDF document.</span></span> <span data-ttu-id="ffcc5-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ffcc5-113">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ffcc5-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ffcc5-114">JSON representation</span></span>

<span data-ttu-id="ffcc5-115">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ffcc5-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreementFileData"
}-->

```json
{
  "data": "Binary"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreementFileData resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
