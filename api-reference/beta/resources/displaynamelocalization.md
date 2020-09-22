---
title: Тип ресурса Дисплайнамелокализатион
description: Предоставляет администратору возможность настраивать строку, используемую в общедоступном интерфейсе Microsoft 365.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: e02af0d4fcd5cdf4ce08df4403736bd6b9c60a84
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48010404"
---
# <a name="displaynamelocalization-resource-type"></a><span data-ttu-id="a8f1e-103">Тип ресурса Дисплайнамелокализатион</span><span class="sxs-lookup"><span data-stu-id="a8f1e-103">displayNameLocalization resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8f1e-104">Предоставляет администратору возможность настраивать строку, используемую в общедоступном интерфейсе Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="a8f1e-104">Provides the ability for an administrator to customize the string used in a shared Microsoft 365 experience.</span></span>

## <a name="properties"></a><span data-ttu-id="a8f1e-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="a8f1e-105">Properties</span></span>

| <span data-ttu-id="a8f1e-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="a8f1e-106">Property</span></span>     | <span data-ttu-id="a8f1e-107">Тип</span><span class="sxs-lookup"><span data-stu-id="a8f1e-107">Type</span></span>        | <span data-ttu-id="a8f1e-108">Описание</span><span class="sxs-lookup"><span data-stu-id="a8f1e-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a8f1e-109">displayName</span><span class="sxs-lookup"><span data-stu-id="a8f1e-109">displayName</span></span>   |<span data-ttu-id="a8f1e-110">String</span><span class="sxs-lookup"><span data-stu-id="a8f1e-110">String</span></span>       | <span data-ttu-id="a8f1e-111">Если этот параметр задан, то значение этого поля содержит строку **DisplayName** , заданную для языка, который указан в поле **лангуажетаг** .</span><span class="sxs-lookup"><span data-stu-id="a8f1e-111">If present, the value of this field contains the **displayName** string that has been set for the language present in the **languageTag** field.</span></span>|
|<span data-ttu-id="a8f1e-112">лангуажетаг</span><span class="sxs-lookup"><span data-stu-id="a8f1e-112">languageTag</span></span>   |<span data-ttu-id="a8f1e-113">String</span><span class="sxs-lookup"><span data-stu-id="a8f1e-113">String</span></span>       | <span data-ttu-id="a8f1e-114">Предоставляет язык и региональные параметры, а также понятное имя языка, в котором указано поле **DisplayName** .</span><span class="sxs-lookup"><span data-stu-id="a8f1e-114">Provides the language culture-code and friendly name of the language that the **displayName** field has been provided in.</span></span>                  |

## <a name="json-representation"></a><span data-ttu-id="a8f1e-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a8f1e-115">JSON representation</span></span>

<span data-ttu-id="a8f1e-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a8f1e-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.displayNameLocalization",
  "baseType": null
}-->

```json
{
  "displayName": "string",
  "languageTag": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "displayNameLocalization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


