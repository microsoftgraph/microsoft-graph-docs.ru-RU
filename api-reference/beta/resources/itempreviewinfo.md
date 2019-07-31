---
author: kevinlam
description: Ресурс Итемпревиевинфо содержит сведения о внедрении предварительного просмотра DriveItem.
ms.date: 3/16/2018
title: 'Итемпревиевинфо: API OneDrive'
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 2d789dacb0f1c1d3daca988f334fca2e8da4b0d5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010058"
---
# <a name="itempreviewinfo-resource-type"></a><span data-ttu-id="2b0e4-103">Тип ресурса Итемпревиевинфо</span><span class="sxs-lookup"><span data-stu-id="2b0e4-103">ItemPreviewInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b0e4-104">Ресурс **итемпревиевинфо** содержит сведения о внедрении предварительного просмотра [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="2b0e4-104">The **ItemPreviewInfo** resource contains information on how to embed a preview of a [DriveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="2b0e4-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2b0e4-105">JSON representation</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

## <a name="properties"></a><span data-ttu-id="2b0e4-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="2b0e4-106">Properties</span></span>

| <span data-ttu-id="2b0e4-107">Имя</span><span class="sxs-lookup"><span data-stu-id="2b0e4-107">Name</span></span>           | <span data-ttu-id="2b0e4-108">Тип</span><span class="sxs-lookup"><span data-stu-id="2b0e4-108">Type</span></span>   | <span data-ttu-id="2b0e4-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2b0e4-109">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="2b0e4-110">Команда</span><span class="sxs-lookup"><span data-stu-id="2b0e4-110">getUrl</span></span>         | <span data-ttu-id="2b0e4-111">string</span><span class="sxs-lookup"><span data-stu-id="2b0e4-111">string</span></span> | <span data-ttu-id="2b0e4-112">URL-адрес, подходящие для внедрения с помощью HTTP GET (Iframes и т. д.)</span><span class="sxs-lookup"><span data-stu-id="2b0e4-112">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="2b0e4-113">Постурл</span><span class="sxs-lookup"><span data-stu-id="2b0e4-113">postUrl</span></span>        | <span data-ttu-id="2b0e4-114">string</span><span class="sxs-lookup"><span data-stu-id="2b0e4-114">string</span></span> | <span data-ttu-id="2b0e4-115">URL-адрес, подходящий для внедрения с помощью HTTP POST (форма POST, JS и т. д.)</span><span class="sxs-lookup"><span data-stu-id="2b0e4-115">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="2b0e4-116">Параметры</span><span class="sxs-lookup"><span data-stu-id="2b0e4-116">postParameters</span></span> | <span data-ttu-id="2b0e4-117">string</span><span class="sxs-lookup"><span data-stu-id="2b0e4-117">string</span></span> | <span data-ttu-id="2b0e4-118">Параметры POST для включения при использовании Постурл</span><span class="sxs-lookup"><span data-stu-id="2b0e4-118">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="2b0e4-119">В зависимости от текущего состояния поддержки для заданных параметров может возвращаться либо getUrl, Постурл, либо и то, и другое.</span><span class="sxs-lookup"><span data-stu-id="2b0e4-119">Either getUrl, postUrl, or both may be returned depending on the current state of support for the specified options.</span></span>

<span data-ttu-id="2b0e4-120">i-параметры — это строка, `application/x-www-form-urlencoded`отформатированная как, и при выполнении POST для постурл Content-Type необходимо задать соответствующие параметры.</span><span class="sxs-lookup"><span data-stu-id="2b0e4-120">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="2b0e4-121">Пример:</span><span class="sxs-lookup"><span data-stu-id="2b0e4-121">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

<span data-ttu-id="2b0e4-122">Форматы URL-адресов и параметров следует считать непрозрачными.</span><span class="sxs-lookup"><span data-stu-id="2b0e4-122">The formats of URLs and parameters should be considered opaque.</span></span>
