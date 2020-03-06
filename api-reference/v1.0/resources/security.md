---
title: Тип ресурса "безопасность"
description: Ресурс Security — точка входа для объектной модели безопасности. Он возвращает одноэлементный ресурс безопасности. Он не содержит пригодных для использования свойств.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 89db6a8efbf50042e5514758ee5a7ae3b7f88de6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533767"
---
# <a name="security-resource-type"></a><span data-ttu-id="354d2-105">Тип ресурса "безопасность"</span><span class="sxs-lookup"><span data-stu-id="354d2-105">security resource type</span></span>

<span data-ttu-id="354d2-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="354d2-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="354d2-107">Ресурс Security — точка входа для объектной модели безопасности.</span><span class="sxs-lookup"><span data-stu-id="354d2-107">The security resource is the entry point for the Security object model.</span></span> <span data-ttu-id="354d2-108">Он возвращает одноэлементный ресурс безопасности.</span><span class="sxs-lookup"><span data-stu-id="354d2-108">It returns a singleton security resource.</span></span> <span data-ttu-id="354d2-109">Он не содержит пригодных для использования свойств.</span><span class="sxs-lookup"><span data-stu-id="354d2-109">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="354d2-110">Методы</span><span class="sxs-lookup"><span data-stu-id="354d2-110">Methods</span></span>

| <span data-ttu-id="354d2-111">Метод</span><span class="sxs-lookup"><span data-stu-id="354d2-111">Method</span></span>       | <span data-ttu-id="354d2-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="354d2-112">Return Type</span></span> | <span data-ttu-id="354d2-113">Описание</span><span class="sxs-lookup"><span data-stu-id="354d2-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="354d2-114">Перечисление оповещений</span><span class="sxs-lookup"><span data-stu-id="354d2-114">List alerts</span></span>](../api/alert-list.md) | <span data-ttu-id="354d2-115">Коллекция [alert](alert.md)</span><span class="sxs-lookup"><span data-stu-id="354d2-115">[alert](alert.md) collection</span></span> | <span data-ttu-id="354d2-116">Получение коллекции объектов Alert.</span><span class="sxs-lookup"><span data-stu-id="354d2-116">Get a alert object collection.</span></span> |
| [<span data-ttu-id="354d2-117">получение оповещений</span><span class="sxs-lookup"><span data-stu-id="354d2-117">get alerts</span></span>](../api/alert-get.md) | <span data-ttu-id="354d2-118">Коллекция [alert](alert.md)</span><span class="sxs-lookup"><span data-stu-id="354d2-118">[alert](alert.md) collection</span></span> | <span data-ttu-id="354d2-119">Получение объекта Alert.</span><span class="sxs-lookup"><span data-stu-id="354d2-119">Get a alert object.</span></span> |
| [<span data-ttu-id="354d2-120">Обновление оповещений</span><span class="sxs-lookup"><span data-stu-id="354d2-120">Update alerts</span></span>](../api/alert-update.md) | <span data-ttu-id="354d2-121">Коллекция [alert](alert.md)</span><span class="sxs-lookup"><span data-stu-id="354d2-121">[alert](alert.md) collection</span></span> | <span data-ttu-id="354d2-122">Получение объекта Alert.</span><span class="sxs-lookup"><span data-stu-id="354d2-122">Get a alert object.</span></span> |

## <a name="properties"></a><span data-ttu-id="354d2-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="354d2-123">Properties</span></span>
<span data-ttu-id="354d2-124">Нет</span><span class="sxs-lookup"><span data-stu-id="354d2-124">None</span></span>

## <a name="relationships"></a><span data-ttu-id="354d2-125">Связи</span><span class="sxs-lookup"><span data-stu-id="354d2-125">Relationships</span></span>
| <span data-ttu-id="354d2-126">Связь</span><span class="sxs-lookup"><span data-stu-id="354d2-126">Relationship</span></span> | <span data-ttu-id="354d2-127">Тип</span><span class="sxs-lookup"><span data-stu-id="354d2-127">Type</span></span>        | <span data-ttu-id="354d2-128">Описание</span><span class="sxs-lookup"><span data-stu-id="354d2-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="354d2-129">alerts</span><span class="sxs-lookup"><span data-stu-id="354d2-129">alerts</span></span>|<span data-ttu-id="354d2-130">Коллекция [alert](alert.md)</span><span class="sxs-lookup"><span data-stu-id="354d2-130">[alert](alert.md) collection</span></span>| <span data-ttu-id="354d2-p103">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="354d2-p103">Read-only. Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="354d2-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="354d2-133">JSON representation</span></span>
<span data-ttu-id="354d2-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="354d2-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.security"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="354d2-135">Пример</span><span class="sxs-lookup"><span data-stu-id="354d2-135">Example</span></span>

<span data-ttu-id="354d2-136">Ресурс **безопасности** доступен в корне графа.</span><span class="sxs-lookup"><span data-stu-id="354d2-136">The **security** resource is available at the root of the graph.</span></span>

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
