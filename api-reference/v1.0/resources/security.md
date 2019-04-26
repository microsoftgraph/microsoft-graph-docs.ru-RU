---
title: Тип ресурса "безопасность"
description: Ресурс Security — точка входа для объектной модели безопасности. Он возвращает одноэлементный ресурс безопасности. Он не содержит пригодных для использования свойств.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: c7bf3f279e50efb451188426d030e356d55ad6be
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579214"
---
# <a name="security-resource-type"></a><span data-ttu-id="80fd5-105">Тип ресурса "безопасность"</span><span class="sxs-lookup"><span data-stu-id="80fd5-105">security resource type</span></span>

<span data-ttu-id="80fd5-106">Ресурс Security — точка входа для объектной модели безопасности.</span><span class="sxs-lookup"><span data-stu-id="80fd5-106">The security resource is the entry point for the Security object model.</span></span> <span data-ttu-id="80fd5-107">Он возвращает одноэлементный ресурс безопасности.</span><span class="sxs-lookup"><span data-stu-id="80fd5-107">It returns a singleton security resource.</span></span> <span data-ttu-id="80fd5-108">Он не содержит пригодных для использования свойств.</span><span class="sxs-lookup"><span data-stu-id="80fd5-108">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="80fd5-109">Методы</span><span class="sxs-lookup"><span data-stu-id="80fd5-109">Methods</span></span>

| <span data-ttu-id="80fd5-110">Метод</span><span class="sxs-lookup"><span data-stu-id="80fd5-110">Method</span></span>       | <span data-ttu-id="80fd5-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="80fd5-111">Return Type</span></span> | <span data-ttu-id="80fd5-112">Описание</span><span class="sxs-lookup"><span data-stu-id="80fd5-112">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="80fd5-113">[перечисление оповещений](../api/alert-list.md);</span><span class="sxs-lookup"><span data-stu-id="80fd5-113">[List alerts](../api/alert-list.md)</span></span> | <span data-ttu-id="80fd5-114">[](alert.md) коллекция Alerts</span><span class="sxs-lookup"><span data-stu-id="80fd5-114">[alert](alert.md) collection</span></span> | <span data-ttu-id="80fd5-115">Получение коллекции объектов Alert.</span><span class="sxs-lookup"><span data-stu-id="80fd5-115">Get a alert object collection.</span></span> |
| [<span data-ttu-id="80fd5-116">получение оповещений</span><span class="sxs-lookup"><span data-stu-id="80fd5-116">get alerts</span></span>](../api/alert-get.md) | <span data-ttu-id="80fd5-117">[](alert.md) коллекция Alerts</span><span class="sxs-lookup"><span data-stu-id="80fd5-117">[alert](alert.md) collection</span></span> | <span data-ttu-id="80fd5-118">Получение объекта Alert.</span><span class="sxs-lookup"><span data-stu-id="80fd5-118">Get a alert object.</span></span> |
| [<span data-ttu-id="80fd5-119">Обновление оповещений</span><span class="sxs-lookup"><span data-stu-id="80fd5-119">Update alerts</span></span>](../api/alert-update.md) | <span data-ttu-id="80fd5-120">[](alert.md) коллекция Alerts</span><span class="sxs-lookup"><span data-stu-id="80fd5-120">[alert](alert.md) collection</span></span> | <span data-ttu-id="80fd5-121">Получение объекта Alert.</span><span class="sxs-lookup"><span data-stu-id="80fd5-121">Get a alert object.</span></span> |

## <a name="properties"></a><span data-ttu-id="80fd5-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="80fd5-122">Properties</span></span>
<span data-ttu-id="80fd5-123">Нет</span><span class="sxs-lookup"><span data-stu-id="80fd5-123">None</span></span>

## <a name="relationships"></a><span data-ttu-id="80fd5-124">Связи</span><span class="sxs-lookup"><span data-stu-id="80fd5-124">Relationships</span></span>
| <span data-ttu-id="80fd5-125">Отношение</span><span class="sxs-lookup"><span data-stu-id="80fd5-125">Relationship</span></span> | <span data-ttu-id="80fd5-126">Тип</span><span class="sxs-lookup"><span data-stu-id="80fd5-126">Type</span></span>        | <span data-ttu-id="80fd5-127">Описание</span><span class="sxs-lookup"><span data-stu-id="80fd5-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="80fd5-128">alerts</span><span class="sxs-lookup"><span data-stu-id="80fd5-128">alerts</span></span>|<span data-ttu-id="80fd5-129">[](alert.md) коллекция Alerts</span><span class="sxs-lookup"><span data-stu-id="80fd5-129">[alert](alert.md) collection</span></span>| <span data-ttu-id="80fd5-p103">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="80fd5-p103">Read-only. Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="80fd5-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="80fd5-132">JSON representation</span></span>
<span data-ttu-id="80fd5-133">Ниже показано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="80fd5-133">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.security"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="80fd5-134">Пример</span><span class="sxs-lookup"><span data-stu-id="80fd5-134">Example</span></span>

<span data-ttu-id="80fd5-135">Ресурс **безопасности** доступен в корне графа.</span><span class="sxs-lookup"><span data-stu-id="80fd5-135">The **security** resource is available at the root of the graph.</span></span>

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
