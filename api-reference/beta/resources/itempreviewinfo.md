---
author: kevinlam
description: Ресурс Итемпревиевинфо содержит сведения о внедрении предварительного просмотра DriveItem.
ms.date: 3/16/2018
title: 'Итемпревиевинфо: API OneDrive'
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: ab62e2a41d257adcb8f763b77e42f0d7e515ee5b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033701"
---
# <a name="itempreviewinfo-resource-type"></a><span data-ttu-id="67a51-103">Тип ресурса Итемпревиевинфо</span><span class="sxs-lookup"><span data-stu-id="67a51-103">ItemPreviewInfo resource type</span></span>

<span data-ttu-id="67a51-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67a51-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67a51-105">Ресурс **итемпревиевинфо** содержит сведения о внедрении предварительного просмотра [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="67a51-105">The **ItemPreviewInfo** resource contains information on how to embed a preview of a [DriveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="67a51-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="67a51-106">JSON representation</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

## <a name="properties"></a><span data-ttu-id="67a51-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="67a51-107">Properties</span></span>

| <span data-ttu-id="67a51-108">Имя</span><span class="sxs-lookup"><span data-stu-id="67a51-108">Name</span></span>           | <span data-ttu-id="67a51-109">Тип</span><span class="sxs-lookup"><span data-stu-id="67a51-109">Type</span></span>   | <span data-ttu-id="67a51-110">Описание</span><span class="sxs-lookup"><span data-stu-id="67a51-110">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="67a51-111">Команда</span><span class="sxs-lookup"><span data-stu-id="67a51-111">getUrl</span></span>         | <span data-ttu-id="67a51-112">string</span><span class="sxs-lookup"><span data-stu-id="67a51-112">string</span></span> | <span data-ttu-id="67a51-113">URL-адрес, подходящие для внедрения с помощью HTTP GET (Iframes и т. д.)</span><span class="sxs-lookup"><span data-stu-id="67a51-113">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="67a51-114">постурл</span><span class="sxs-lookup"><span data-stu-id="67a51-114">postUrl</span></span>        | <span data-ttu-id="67a51-115">string</span><span class="sxs-lookup"><span data-stu-id="67a51-115">string</span></span> | <span data-ttu-id="67a51-116">URL-адрес, подходящий для внедрения с помощью HTTP POST (форма POST, JS и т. д.)</span><span class="sxs-lookup"><span data-stu-id="67a51-116">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="67a51-117">Параметры</span><span class="sxs-lookup"><span data-stu-id="67a51-117">postParameters</span></span> | <span data-ttu-id="67a51-118">string</span><span class="sxs-lookup"><span data-stu-id="67a51-118">string</span></span> | <span data-ttu-id="67a51-119">Параметры POST для включения при использовании Постурл</span><span class="sxs-lookup"><span data-stu-id="67a51-119">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="67a51-120">В зависимости от текущего состояния поддержки для заданных параметров может возвращаться либо getUrl, Постурл, либо и то, и другое.</span><span class="sxs-lookup"><span data-stu-id="67a51-120">Either getUrl, postUrl, or both may be returned depending on the current state of support for the specified options.</span></span>

<span data-ttu-id="67a51-121">i-параметры — это строка, отформатированная как `application/x-www-form-urlencoded` , и при выполнении POST для постурл Content-Type необходимо задать соответствующие параметры.</span><span class="sxs-lookup"><span data-stu-id="67a51-121">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="67a51-122">Например:</span><span class="sxs-lookup"><span data-stu-id="67a51-122">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

<span data-ttu-id="67a51-123">Форматы URL-адресов и параметров следует считать непрозрачными.</span><span class="sxs-lookup"><span data-stu-id="67a51-123">The formats of URLs and parameters should be considered opaque.</span></span>


