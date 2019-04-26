---
title: Тип ресурса Агриментфиледата
description: Представляет большой двоичный объект условий использования файла соглашения Azure Active Directory (Azure AD).
localization_priority: Normal
ms.openlocfilehash: c6f4b6708493c0063928a81c95eeb60b7e7603b0
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339145"
---
# <a name="agreementfiledata-resource-type"></a><span data-ttu-id="fc64e-103">Тип ресурса Агриментфиледата</span><span class="sxs-lookup"><span data-stu-id="fc64e-103">agreementFileData resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc64e-104">Представляет большой двоичный объект условий использования файла соглашения Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="fc64e-104">Represents the blob of an Azure Active Directory (Azure AD) terms of use agreement file.</span></span>

## <a name="properties"></a><span data-ttu-id="fc64e-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="fc64e-105">Properties</span></span>
| <span data-ttu-id="fc64e-106">Метод</span><span class="sxs-lookup"><span data-stu-id="fc64e-106">Method</span></span>       | <span data-ttu-id="fc64e-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fc64e-107">Return Type</span></span> | <span data-ttu-id="fc64e-108">Описание</span><span class="sxs-lookup"><span data-stu-id="fc64e-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fc64e-109">data</span><span class="sxs-lookup"><span data-stu-id="fc64e-109">data</span></span>|<span data-ttu-id="fc64e-110">Двоичный</span><span class="sxs-lookup"><span data-stu-id="fc64e-110">Binary</span></span>|<span data-ttu-id="fc64e-111">Данные, представляющие условия использования PDF-документа.</span><span class="sxs-lookup"><span data-stu-id="fc64e-111">Data representing the terms of use PDF document.</span></span> <span data-ttu-id="fc64e-112">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fc64e-112">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fc64e-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fc64e-113">JSON representation</span></span>

<span data-ttu-id="fc64e-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fc64e-114">The following is a JSON representation of the resource.</span></span>

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
