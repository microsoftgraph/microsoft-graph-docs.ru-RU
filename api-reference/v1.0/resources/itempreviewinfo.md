---
author: kevinlam
ms.author: kevinlam
ms.date: 3/16/2018
title: ItemPreviewInfo
ms.openlocfilehash: 8b8f7a962e237cc20a42503efd31f083996ad715
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026840"
---
# <a name="itempreviewinfo-resource-type"></a><span data-ttu-id="b306f-102">Тип ресурса itemPreviewInfo</span><span class="sxs-lookup"><span data-stu-id="b306f-102">itemPreviewInfo resource type</span></span>

<span data-ttu-id="b306f-103">Ресурс **itemPreviewInfo** содержит сведения о том, как внедрить Предварительный просмотр [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="b306f-103">The **itemPreviewInfo** resource contains information on how to embed a preview of a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="b306f-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b306f-104">JSON representation</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

## <a name="properties"></a><span data-ttu-id="b306f-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="b306f-105">Properties</span></span>

| <span data-ttu-id="b306f-106">Имя</span><span class="sxs-lookup"><span data-stu-id="b306f-106">Name</span></span>           | <span data-ttu-id="b306f-107">Тип</span><span class="sxs-lookup"><span data-stu-id="b306f-107">Type</span></span>   | <span data-ttu-id="b306f-108">Description</span><span class="sxs-lookup"><span data-stu-id="b306f-108">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="b306f-109">getUrl</span><span class="sxs-lookup"><span data-stu-id="b306f-109">getUrl</span></span>         | <span data-ttu-id="b306f-110">string</span><span class="sxs-lookup"><span data-stu-id="b306f-110">string</span></span> | <span data-ttu-id="b306f-111">URL-адрес для внедрения с помощью HTTP GET (Интернет-кадров, и т.д.)</span><span class="sxs-lookup"><span data-stu-id="b306f-111">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="b306f-112">postUrl</span><span class="sxs-lookup"><span data-stu-id="b306f-112">postUrl</span></span>        | <span data-ttu-id="b306f-113">string</span><span class="sxs-lookup"><span data-stu-id="b306f-113">string</span></span> | <span data-ttu-id="b306f-114">URL-адрес для внедрения с помощью HTTP POST (отправки формы, JS, и т.д.)</span><span class="sxs-lookup"><span data-stu-id="b306f-114">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="b306f-115">postParameters</span><span class="sxs-lookup"><span data-stu-id="b306f-115">postParameters</span></span> | <span data-ttu-id="b306f-116">string</span><span class="sxs-lookup"><span data-stu-id="b306f-116">string</span></span> | <span data-ttu-id="b306f-117">Параметры отправки для включения при использовании postUrl</span><span class="sxs-lookup"><span data-stu-id="b306f-117">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="b306f-118">В зависимости от текущего состояния поддержка указанные параметры могут быть возвращены getUrl, postUrl или оба.</span><span class="sxs-lookup"><span data-stu-id="b306f-118">Either getUrl, postUrl, or both may be returned depending on the current state of support for the specified options.</span></span>

<span data-ttu-id="b306f-119">postParameters — это строка в формате `application/x-www-form-urlencoded`, и, если для выполнения ОТПРАВКУ postUrl типа контента необходимо задать соответствующим образом.</span><span class="sxs-lookup"><span data-stu-id="b306f-119">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="b306f-120">Пример:</span><span class="sxs-lookup"><span data-stu-id="b306f-120">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

<span data-ttu-id="b306f-121">Форматы URL-адреса и параметры должны считаться непрозрачный.</span><span class="sxs-lookup"><span data-stu-id="b306f-121">The formats of URLs and parameters should be considered opaque.</span></span>
