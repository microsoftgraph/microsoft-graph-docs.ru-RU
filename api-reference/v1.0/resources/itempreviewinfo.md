---
author: kevinlam
ms.author: kevinlam
ms.date: 3/16/2018
title: итемпревиевинфо
localization_priority: Normal
description: Ресурс Итемпревиевинфо содержит сведения о внедрении предварительного просмотра driveItem.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 4d04384ba8efe27b369bfd4d73a560baf920cd53
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48009242"
---
# <a name="itempreviewinfo-resource-type"></a><span data-ttu-id="755af-103">Тип ресурса Итемпревиевинфо</span><span class="sxs-lookup"><span data-stu-id="755af-103">itemPreviewInfo resource type</span></span>

<span data-ttu-id="755af-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="755af-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="755af-105">Ресурс **итемпревиевинфо** содержит сведения о внедрении предварительного просмотра [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="755af-105">The **itemPreviewInfo** resource contains information on how to embed a preview of a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="755af-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="755af-106">JSON representation</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

## <a name="properties"></a><span data-ttu-id="755af-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="755af-107">Properties</span></span>

| <span data-ttu-id="755af-108">Имя</span><span class="sxs-lookup"><span data-stu-id="755af-108">Name</span></span>           | <span data-ttu-id="755af-109">Тип</span><span class="sxs-lookup"><span data-stu-id="755af-109">Type</span></span>   | <span data-ttu-id="755af-110">Описание</span><span class="sxs-lookup"><span data-stu-id="755af-110">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="755af-111">Команда</span><span class="sxs-lookup"><span data-stu-id="755af-111">getUrl</span></span>         | <span data-ttu-id="755af-112">string</span><span class="sxs-lookup"><span data-stu-id="755af-112">string</span></span> | <span data-ttu-id="755af-113">URL-адрес, подходящие для внедрения с помощью HTTP GET (Iframes и т. д.)</span><span class="sxs-lookup"><span data-stu-id="755af-113">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="755af-114">постурл</span><span class="sxs-lookup"><span data-stu-id="755af-114">postUrl</span></span>        | <span data-ttu-id="755af-115">string</span><span class="sxs-lookup"><span data-stu-id="755af-115">string</span></span> | <span data-ttu-id="755af-116">URL-адрес, подходящий для внедрения с помощью HTTP POST (форма POST, JS и т. д.)</span><span class="sxs-lookup"><span data-stu-id="755af-116">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="755af-117">Параметры</span><span class="sxs-lookup"><span data-stu-id="755af-117">postParameters</span></span> | <span data-ttu-id="755af-118">string</span><span class="sxs-lookup"><span data-stu-id="755af-118">string</span></span> | <span data-ttu-id="755af-119">Параметры POST для включения при использовании Постурл</span><span class="sxs-lookup"><span data-stu-id="755af-119">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="755af-120">В зависимости от текущего состояния поддержки для заданных параметров может возвращаться либо getUrl, Постурл, либо и то, и другое.</span><span class="sxs-lookup"><span data-stu-id="755af-120">Either getUrl, postUrl, or both may be returned depending on the current state of support for the specified options.</span></span>

<span data-ttu-id="755af-121">i-параметры — это строка, отформатированная как `application/x-www-form-urlencoded` , и при выполнении POST для постурл Content-Type необходимо задать соответствующие параметры.</span><span class="sxs-lookup"><span data-stu-id="755af-121">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="755af-122">Например:</span><span class="sxs-lookup"><span data-stu-id="755af-122">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

<span data-ttu-id="755af-123">Форматы URL-адресов и параметров следует считать непрозрачными.</span><span class="sxs-lookup"><span data-stu-id="755af-123">The formats of URLs and parameters should be considered opaque.</span></span>

