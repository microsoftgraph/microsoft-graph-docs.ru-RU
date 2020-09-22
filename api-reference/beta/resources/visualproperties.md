---
title: Тип ресурса Висуалпропертиес
description: 'Представляет визуальное содержимое, название и основной текст визуального уведомления, предназначенного для пользователя.  '
localization_priority: Normal
author: merzink
ms.prod: notifications
doc_type: resourcePageType
ms.openlocfilehash: 62580847844a4b397ed117ea4b256cc4f035577a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057691"
---
# <a name="visualproperties-resource-type"></a><span data-ttu-id="24641-103">Тип ресурса Висуалпропертиес</span><span class="sxs-lookup"><span data-stu-id="24641-103">visualProperties resource type</span></span>

<span data-ttu-id="24641-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24641-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24641-105">Представляет визуальное содержимое, название и основной текст визуального уведомления, предназначенного для пользователя.</span><span class="sxs-lookup"><span data-stu-id="24641-105">Represents the visual content, namely title and body, of a visual notification targeted to a user.</span></span> 

## <a name="properties"></a><span data-ttu-id="24641-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="24641-106">Properties</span></span>

| <span data-ttu-id="24641-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="24641-107">Property</span></span>     | <span data-ttu-id="24641-108">Тип</span><span class="sxs-lookup"><span data-stu-id="24641-108">Type</span></span>        | <span data-ttu-id="24641-109">Описание</span><span class="sxs-lookup"><span data-stu-id="24641-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="24641-110">title</span><span class="sxs-lookup"><span data-stu-id="24641-110">title</span></span>|<span data-ttu-id="24641-111">String</span><span class="sxs-lookup"><span data-stu-id="24641-111">String</span></span>|<span data-ttu-id="24641-112">Название визуального уведомления пользователя.</span><span class="sxs-lookup"><span data-stu-id="24641-112">The title of a visual user notification.</span></span> <span data-ttu-id="24641-113">Это поле является обязательным для полезных данных визуальных уведомлений.</span><span class="sxs-lookup"><span data-stu-id="24641-113">This field is required for visual notification payloads.</span></span> |
|<span data-ttu-id="24641-114">body</span><span class="sxs-lookup"><span data-stu-id="24641-114">body</span></span>|<span data-ttu-id="24641-115">String</span><span class="sxs-lookup"><span data-stu-id="24641-115">String</span></span>|<span data-ttu-id="24641-116">Текст уведомления визуального пользователя.</span><span class="sxs-lookup"><span data-stu-id="24641-116">The body of a visual user notification.</span></span> <span data-ttu-id="24641-117">Основной текст является необязательным.</span><span class="sxs-lookup"><span data-stu-id="24641-117">Body is optional.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="24641-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="24641-118">JSON representation</span></span>

<span data-ttu-id="24641-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="24641-119">The following is a JSON representation of the resource.</span></span>

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

