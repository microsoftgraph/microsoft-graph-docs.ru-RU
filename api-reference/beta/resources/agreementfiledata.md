---
title: Тип ресурса agreementFileData
description: Представляет blob Azure Active Directory (Azure AD) условия соглашения использовать файл.
ms.openlocfilehash: 557725e14f4954f8b2c10112e1013beb71dda0be
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078732"
---
# <a name="agreementfiledata-resource-type"></a><span data-ttu-id="a5513-103">Тип ресурса agreementFileData</span><span class="sxs-lookup"><span data-stu-id="a5513-103">agreementFileData resource type</span></span>

> <span data-ttu-id="a5513-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a5513-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a5513-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5513-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a5513-106">Представляет blob Azure Active Directory (Azure AD) условия соглашения использовать файл.</span><span class="sxs-lookup"><span data-stu-id="a5513-106">Represents the blob of an Azure Active Directory (Azure AD) terms of use agreement file.</span></span>

## <a name="properties"></a><span data-ttu-id="a5513-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a5513-107">Properties</span></span>
| <span data-ttu-id="a5513-108">Метод</span><span class="sxs-lookup"><span data-stu-id="a5513-108">Method</span></span>       | <span data-ttu-id="a5513-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a5513-109">Return Type</span></span> | <span data-ttu-id="a5513-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a5513-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a5513-111">data</span><span class="sxs-lookup"><span data-stu-id="a5513-111">data</span></span>|<span data-ttu-id="a5513-112">Двоичный</span><span class="sxs-lookup"><span data-stu-id="a5513-112">Binary</span></span>|<span data-ttu-id="a5513-113">Данные, представляющие условия использования PDF-документа.</span><span class="sxs-lookup"><span data-stu-id="a5513-113">Data representing the terms of use PDF document.</span></span> <span data-ttu-id="a5513-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a5513-114">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a5513-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a5513-115">JSON representation</span></span>

<span data-ttu-id="a5513-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a5513-116">The following is a JSON representation of the resource.</span></span>

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
