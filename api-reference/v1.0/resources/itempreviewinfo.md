---
author: kevinlam
ms.author: kevinlam
ms.date: 3/16/2018
title: Итемпревиевинфо
localization_priority: Normal
ms.openlocfilehash: e7df636f9c406a499baa5ef3be1748273920cac4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32585239"
---
# <a name="itempreviewinfo-resource-type"></a><span data-ttu-id="f3315-102">Тип ресурса Итемпревиевинфо</span><span class="sxs-lookup"><span data-stu-id="f3315-102">itemPreviewInfo resource type</span></span>

<span data-ttu-id="f3315-103">Ресурс **итемпревиевинфо** содержит сведения о внедрении предварительного просмотра [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="f3315-103">The **itemPreviewInfo** resource contains information on how to embed a preview of a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="f3315-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f3315-104">JSON representation</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

## <a name="properties"></a><span data-ttu-id="f3315-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="f3315-105">Properties</span></span>

| <span data-ttu-id="f3315-106">Имя</span><span class="sxs-lookup"><span data-stu-id="f3315-106">Name</span></span>           | <span data-ttu-id="f3315-107">Тип</span><span class="sxs-lookup"><span data-stu-id="f3315-107">Type</span></span>   | <span data-ttu-id="f3315-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f3315-108">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="f3315-109">Команда</span><span class="sxs-lookup"><span data-stu-id="f3315-109">getUrl</span></span>         | <span data-ttu-id="f3315-110">строка</span><span class="sxs-lookup"><span data-stu-id="f3315-110">string</span></span> | <span data-ttu-id="f3315-111">URL-адрес, подходящие для внедрения с помощью HTTP GET (Iframes и т. д.)</span><span class="sxs-lookup"><span data-stu-id="f3315-111">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="f3315-112">Постурл</span><span class="sxs-lookup"><span data-stu-id="f3315-112">postUrl</span></span>        | <span data-ttu-id="f3315-113">строка</span><span class="sxs-lookup"><span data-stu-id="f3315-113">string</span></span> | <span data-ttu-id="f3315-114">URL-адрес, подходящий для внедрения с помощью HTTP POST (форма POST, JS и т. д.)</span><span class="sxs-lookup"><span data-stu-id="f3315-114">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="f3315-115">Параметры</span><span class="sxs-lookup"><span data-stu-id="f3315-115">postParameters</span></span> | <span data-ttu-id="f3315-116">строка</span><span class="sxs-lookup"><span data-stu-id="f3315-116">string</span></span> | <span data-ttu-id="f3315-117">Параметры POST для включения при использовании Постурл</span><span class="sxs-lookup"><span data-stu-id="f3315-117">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="f3315-118">В зависимости от текущего состояния поддержки для заданных параметров может возвращаться либо getUrl, Постурл, либо и то, и другое.</span><span class="sxs-lookup"><span data-stu-id="f3315-118">Either getUrl, postUrl, or both may be returned depending on the current state of support for the specified options.</span></span>

<span data-ttu-id="f3315-119">i-параметры — это строка, `application/x-www-form-urlencoded`отформатированная как, и при выполнении POST для постурл Content-Type необходимо задать соответствующие параметры.</span><span class="sxs-lookup"><span data-stu-id="f3315-119">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="f3315-120">Пример:</span><span class="sxs-lookup"><span data-stu-id="f3315-120">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

<span data-ttu-id="f3315-121">Форматы URL-адресов и параметров следует считать непрозрачными.</span><span class="sxs-lookup"><span data-stu-id="f3315-121">The formats of URLs and parameters should be considered opaque.</span></span>
