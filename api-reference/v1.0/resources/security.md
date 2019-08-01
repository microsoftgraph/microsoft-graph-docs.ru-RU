---
title: Тип ресурса "безопасность"
description: Ресурс Security — точка входа для объектной модели безопасности. Он возвращает одноэлементный ресурс безопасности. Он не содержит пригодных для использования свойств.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 87bd321a3c5e66cdc5d4fdc7fcb1407d02fbca1c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034456"
---
# <a name="security-resource-type"></a><span data-ttu-id="2dde1-105">Тип ресурса "безопасность"</span><span class="sxs-lookup"><span data-stu-id="2dde1-105">security resource type</span></span>

<span data-ttu-id="2dde1-106">Ресурс Security — точка входа для объектной модели безопасности.</span><span class="sxs-lookup"><span data-stu-id="2dde1-106">The security resource is the entry point for the Security object model.</span></span> <span data-ttu-id="2dde1-107">Он возвращает одноэлементный ресурс безопасности.</span><span class="sxs-lookup"><span data-stu-id="2dde1-107">It returns a singleton security resource.</span></span> <span data-ttu-id="2dde1-108">Он не содержит пригодных для использования свойств.</span><span class="sxs-lookup"><span data-stu-id="2dde1-108">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="2dde1-109">Методы</span><span class="sxs-lookup"><span data-stu-id="2dde1-109">Methods</span></span>

| <span data-ttu-id="2dde1-110">Метод</span><span class="sxs-lookup"><span data-stu-id="2dde1-110">Method</span></span>       | <span data-ttu-id="2dde1-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2dde1-111">Return Type</span></span> | <span data-ttu-id="2dde1-112">Описание</span><span class="sxs-lookup"><span data-stu-id="2dde1-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="2dde1-113">Перечисление оповещений</span><span class="sxs-lookup"><span data-stu-id="2dde1-113">List alerts</span></span>](../api/alert-list.md) | <span data-ttu-id="2dde1-114">Коллекция [alert](alert.md)</span><span class="sxs-lookup"><span data-stu-id="2dde1-114">[alert](alert.md) collection</span></span> | <span data-ttu-id="2dde1-115">Получение коллекции объектов Alert.</span><span class="sxs-lookup"><span data-stu-id="2dde1-115">Get a alert object collection.</span></span> |
| [<span data-ttu-id="2dde1-116">получение оповещений</span><span class="sxs-lookup"><span data-stu-id="2dde1-116">get alerts</span></span>](../api/alert-get.md) | <span data-ttu-id="2dde1-117">Коллекция [alert](alert.md)</span><span class="sxs-lookup"><span data-stu-id="2dde1-117">[alert](alert.md) collection</span></span> | <span data-ttu-id="2dde1-118">Получение объекта Alert.</span><span class="sxs-lookup"><span data-stu-id="2dde1-118">Get a alert object.</span></span> |
| [<span data-ttu-id="2dde1-119">Обновление оповещений</span><span class="sxs-lookup"><span data-stu-id="2dde1-119">Update alerts</span></span>](../api/alert-update.md) | <span data-ttu-id="2dde1-120">Коллекция [alert](alert.md)</span><span class="sxs-lookup"><span data-stu-id="2dde1-120">[alert](alert.md) collection</span></span> | <span data-ttu-id="2dde1-121">Получение объекта Alert.</span><span class="sxs-lookup"><span data-stu-id="2dde1-121">Get a alert object.</span></span> |

## <a name="properties"></a><span data-ttu-id="2dde1-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="2dde1-122">Properties</span></span>
<span data-ttu-id="2dde1-123">Нет</span><span class="sxs-lookup"><span data-stu-id="2dde1-123">None</span></span>

## <a name="relationships"></a><span data-ttu-id="2dde1-124">Отношения</span><span class="sxs-lookup"><span data-stu-id="2dde1-124">Relationships</span></span>
| <span data-ttu-id="2dde1-125">Отношение</span><span class="sxs-lookup"><span data-stu-id="2dde1-125">Relationship</span></span> | <span data-ttu-id="2dde1-126">Тип</span><span class="sxs-lookup"><span data-stu-id="2dde1-126">Type</span></span>        | <span data-ttu-id="2dde1-127">Описание</span><span class="sxs-lookup"><span data-stu-id="2dde1-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2dde1-128">alerts</span><span class="sxs-lookup"><span data-stu-id="2dde1-128">alerts</span></span>|<span data-ttu-id="2dde1-129">Коллекция [alert](alert.md)</span><span class="sxs-lookup"><span data-stu-id="2dde1-129">[alert](alert.md) collection</span></span>| <span data-ttu-id="2dde1-p103">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="2dde1-p103">Read-only. Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="2dde1-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2dde1-132">JSON representation</span></span>
<span data-ttu-id="2dde1-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2dde1-133">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.security"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="2dde1-134">Пример</span><span class="sxs-lookup"><span data-stu-id="2dde1-134">Example</span></span>

<span data-ttu-id="2dde1-135">Ресурс **безопасности** доступен в корне графа.</span><span class="sxs-lookup"><span data-stu-id="2dde1-135">The **security** resource is available at the root of the graph.</span></span>

<!--{
  "blockType": "request"
}-->
```http
GET https://graph.microsoft.com/v1.0/security
```

<!--{
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security"
}-->
```json
HTTP/1.1 200 OK
Content-type: application/json

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "security resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
