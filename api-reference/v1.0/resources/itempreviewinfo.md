---
author: kevinlam
ms.date: 3/16/2018
title: ItemPreviewInfo
localization_priority: Normal
description: Ресурс itemPreviewInfo содержит сведения о встраии предварительного просмотра ресурса driveItem.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: fc7ece7ed529a714b2e1262c4e39444639caced1
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50240572"
---
# <a name="itempreviewinfo-resource-type"></a><span data-ttu-id="58940-103">Тип ресурса itemPreviewInfo</span><span class="sxs-lookup"><span data-stu-id="58940-103">itemPreviewInfo resource type</span></span>

<span data-ttu-id="58940-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58940-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="58940-105">Ресурс **itemPreviewInfo содержит** сведения о том, как встраить предварительный просмотр [ресурса driveItem.](driveitem.md)</span><span class="sxs-lookup"><span data-stu-id="58940-105">The **itemPreviewInfo** resource contains information on how to embed a preview of a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="58940-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="58940-106">JSON representation</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

## <a name="properties"></a><span data-ttu-id="58940-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="58940-107">Properties</span></span>

| <span data-ttu-id="58940-108">Имя</span><span class="sxs-lookup"><span data-stu-id="58940-108">Name</span></span>           | <span data-ttu-id="58940-109">Тип</span><span class="sxs-lookup"><span data-stu-id="58940-109">Type</span></span>   | <span data-ttu-id="58940-110">Описание</span><span class="sxs-lookup"><span data-stu-id="58940-110">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="58940-111">getUrl</span><span class="sxs-lookup"><span data-stu-id="58940-111">getUrl</span></span>         | <span data-ttu-id="58940-112">string</span><span class="sxs-lookup"><span data-stu-id="58940-112">string</span></span> | <span data-ttu-id="58940-113">URL-адрес, подходящий для встраивки с помощью HTTP GET (iframes и т. д.)</span><span class="sxs-lookup"><span data-stu-id="58940-113">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="58940-114">postUrl</span><span class="sxs-lookup"><span data-stu-id="58940-114">postUrl</span></span>        | <span data-ttu-id="58940-115">string</span><span class="sxs-lookup"><span data-stu-id="58940-115">string</span></span> | <span data-ttu-id="58940-116">URL-адрес, подходящий для встраивки с помощью HTTP POST (публикация формы, JS и т. д.)</span><span class="sxs-lookup"><span data-stu-id="58940-116">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="58940-117">postParameters</span><span class="sxs-lookup"><span data-stu-id="58940-117">postParameters</span></span> | <span data-ttu-id="58940-118">string</span><span class="sxs-lookup"><span data-stu-id="58940-118">string</span></span> | <span data-ttu-id="58940-119">Параметры POST, которые необходимо включить при использовании postUrl</span><span class="sxs-lookup"><span data-stu-id="58940-119">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="58940-120">В зависимости от текущего состояния поддержки указанных параметров может быть возвращено либо getUrl, либо postUrl, либо оба этих параметра.</span><span class="sxs-lookup"><span data-stu-id="58940-120">Either getUrl, postUrl, or both may be returned depending on the current state of support for the specified options.</span></span>

<span data-ttu-id="58940-121">postParameters — это строка в формате , и если postUrl выполняет postUrl, тип контента `application/x-www-form-urlencoded` должен быть установлен соответствующим образом.</span><span class="sxs-lookup"><span data-stu-id="58940-121">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="58940-122">Например,</span><span class="sxs-lookup"><span data-stu-id="58940-122">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

<span data-ttu-id="58940-123">Форматы URL-адресов и параметров следует считать непрозрачной.</span><span class="sxs-lookup"><span data-stu-id="58940-123">The formats of URLs and parameters should be considered opaque.</span></span>

