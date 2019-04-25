---
title: Тип ресурса Агриментфиледата
description: Представляет большой двоичный объект условий использования файла соглашения Azure Active Directory (Azure AD).
localization_priority: Normal
ms.openlocfilehash: bc0e7395875f64a3ee52e43b26da1a2df6276c9c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544133"
---
# <a name="agreementfiledata-resource-type"></a><span data-ttu-id="a85a0-103">Тип ресурса Агриментфиледата</span><span class="sxs-lookup"><span data-stu-id="a85a0-103">agreementFileData resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a85a0-104">Представляет большой двоичный объект условий использования файла соглашения Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="a85a0-104">Represents the blob of an Azure Active Directory (Azure AD) terms of use agreement file.</span></span>

## <a name="properties"></a><span data-ttu-id="a85a0-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="a85a0-105">Properties</span></span>
| <span data-ttu-id="a85a0-106">Метод</span><span class="sxs-lookup"><span data-stu-id="a85a0-106">Method</span></span>       | <span data-ttu-id="a85a0-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a85a0-107">Return Type</span></span> | <span data-ttu-id="a85a0-108">Описание</span><span class="sxs-lookup"><span data-stu-id="a85a0-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a85a0-109">data</span><span class="sxs-lookup"><span data-stu-id="a85a0-109">data</span></span>|<span data-ttu-id="a85a0-110">Двоичный</span><span class="sxs-lookup"><span data-stu-id="a85a0-110">Binary</span></span>|<span data-ttu-id="a85a0-111">Данные, представляющие условия использования PDF-документа.</span><span class="sxs-lookup"><span data-stu-id="a85a0-111">Data representing the terms of use PDF document.</span></span> <span data-ttu-id="a85a0-112">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a85a0-112">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a85a0-113">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a85a0-113">JSON representation</span></span>

<span data-ttu-id="a85a0-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a85a0-114">The following is a JSON representation of the resource.</span></span>

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
