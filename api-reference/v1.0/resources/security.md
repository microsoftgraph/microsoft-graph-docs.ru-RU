---
title: тип ресурсов безопасности
description: Ресурс безопасности является точкой входа для объектной модели безопасности. Он возвращает ресурс безопасности singleton. Он не содержит никаких полезных свойств.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 345e3e81b86fe42d16f4110450120c9f225c22dd
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473667"
---
# <a name="security-resource-type"></a><span data-ttu-id="34b51-105">тип ресурсов безопасности</span><span class="sxs-lookup"><span data-stu-id="34b51-105">security resource type</span></span>

<span data-ttu-id="34b51-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34b51-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="34b51-107">Ресурс безопасности является точкой входа для объектной модели безопасности.</span><span class="sxs-lookup"><span data-stu-id="34b51-107">The security resource is the entry point for the Security object model.</span></span> <span data-ttu-id="34b51-108">Он возвращает ресурс безопасности singleton.</span><span class="sxs-lookup"><span data-stu-id="34b51-108">It returns a singleton security resource.</span></span> <span data-ttu-id="34b51-109">Он не содержит никаких полезных свойств.</span><span class="sxs-lookup"><span data-stu-id="34b51-109">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="34b51-110">Методы</span><span class="sxs-lookup"><span data-stu-id="34b51-110">Methods</span></span>

| <span data-ttu-id="34b51-111">Метод</span><span class="sxs-lookup"><span data-stu-id="34b51-111">Method</span></span>       | <span data-ttu-id="34b51-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="34b51-112">Return Type</span></span> | <span data-ttu-id="34b51-113">Описание</span><span class="sxs-lookup"><span data-stu-id="34b51-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="34b51-114">Перечисление оповещений</span><span class="sxs-lookup"><span data-stu-id="34b51-114">List alerts</span></span>](../api/alert-list.md) | <span data-ttu-id="34b51-115">Коллекция [alert](alert.md)</span><span class="sxs-lookup"><span data-stu-id="34b51-115">[alert](alert.md) collection</span></span> | <span data-ttu-id="34b51-116">Получите коллекцию объектов оповещения.</span><span class="sxs-lookup"><span data-stu-id="34b51-116">Get a alert object collection.</span></span> |
| [<span data-ttu-id="34b51-117">получения оповещений</span><span class="sxs-lookup"><span data-stu-id="34b51-117">get alerts</span></span>](../api/alert-get.md) | <span data-ttu-id="34b51-118">Коллекция [alert](alert.md)</span><span class="sxs-lookup"><span data-stu-id="34b51-118">[alert](alert.md) collection</span></span> | <span data-ttu-id="34b51-119">Получите объект оповещений.</span><span class="sxs-lookup"><span data-stu-id="34b51-119">Get a alert object.</span></span> |
| [<span data-ttu-id="34b51-120">Обновление оповещений</span><span class="sxs-lookup"><span data-stu-id="34b51-120">Update alerts</span></span>](../api/alert-update.md) | <span data-ttu-id="34b51-121">Коллекция [alert](alert.md)</span><span class="sxs-lookup"><span data-stu-id="34b51-121">[alert](alert.md) collection</span></span> | <span data-ttu-id="34b51-122">Получите объект оповещений.</span><span class="sxs-lookup"><span data-stu-id="34b51-122">Get a alert object.</span></span> |

## <a name="properties"></a><span data-ttu-id="34b51-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="34b51-123">Properties</span></span>
<span data-ttu-id="34b51-124">Нет</span><span class="sxs-lookup"><span data-stu-id="34b51-124">None</span></span>

## <a name="relationships"></a><span data-ttu-id="34b51-125">Связи</span><span class="sxs-lookup"><span data-stu-id="34b51-125">Relationships</span></span>
| <span data-ttu-id="34b51-126">Связь</span><span class="sxs-lookup"><span data-stu-id="34b51-126">Relationship</span></span> | <span data-ttu-id="34b51-127">Тип</span><span class="sxs-lookup"><span data-stu-id="34b51-127">Type</span></span>        | <span data-ttu-id="34b51-128">Описание</span><span class="sxs-lookup"><span data-stu-id="34b51-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="34b51-129">alerts</span><span class="sxs-lookup"><span data-stu-id="34b51-129">alerts</span></span>|<span data-ttu-id="34b51-130">Коллекция [alert](alert.md)</span><span class="sxs-lookup"><span data-stu-id="34b51-130">[alert](alert.md) collection</span></span>| <span data-ttu-id="34b51-p103">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="34b51-p103">Read-only. Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="34b51-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="34b51-133">JSON representation</span></span>
<span data-ttu-id="34b51-134">Ниже показано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="34b51-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.security"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="34b51-135">Пример</span><span class="sxs-lookup"><span data-stu-id="34b51-135">Example</span></span>

<span data-ttu-id="34b51-136">Ресурс **безопасности** доступен в корне графа.</span><span class="sxs-lookup"><span data-stu-id="34b51-136">The **security** resource is available at the root of the graph.</span></span>

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
```http
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

