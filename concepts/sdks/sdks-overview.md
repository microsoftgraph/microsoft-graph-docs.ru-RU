---
title: Обзор Graph SDKs
description: Описывает доступные SDKs, поддерживаемые ими платформы и их значение для разработчиков.
localization_priority: Normal
author: MichaelMainer
ms.custom: scenarios:getting-started
ms.openlocfilehash: 764bfe113c0bd66170eec1e21c2a1abddaf8b28e
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52546919"
---
# <a name="microsoft-graph-sdks-overview"></a><span data-ttu-id="f6c0a-103">Обзор Graph SDKs</span><span class="sxs-lookup"><span data-stu-id="f6c0a-103">Microsoft Graph SDKs overview</span></span>

<span data-ttu-id="f6c0a-104">SDKs Graph Microsoft предназначены для упрощения создания высококачественных, эффективных и устойчивых приложений, которые имеют доступ к microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f6c0a-104">The Microsoft Graph SDKs are designed to simplify building high-quality, efficient, and resilient applications that access Microsoft Graph.</span></span> <span data-ttu-id="f6c0a-105">SDKs включают два компонента: библиотеку служб и основную библиотеку.</span><span class="sxs-lookup"><span data-stu-id="f6c0a-105">The SDKs include two components: a service library and a core library.</span></span>

<span data-ttu-id="f6c0a-106">Библиотека служб содержит модели и конструкторы запросов, созданные из метаданных Microsoft Graph, чтобы обеспечить богатый, строго впечатаемый и обнаруживаемый опыт при работе с множеством наборов данных, доступных в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f6c0a-106">The service library contains models and request builders that are generated from Microsoft Graph metadata to provide a rich, strongly typed, and discoverable experience when working with the many datasets available in Microsoft Graph.</span></span>

<span data-ttu-id="f6c0a-107">В основной библиотеке содержится набор функций, которые улучшают работу со всеми службами Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f6c0a-107">The core library provides a set of features that enhance working with all the Microsoft Graph services.</span></span> <span data-ttu-id="f6c0a-108">Встроенная поддержка обработки повторной обработки, безопасных перенаправлений, прозрачной проверки подлинности и сжатия полезной нагрузки повышает качество взаимодействия приложения с Microsoft Graph без дополнительных сложностей, при этом вы полностью контролируете ситуацию.</span><span class="sxs-lookup"><span data-stu-id="f6c0a-108">Embedded support for retry handling, secure redirects, transparent authentication, and payload compression, improve the quality of your application's interactions with Microsoft Graph, with no added complexity, while leaving you completely in control.</span></span> <span data-ttu-id="f6c0a-109">В основной библиотеке также поддерживается выполнение общих задач, таких как прогона через коллекции и создание пакетных запросов.</span><span class="sxs-lookup"><span data-stu-id="f6c0a-109">The core library also provides support for common tasks such as paging through collections and creating batch requests.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/hDnsd2nJf88]


## <a name="supported-platforms"></a><span data-ttu-id="f6c0a-110">Поддерживаемые платформы</span><span class="sxs-lookup"><span data-stu-id="f6c0a-110">Supported platforms</span></span>

<span data-ttu-id="f6c0a-111">В настоящее время SDKs доступны для следующих языков и платформ:</span><span class="sxs-lookup"><span data-stu-id="f6c0a-111">SDKs are currently available for the following languages and platforms:</span></span>

