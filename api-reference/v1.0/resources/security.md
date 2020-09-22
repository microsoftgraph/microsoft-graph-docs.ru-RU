---
title: Тип ресурса "безопасность"
description: Ресурс Security — точка входа для объектной модели безопасности. Он возвращает одноэлементный ресурс безопасности. Он не содержит пригодных для использования свойств.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 0c120bccd3defa4cb56966c8cee26119472b3876
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47984007"
---
# <a name="security-resource-type"></a><span data-ttu-id="5d4e1-105">Тип ресурса "безопасность"</span><span class="sxs-lookup"><span data-stu-id="5d4e1-105">security resource type</span></span>

<span data-ttu-id="5d4e1-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d4e1-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5d4e1-107">Ресурс Security — точка входа для объектной модели безопасности.</span><span class="sxs-lookup"><span data-stu-id="5d4e1-107">The security resource is the entry point for the Security object model.</span></span> <span data-ttu-id="5d4e1-108">Он возвращает одноэлементный ресурс безопасности.</span><span class="sxs-lookup"><span data-stu-id="5d4e1-108">It returns a singleton security resource.</span></span> <span data-ttu-id="5d4e1-109">Он не содержит пригодных для использования свойств.</span><span class="sxs-lookup"><span data-stu-id="5d4e1-109">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="5d4e1-110">Методы</span><span class="sxs-lookup"><span data-stu-id="5d4e1-110">Methods</span></span>

| <span data-ttu-id="5d4e1-111">Метод</span><span class="sxs-lookup"><span data-stu-id="5d4e1-111">Method</span></span>       | <span data-ttu-id="5d4e1-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5d4e1-112">Return Type</span></span> | <span data-ttu-id="5d4e1-113">Описание</span><span class="sxs-lookup"><span data-stu-id="5d4e1-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="5d4e1-114">Перечисление оповещений</span><span class="sxs-lookup"><span data-stu-id="5d4e1-114">List alerts</span></span>](../api/alert-list.md) | <span data-ttu-id="5d4e1-115">Коллекция [alert](alert.md)</span><span class="sxs-lookup"><span data-stu-id="5d4e1-115">[alert](alert.md) collection</span></span> | <span data-ttu-id="5d4e1-116">Получение коллекции объектов Alert.</span><span class="sxs-lookup"><span data-stu-id="5d4e1-116">Get a alert object collection.</span></span> |
| [<span data-ttu-id="5d4e1-117">получение оповещений</span><span class="sxs-lookup"><span data-stu-id="5d4e1-117">get alerts</span></span>](../api/alert-get.md) | <span data-ttu-id="5d4e1-118">Коллекция [alert](alert.md)</span><span class="sxs-lookup"><span data-stu-id="5d4e1-118">[alert](alert.md) collection</span></span> | <span data-ttu-id="5d4e1-119">Получение объекта Alert.</span><span class="sxs-lookup"><span data-stu-id="5d4e1-119">Get a alert object.</span></span> |
| [<span data-ttu-id="5d4e1-120">Обновление оповещений</span><span class="sxs-lookup"><span data-stu-id="5d4e1-120">Update alerts</span></span>](../api/alert-update.md) | <span data-ttu-id="5d4e1-121">Коллекция [alert](alert.md)</span><span class="sxs-lookup"><span data-stu-id="5d4e1-121">[alert](alert.md) collection</span></span> | <span data-ttu-id="5d4e1-122">Получение объекта Alert.</span><span class="sxs-lookup"><span data-stu-id="5d4e1-122">Get a alert object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5d4e1-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="5d4e1-123">Properties</span></span>
<span data-ttu-id="5d4e1-124">Нет</span><span class="sxs-lookup"><span data-stu-id="5d4e1-124">None</span></span>

## <a name="relationships"></a><span data-ttu-id="5d4e1-125">Связи</span><span class="sxs-lookup"><span data-stu-id="5d4e1-125">Relationships</span></span>
| <span data-ttu-id="5d4e1-126">Связь</span><span class="sxs-lookup"><span data-stu-id="5d4e1-126">Relationship</span></span> | <span data-ttu-id="5d4e1-127">Тип</span><span class="sxs-lookup"><span data-stu-id="5d4e1-127">Type</span></span>        | <span data-ttu-id="5d4e1-128">Описание</span><span class="sxs-lookup"><span data-stu-id="5d4e1-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5d4e1-129">alerts</span><span class="sxs-lookup"><span data-stu-id="5d4e1-129">alerts</span></span>|<span data-ttu-id="5d4e1-130">Коллекция [alert](alert.md)</span><span class="sxs-lookup"><span data-stu-id="5d4e1-130">[alert](alert.md) collection</span></span>| <span data-ttu-id="5d4e1-p103">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="5d4e1-p103">Read-only. Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="5d4e1-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5d4e1-133">JSON representation</span></span>
<span data-ttu-id="5d4e1-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5d4e1-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.security"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="5d4e1-135">Пример</span><span class="sxs-lookup"><span data-stu-id="5d4e1-135">Example</span></span>

<span data-ttu-id="5d4e1-136">Ресурс **безопасности** доступен в корне графа.</span><span class="sxs-lookup"><span data-stu-id="5d4e1-136">The **security** resource is available at the root of the graph.</span></span>

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

