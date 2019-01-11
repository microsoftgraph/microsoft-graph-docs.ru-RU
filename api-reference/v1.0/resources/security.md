---
title: Тип ресурса безопасности
description: Безопасность ресурсов — это точка входа для объектной модели безопасности. Возвращает ресурсов безопасности одного. Он не содержит какие-либо можно использовать свойства.
localization_priority: Normal
ms.openlocfilehash: 2486bf9cae2ffad471c1bacb8b7ca01c6bef4ee7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27827015"
---
# <a name="security-resource-type"></a><span data-ttu-id="3ce77-105">Тип ресурса безопасности</span><span class="sxs-lookup"><span data-stu-id="3ce77-105">security resource type</span></span>

<span data-ttu-id="3ce77-106">Безопасность ресурсов — это точка входа для объектной модели безопасности.</span><span class="sxs-lookup"><span data-stu-id="3ce77-106">The security resource is the entry point for the Security object model.</span></span> <span data-ttu-id="3ce77-107">Возвращает ресурсов безопасности одного.</span><span class="sxs-lookup"><span data-stu-id="3ce77-107">It returns a singleton security resource.</span></span> <span data-ttu-id="3ce77-108">Он не содержит какие-либо можно использовать свойства.</span><span class="sxs-lookup"><span data-stu-id="3ce77-108">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="3ce77-109">Методы</span><span class="sxs-lookup"><span data-stu-id="3ce77-109">Methods</span></span>

| <span data-ttu-id="3ce77-110">Метод</span><span class="sxs-lookup"><span data-stu-id="3ce77-110">Method</span></span>       | <span data-ttu-id="3ce77-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3ce77-111">Return Type</span></span> | <span data-ttu-id="3ce77-112">Описание</span><span class="sxs-lookup"><span data-stu-id="3ce77-112">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="3ce77-113">[перечисление оповещений](../api/alert-list.md);</span><span class="sxs-lookup"><span data-stu-id="3ce77-113">[List alerts](../api/alert-list.md)</span></span> | <span data-ttu-id="3ce77-114">[оповещение о](alert.md) семейства сайтов</span><span class="sxs-lookup"><span data-stu-id="3ce77-114">[alert](alert.md) collection</span></span> | <span data-ttu-id="3ce77-115">Получите коллекцию объекта оповещения.</span><span class="sxs-lookup"><span data-stu-id="3ce77-115">Get a alert object collection.</span></span> |
| [<span data-ttu-id="3ce77-116">Получение оповещений</span><span class="sxs-lookup"><span data-stu-id="3ce77-116">get alerts</span></span>](../api/alert-get.md) | <span data-ttu-id="3ce77-117">[оповещение о](alert.md) семейства сайтов</span><span class="sxs-lookup"><span data-stu-id="3ce77-117">[alert](alert.md) collection</span></span> | <span data-ttu-id="3ce77-118">Получите объект оповещения.</span><span class="sxs-lookup"><span data-stu-id="3ce77-118">Get a alert object.</span></span> |
| [<span data-ttu-id="3ce77-119">Обновление оповещений</span><span class="sxs-lookup"><span data-stu-id="3ce77-119">Update alerts</span></span>](../api/alert-update.md) | <span data-ttu-id="3ce77-120">[оповещение о](alert.md) семейства сайтов</span><span class="sxs-lookup"><span data-stu-id="3ce77-120">[alert](alert.md) collection</span></span> | <span data-ttu-id="3ce77-121">Получите объект оповещения.</span><span class="sxs-lookup"><span data-stu-id="3ce77-121">Get a alert object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3ce77-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="3ce77-122">Properties</span></span>
<span data-ttu-id="3ce77-123">Нет</span><span class="sxs-lookup"><span data-stu-id="3ce77-123">None</span></span>

## <a name="relationships"></a><span data-ttu-id="3ce77-124">Связи</span><span class="sxs-lookup"><span data-stu-id="3ce77-124">Relationships</span></span>
| <span data-ttu-id="3ce77-125">Связь</span><span class="sxs-lookup"><span data-stu-id="3ce77-125">Relationship</span></span> | <span data-ttu-id="3ce77-126">Тип</span><span class="sxs-lookup"><span data-stu-id="3ce77-126">Type</span></span>        | <span data-ttu-id="3ce77-127">Описание</span><span class="sxs-lookup"><span data-stu-id="3ce77-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3ce77-128">alerts</span><span class="sxs-lookup"><span data-stu-id="3ce77-128">alerts</span></span>|<span data-ttu-id="3ce77-129">[оповещение о](alert.md) семейства сайтов</span><span class="sxs-lookup"><span data-stu-id="3ce77-129">[alert](alert.md) collection</span></span>| <span data-ttu-id="3ce77-p103">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="3ce77-p103">Read-only. Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="3ce77-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3ce77-132">JSON representation</span></span>
<span data-ttu-id="3ce77-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3ce77-133">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.security"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="3ce77-134">Пример</span><span class="sxs-lookup"><span data-stu-id="3ce77-134">Example</span></span>

<span data-ttu-id="3ce77-135">**Безопасность** ресурсов доступна в корне диаграммы.</span><span class="sxs-lookup"><span data-stu-id="3ce77-135">The **security** resource is available at the root of the graph.</span></span>

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
