---
title: Тип ресурса agreementFileData
description: Представляет blob Azure Active Directory (Azure AD) условия соглашения использовать файл.
localization_priority: Normal
ms.openlocfilehash: 64de3a72ad648225f24429987f5729f76ed8a2e7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815220"
---
# <a name="agreementfiledata-resource-type"></a><span data-ttu-id="2bc23-103">Тип ресурса agreementFileData</span><span class="sxs-lookup"><span data-stu-id="2bc23-103">agreementFileData resource type</span></span>

> <span data-ttu-id="2bc23-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2bc23-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2bc23-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2bc23-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2bc23-106">Представляет blob Azure Active Directory (Azure AD) условия соглашения использовать файл.</span><span class="sxs-lookup"><span data-stu-id="2bc23-106">Represents the blob of an Azure Active Directory (Azure AD) terms of use agreement file.</span></span>

## <a name="properties"></a><span data-ttu-id="2bc23-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2bc23-107">Properties</span></span>
| <span data-ttu-id="2bc23-108">Метод</span><span class="sxs-lookup"><span data-stu-id="2bc23-108">Method</span></span>       | <span data-ttu-id="2bc23-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2bc23-109">Return Type</span></span> | <span data-ttu-id="2bc23-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2bc23-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2bc23-111">data</span><span class="sxs-lookup"><span data-stu-id="2bc23-111">data</span></span>|<span data-ttu-id="2bc23-112">Binary</span><span class="sxs-lookup"><span data-stu-id="2bc23-112">Binary</span></span>|<span data-ttu-id="2bc23-113">Данные, представляющие условия использования PDF-документа.</span><span class="sxs-lookup"><span data-stu-id="2bc23-113">Data representing the terms of use PDF document.</span></span> <span data-ttu-id="2bc23-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2bc23-114">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2bc23-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2bc23-115">JSON representation</span></span>

<span data-ttu-id="2bc23-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2bc23-116">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "agreementFileData resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
