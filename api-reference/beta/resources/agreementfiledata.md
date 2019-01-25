---
title: Тип ресурса agreementFileData
description: Представляет blob Azure Active Directory (Azure AD) условия соглашения использовать файл.
localization_priority: Normal
ms.openlocfilehash: bc0e7395875f64a3ee52e43b26da1a2df6276c9c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517031"
---
# <a name="agreementfiledata-resource-type"></a><span data-ttu-id="eac76-103">Тип ресурса agreementFileData</span><span class="sxs-lookup"><span data-stu-id="eac76-103">agreementFileData resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eac76-104">Представляет blob Azure Active Directory (Azure AD) условия соглашения использовать файл.</span><span class="sxs-lookup"><span data-stu-id="eac76-104">Represents the blob of an Azure Active Directory (Azure AD) terms of use agreement file.</span></span>

## <a name="properties"></a><span data-ttu-id="eac76-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="eac76-105">Properties</span></span>
| <span data-ttu-id="eac76-106">Метод</span><span class="sxs-lookup"><span data-stu-id="eac76-106">Method</span></span>       | <span data-ttu-id="eac76-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="eac76-107">Return Type</span></span> | <span data-ttu-id="eac76-108">Описание</span><span class="sxs-lookup"><span data-stu-id="eac76-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="eac76-109">data</span><span class="sxs-lookup"><span data-stu-id="eac76-109">data</span></span>|<span data-ttu-id="eac76-110">Binary</span><span class="sxs-lookup"><span data-stu-id="eac76-110">Binary</span></span>|<span data-ttu-id="eac76-111">Данные, представляющие условия использования PDF-документа.</span><span class="sxs-lookup"><span data-stu-id="eac76-111">Data representing the terms of use PDF document.</span></span> <span data-ttu-id="eac76-112">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="eac76-112">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eac76-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eac76-113">JSON representation</span></span>

<span data-ttu-id="eac76-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eac76-114">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/agreementfiledata.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
