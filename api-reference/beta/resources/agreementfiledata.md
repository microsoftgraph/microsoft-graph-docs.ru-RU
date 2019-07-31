---
title: Тип ресурса Агриментфиледата
description: Представляет большой двоичный объект условий использования файла соглашения Azure Active Directory (Azure AD).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: da4e600480e6ddd65112323b22f7a905b3ba29db
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013425"
---
# <a name="agreementfiledata-resource-type"></a><span data-ttu-id="65219-103">Тип ресурса Агриментфиледата</span><span class="sxs-lookup"><span data-stu-id="65219-103">agreementFileData resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65219-104">Представляет большой двоичный объект условий использования файла соглашения Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="65219-104">Represents the blob of an Azure Active Directory (Azure AD) terms of use agreement file.</span></span>

## <a name="properties"></a><span data-ttu-id="65219-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="65219-105">Properties</span></span>
| <span data-ttu-id="65219-106">Метод</span><span class="sxs-lookup"><span data-stu-id="65219-106">Method</span></span>       | <span data-ttu-id="65219-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="65219-107">Return Type</span></span> | <span data-ttu-id="65219-108">Описание</span><span class="sxs-lookup"><span data-stu-id="65219-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="65219-109">data</span><span class="sxs-lookup"><span data-stu-id="65219-109">data</span></span>|<span data-ttu-id="65219-110">Binary</span><span class="sxs-lookup"><span data-stu-id="65219-110">Binary</span></span>|<span data-ttu-id="65219-111">Данные, представляющие условия использования PDF-документа.</span><span class="sxs-lookup"><span data-stu-id="65219-111">Data representing the terms of use PDF document.</span></span> <span data-ttu-id="65219-112">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="65219-112">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="65219-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="65219-113">JSON representation</span></span>

<span data-ttu-id="65219-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="65219-114">The following is a JSON representation of the resource.</span></span>

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