- [<span data-ttu-id="f6c0a-112">Android</span><span class="sxs-lookup"><span data-stu-id="f6c0a-112">Android</span></span>](https://developer.microsoft.com/en-us/graph/get-started/android)
- [<span data-ttu-id="f6c0a-113">Angular</span><span class="sxs-lookup"><span data-stu-id="f6c0a-113">Angular</span></span>](https://developer.microsoft.com/en-us/graph/get-started/angular)
- [<span data-ttu-id="f6c0a-114">ASP.NET</span><span class="sxs-lookup"><span data-stu-id="f6c0a-114">ASP.NET</span></span>](https://developer.microsoft.com/en-us/graph/get-started/asp.net)
- [<span data-ttu-id="f6c0a-115">iOS</span><span class="sxs-lookup"><span data-stu-id="f6c0a-115">iOS</span></span>](https://developer.microsoft.com/en-us/graph/get-started/ios)
- [<span data-ttu-id="f6c0a-116">Javascript</span><span class="sxs-lookup"><span data-stu-id="f6c0a-116">Javascript</span></span>](https://developer.microsoft.com/en-us/graph/get-started/javascript)
- [<span data-ttu-id="f6c0a-117">Node.js</span><span class="sxs-lookup"><span data-stu-id="f6c0a-117">Node.js</span></span>](https://developer.microsoft.com/en-us/graph/get-started/node.js)
- [<span data-ttu-id="f6c0a-118">Java</span><span class="sxs-lookup"><span data-stu-id="f6c0a-118">Java</span></span>](https://developer.microsoft.com/en-us/graph/get-started/java)
- [<span data-ttu-id="f6c0a-119">PHP</span><span class="sxs-lookup"><span data-stu-id="f6c0a-119">PHP</span></span>](https://developer.microsoft.com/en-us/graph/get-started/php)
- [<span data-ttu-id="f6c0a-120">Python</span><span class="sxs-lookup"><span data-stu-id="f6c0a-120">Python</span></span>](https://developer.microsoft.com/en-us/graph/get-started/python)
- [<span data-ttu-id="f6c0a-121">Ruby</span><span class="sxs-lookup"><span data-stu-id="f6c0a-121">Ruby</span></span>](https://developer.microsoft.com/en-us/graph/get-started/ruby)

## <a name="microsoft-365-developer-subscription"></a><span data-ttu-id="f6c0a-122">Microsoft 365 подписка на разработчика</span><span class="sxs-lookup"><span data-stu-id="f6c0a-122">Microsoft 365 developer subscription</span></span>

<span data-ttu-id="f6c0a-123">При создании приложений с Graph Microsoft мы рекомендуем вам получить бесплатную подписку Microsoft 365 разработчика, подписавшись на Microsoft 365 [разработчика.](https://developer.microsoft.com/microsoft-365/dev-program)</span><span class="sxs-lookup"><span data-stu-id="f6c0a-123">When building applications using Microsoft Graph, we recommend that you get a free Microsoft 365 developer subscription by signing up for the [Microsoft 365 Developer Program](https://developer.microsoft.com/microsoft-365/dev-program).</span></span>

## <a name="see-also"></a><span data-ttu-id="f6c0a-124">См. также</span><span class="sxs-lookup"><span data-stu-id="f6c0a-124">See also</span></span>

<span data-ttu-id="f6c0a-125">Документация по [требованиям](https://github.com/microsoftgraph/msgraph-sdk-design) к проектированию SDK содержит дополнительные сведения о возможностях и возможностях SDK.</span><span class="sxs-lookup"><span data-stu-id="f6c0a-125">The SDK [design requirements documentation](https://github.com/microsoftgraph/msgraph-sdk-design) provides more details about the features and capabilities of the SDK.</span></span> <span data-ttu-id="f6c0a-126">Запрос или голосование по дополнительным функциям [на форуме идей Microsoft 365 платформы разработчиков](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph).</span><span class="sxs-lookup"><span data-stu-id="f6c0a-126">Request or vote on additional features at the [Microsoft 365 Developer Platform ideas forum](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph).</span></span> <span data-ttu-id="f6c0a-127">Список SDKs и примеров для Microsoft Graph см. на странице [microsoft Graph ресурсов.](https://developer.microsoft.com/en-us/graph/gallery/?filterBy=Samples,SDKs)</span><span class="sxs-lookup"><span data-stu-id="f6c0a-127">For a list of SDKs and samples for Microsoft Graph, see the [Microsoft Graph resources page](https://developer.microsoft.com/en-us/graph/gallery/?filterBy=Samples,SDKs).</span></span>
