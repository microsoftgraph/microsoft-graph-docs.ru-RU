---
title: Тип ресурса Маилтипсеррор
description: Ошибка, возникающая во время действия.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 0c17a2fa6cd5475c043fddadef735599c954779d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009820"
---
# <a name="mailtipserror-resource-type"></a><span data-ttu-id="f7e6b-103">Тип ресурса Маилтипсеррор</span><span class="sxs-lookup"><span data-stu-id="f7e6b-103">mailTipsError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7e6b-104">Ошибка, возникающая во время действия.</span><span class="sxs-lookup"><span data-stu-id="f7e6b-104">An error that occurs during an action.</span></span>

## <a name="properties"></a><span data-ttu-id="f7e6b-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="f7e6b-105">Properties</span></span>
| <span data-ttu-id="f7e6b-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="f7e6b-106">Property</span></span>     | <span data-ttu-id="f7e6b-107">Тип</span><span class="sxs-lookup"><span data-stu-id="f7e6b-107">Type</span></span>   |<span data-ttu-id="f7e6b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f7e6b-108">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="f7e6b-109">message</span><span class="sxs-lookup"><span data-stu-id="f7e6b-109">message</span></span> | <span data-ttu-id="f7e6b-110">String</span><span class="sxs-lookup"><span data-stu-id="f7e6b-110">String</span></span> | <span data-ttu-id="f7e6b-111">Сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="f7e6b-111">The error message.</span></span> |
| <span data-ttu-id="f7e6b-112">code</span><span class="sxs-lookup"><span data-stu-id="f7e6b-112">code</span></span> | <span data-ttu-id="f7e6b-113">String</span><span class="sxs-lookup"><span data-stu-id="f7e6b-113">String</span></span> | <span data-ttu-id="f7e6b-114">Код ошибки.</span><span class="sxs-lookup"><span data-stu-id="f7e6b-114">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f7e6b-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f7e6b-115">JSON representation</span></span>

<span data-ttu-id="f7e6b-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f7e6b-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mailTipsError"
}-->

```json
{
  "message": "string",
  "code": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mailTipsError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
