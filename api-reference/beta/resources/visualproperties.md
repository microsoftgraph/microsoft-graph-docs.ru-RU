---
title: Тип ресурса Висуалпропертиес
description: 'Представляет визуальное содержимое, название и основной текст визуального уведомления, предназначенного для пользователя.  '
localization_priority: Normal
author: merzink
ms.prod: notifications
doc_type: resourcePageType
ms.openlocfilehash: f03563549cc1b2f42a274032dab7b310511c70c7
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939182"
---
# <a name="visualproperties-resource-type"></a><span data-ttu-id="f420b-103">Тип ресурса Висуалпропертиес</span><span class="sxs-lookup"><span data-stu-id="f420b-103">visualProperties resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f420b-104">Представляет визуальное содержимое, название и основной текст визуального уведомления, предназначенного для пользователя.</span><span class="sxs-lookup"><span data-stu-id="f420b-104">Represents the visual content, namely title and body, of a visual notification targeted to a user.</span></span> 

## <a name="properties"></a><span data-ttu-id="f420b-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="f420b-105">Properties</span></span>

| <span data-ttu-id="f420b-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="f420b-106">Property</span></span>     | <span data-ttu-id="f420b-107">Тип</span><span class="sxs-lookup"><span data-stu-id="f420b-107">Type</span></span>        | <span data-ttu-id="f420b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f420b-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f420b-109">title</span><span class="sxs-lookup"><span data-stu-id="f420b-109">title</span></span>|<span data-ttu-id="f420b-110">Строка</span><span class="sxs-lookup"><span data-stu-id="f420b-110">String</span></span>|<span data-ttu-id="f420b-111">Название визуального уведомления пользователя.</span><span class="sxs-lookup"><span data-stu-id="f420b-111">The title of a visual user notification.</span></span> <span data-ttu-id="f420b-112">Это поле является обязательным для полезных данных визуальных уведомлений.</span><span class="sxs-lookup"><span data-stu-id="f420b-112">This field is required for visual notification payloads.</span></span> |
|<span data-ttu-id="f420b-113">body</span><span class="sxs-lookup"><span data-stu-id="f420b-113">body</span></span>|<span data-ttu-id="f420b-114">Строка</span><span class="sxs-lookup"><span data-stu-id="f420b-114">String</span></span>|<span data-ttu-id="f420b-115">Текст уведомления визуального пользователя.</span><span class="sxs-lookup"><span data-stu-id="f420b-115">The body of a visual user notification.</span></span> <span data-ttu-id="f420b-116">Основной текст является необязательным.</span><span class="sxs-lookup"><span data-stu-id="f420b-116">Body is optional.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="f420b-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f420b-117">JSON representation</span></span>

<span data-ttu-id="f420b-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f420b-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.visualProperties",
  "baseType": null
}-->

```json
{
  "title": "String",
  "body": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "visualProperties resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->