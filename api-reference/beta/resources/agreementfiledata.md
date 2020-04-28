---
title: Тип ресурса Агриментфиледата
description: Представляет большой двоичный объект условий использования файла соглашения Azure Active Directory (Azure AD).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 8758de3282bb59220423632be0be9c6e035c18b9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508368"
---
# <a name="agreementfiledata-resource-type"></a><span data-ttu-id="3be09-103">Тип ресурса Агриментфиледата</span><span class="sxs-lookup"><span data-stu-id="3be09-103">agreementFileData resource type</span></span>

<span data-ttu-id="3be09-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3be09-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3be09-105">Представляет большой двоичный объект условий использования файла соглашения Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="3be09-105">Represents the blob of an Azure Active Directory (Azure AD) terms of use agreement file.</span></span>

## <a name="properties"></a><span data-ttu-id="3be09-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="3be09-106">Properties</span></span>
| <span data-ttu-id="3be09-107">Метод</span><span class="sxs-lookup"><span data-stu-id="3be09-107">Method</span></span>       | <span data-ttu-id="3be09-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3be09-108">Return Type</span></span> | <span data-ttu-id="3be09-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3be09-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3be09-110">data</span><span class="sxs-lookup"><span data-stu-id="3be09-110">data</span></span>|<span data-ttu-id="3be09-111">Binary</span><span class="sxs-lookup"><span data-stu-id="3be09-111">Binary</span></span>|<span data-ttu-id="3be09-112">Данные, представляющие условия использования PDF-документа.</span><span class="sxs-lookup"><span data-stu-id="3be09-112">Data representing the terms of use PDF document.</span></span> <span data-ttu-id="3be09-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3be09-113">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3be09-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3be09-114">JSON representation</span></span>

<span data-ttu-id="3be09-115">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3be09-115">The following is a JSON representation of the resource.</span></span>

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
