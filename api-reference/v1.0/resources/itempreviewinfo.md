---
author: kevinlam
ms.author: kevinlam
ms.date: 3/16/2018
title: Итемпревиевинфо
localization_priority: Normal
description: Ресурс Итемпревиевинфо содержит сведения о внедрении предварительного просмотра driveItem.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 71d660a71bce09f198a0feb9c3acbb9a69a23a5f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036563"
---
# <a name="itempreviewinfo-resource-type"></a><span data-ttu-id="4b731-103">Тип ресурса Итемпревиевинфо</span><span class="sxs-lookup"><span data-stu-id="4b731-103">itemPreviewInfo resource type</span></span>

<span data-ttu-id="4b731-104">Ресурс **итемпревиевинфо** содержит сведения о внедрении предварительного просмотра [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="4b731-104">The **itemPreviewInfo** resource contains information on how to embed a preview of a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="4b731-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4b731-105">JSON representation</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

## <a name="properties"></a><span data-ttu-id="4b731-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="4b731-106">Properties</span></span>

| <span data-ttu-id="4b731-107">Имя</span><span class="sxs-lookup"><span data-stu-id="4b731-107">Name</span></span>           | <span data-ttu-id="4b731-108">Тип</span><span class="sxs-lookup"><span data-stu-id="4b731-108">Type</span></span>   | <span data-ttu-id="4b731-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4b731-109">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="4b731-110">Команда</span><span class="sxs-lookup"><span data-stu-id="4b731-110">getUrl</span></span>         | <span data-ttu-id="4b731-111">string</span><span class="sxs-lookup"><span data-stu-id="4b731-111">string</span></span> | <span data-ttu-id="4b731-112">URL-адрес, подходящие для внедрения с помощью HTTP GET (Iframes и т. д.)</span><span class="sxs-lookup"><span data-stu-id="4b731-112">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="4b731-113">Постурл</span><span class="sxs-lookup"><span data-stu-id="4b731-113">postUrl</span></span>        | <span data-ttu-id="4b731-114">string</span><span class="sxs-lookup"><span data-stu-id="4b731-114">string</span></span> | <span data-ttu-id="4b731-115">URL-адрес, подходящий для внедрения с помощью HTTP POST (форма POST, JS и т. д.)</span><span class="sxs-lookup"><span data-stu-id="4b731-115">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="4b731-116">Параметры</span><span class="sxs-lookup"><span data-stu-id="4b731-116">postParameters</span></span> | <span data-ttu-id="4b731-117">string</span><span class="sxs-lookup"><span data-stu-id="4b731-117">string</span></span> | <span data-ttu-id="4b731-118">Параметры POST для включения при использовании Постурл</span><span class="sxs-lookup"><span data-stu-id="4b731-118">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="4b731-119">В зависимости от текущего состояния поддержки для заданных параметров может возвращаться либо getUrl, Постурл, либо и то, и другое.</span><span class="sxs-lookup"><span data-stu-id="4b731-119">Either getUrl, postUrl, or both may be returned depending on the current state of support for the specified options.</span></span>

<span data-ttu-id="4b731-120">i-параметры — это строка, `application/x-www-form-urlencoded`отформатированная как, и при выполнении POST для постурл Content-Type необходимо задать соответствующие параметры.</span><span class="sxs-lookup"><span data-stu-id="4b731-120">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="4b731-121">Пример:</span><span class="sxs-lookup"><span data-stu-id="4b731-121">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

<span data-ttu-id="4b731-122">Форматы URL-адресов и параметров следует считать непрозрачными.</span><span class="sxs-lookup"><span data-stu-id="4b731-122">The formats of URLs and parameters should be considered opaque.</span></span>
