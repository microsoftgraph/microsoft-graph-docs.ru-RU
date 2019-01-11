---
author: kevinlam
ms.author: kevinlam
ms.date: 3/16/2018
title: ItemPreviewInfo - OneDrive API
localization_priority: Normal
ms.openlocfilehash: 0f2a161b9b43a8d372b90530b1b9d9244f77d8e9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27857346"
---
# <a name="itempreviewinfo-resource-type"></a><span data-ttu-id="51b90-102">Тип ресурса ItemPreviewInfo</span><span class="sxs-lookup"><span data-stu-id="51b90-102">ItemPreviewInfo resource type</span></span>

> <span data-ttu-id="51b90-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="51b90-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="51b90-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51b90-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="51b90-105">Ресурс **ItemPreviewInfo** содержит сведения о том, как внедрить Предварительный просмотр [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="51b90-105">The **ItemPreviewInfo** resource contains information on how to embed a preview of a [DriveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="51b90-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="51b90-106">JSON representation</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

## <a name="properties"></a><span data-ttu-id="51b90-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="51b90-107">Properties</span></span>

| <span data-ttu-id="51b90-108">Имя</span><span class="sxs-lookup"><span data-stu-id="51b90-108">Name</span></span>           | <span data-ttu-id="51b90-109">Тип</span><span class="sxs-lookup"><span data-stu-id="51b90-109">Type</span></span>   | <span data-ttu-id="51b90-110">Описание</span><span class="sxs-lookup"><span data-stu-id="51b90-110">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="51b90-111">getUrl</span><span class="sxs-lookup"><span data-stu-id="51b90-111">getUrl</span></span>         | <span data-ttu-id="51b90-112">string</span><span class="sxs-lookup"><span data-stu-id="51b90-112">string</span></span> | <span data-ttu-id="51b90-113">URL-адрес для внедрения с помощью HTTP GET (Интернет-кадров, и т.д.)</span><span class="sxs-lookup"><span data-stu-id="51b90-113">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="51b90-114">postUrl</span><span class="sxs-lookup"><span data-stu-id="51b90-114">postUrl</span></span>        | <span data-ttu-id="51b90-115">string</span><span class="sxs-lookup"><span data-stu-id="51b90-115">string</span></span> | <span data-ttu-id="51b90-116">URL-адрес для внедрения с помощью HTTP POST (отправки формы, JS, и т.д.)</span><span class="sxs-lookup"><span data-stu-id="51b90-116">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="51b90-117">postParameters</span><span class="sxs-lookup"><span data-stu-id="51b90-117">postParameters</span></span> | <span data-ttu-id="51b90-118">string</span><span class="sxs-lookup"><span data-stu-id="51b90-118">string</span></span> | <span data-ttu-id="51b90-119">Параметры отправки для включения при использовании postUrl</span><span class="sxs-lookup"><span data-stu-id="51b90-119">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="51b90-120">В зависимости от текущего состояния поддержка указанные параметры могут быть возвращены getUrl, postUrl или оба.</span><span class="sxs-lookup"><span data-stu-id="51b90-120">Either getUrl, postUrl, or both may be returned depending on the current state of support for the specified options.</span></span>

<span data-ttu-id="51b90-121">postParameters — это строка в формате `application/x-www-form-urlencoded`, и, если для выполнения ОТПРАВКУ postUrl типа контента необходимо задать соответствующим образом.</span><span class="sxs-lookup"><span data-stu-id="51b90-121">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="51b90-122">Пример:</span><span class="sxs-lookup"><span data-stu-id="51b90-122">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

<span data-ttu-id="51b90-123">Форматы URL-адреса и параметры должны считаться непрозрачный.</span><span class="sxs-lookup"><span data-stu-id="51b90-123">The formats of URLs and parameters should be considered opaque.</span></span>
