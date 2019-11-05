---
title: Общие сведения о пакетах SDK Microsoft Graph
description: Описывает доступные пакеты SDK, Поддерживаемые платформы и значения, которые они предоставляют разработчикам.
localization_priority: Normal
author: MichaelMainer
ms.custom: scenarios:getting-started
ms.openlocfilehash: 93b2606aeb3cea9053c04d4caa87d6cf50e833e4
ms.sourcegitcommit: b1e1f614299f668453916bd85761ef7b6c8d6eff
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37969474"
---
# <a name="microsoft-graph-sdks-overview"></a><span data-ttu-id="2c4ae-103">Общие сведения о пакетах SDK Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2c4ae-103">Microsoft Graph SDKs overview</span></span>

<span data-ttu-id="2c4ae-104">Пакеты SDK Microsoft Graph предназначены для упрощения создания высококачественных, эффективных и устойчивых приложений, обращающихся к Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2c4ae-104">The Microsoft Graph SDKs are designed to simplify building high-quality, efficient, and resilient applications that access Microsoft Graph.</span></span> <span data-ttu-id="2c4ae-105">Пакеты SDK включают два компонента: библиотеку службы и основную библиотеку.</span><span class="sxs-lookup"><span data-stu-id="2c4ae-105">The SDKs include two components: a service library and a core library.</span></span>

<span data-ttu-id="2c4ae-106">Библиотека служб содержит модели и построители запросов, которые создаются из метаданных Microsoft Graph для предоставления полнофункционального, строго типизированного и обнаруживаемого интерфейса при работе с множеством наборов данных, доступных в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2c4ae-106">The service library contains models and request builders that are generated from Microsoft Graph metadata to provide a rich, strongly typed, and discoverable experience when working with the many datasets available in Microsoft Graph.</span></span>

<span data-ttu-id="2c4ae-107">Основная библиотека содержит набор функций, которые улучшают работу со всеми службами Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2c4ae-107">The core library provide a set of features that enhance working with all the Microsoft Graph services.</span></span> <span data-ttu-id="2c4ae-108">Встроенная поддержка повторных попыток обработки, безопасного перенаправления, прозрачной проверки подлинности и сжатия полезных данных, повышает качество взаимодействия приложения с Microsoft Graph, не добавляя полную сложность, в то же время не покидая все элементы управления.</span><span class="sxs-lookup"><span data-stu-id="2c4ae-108">Embedded support for retry handling, secure redirects, transparent authentication, and payload compression, improve the quality of your application's interactions with Microsoft Graph, with no added complexity, while leaving you completely in control.</span></span> <span data-ttu-id="2c4ae-109">Основная библиотека также предоставляет поддержку для распространенных задач, таких как разбиение по коллекциям и создание пакетных запросов.</span><span class="sxs-lookup"><span data-stu-id="2c4ae-109">The core library also provides support for common tasks such as paging through collections and creating batch requests.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/hDnsd2nJf88]


## <a name="supported-platforms"></a><span data-ttu-id="2c4ae-110">Поддерживаемые платформы</span><span class="sxs-lookup"><span data-stu-id="2c4ae-110">Supported platforms</span></span>

<span data-ttu-id="2c4ae-111">В настоящее время пакеты SDK доступны для следующих языков и платформ:</span><span class="sxs-lookup"><span data-stu-id="2c4ae-111">SDKs are currently available for the following languages and platforms:</span></span>

- [<span data-ttu-id="2c4ae-112">Android</span><span class="sxs-lookup"><span data-stu-id="2c4ae-112">Android</span></span>](https://developer.microsoft.com/en-us/graph/get-started/android)
- [<span data-ttu-id="2c4ae-113">Angular</span><span class="sxs-lookup"><span data-stu-id="2c4ae-113">Angular</span></span>](https://developer.microsoft.com/en-us/graph/get-started/angular)
- [<span data-ttu-id="2c4ae-114">ASP.NET</span><span class="sxs-lookup"><span data-stu-id="2c4ae-114">ASP.NET</span></span>](https://developer.microsoft.com/en-us/graph/get-started/asp.net)
- [<span data-ttu-id="2c4ae-115">iOS</span><span class="sxs-lookup"><span data-stu-id="2c4ae-115">iOS</span></span>](https://developer.microsoft.com/en-us/graph/get-started/ios)
- [<span data-ttu-id="2c4ae-116">Javascript</span><span class="sxs-lookup"><span data-stu-id="2c4ae-116">Javascript</span></span>](https://developer.microsoft.com/en-us/graph/get-started/javascript)
- [<span data-ttu-id="2c4ae-117">Node.js</span><span class="sxs-lookup"><span data-stu-id="2c4ae-117">Node.js</span></span>](https://developer.microsoft.com/en-us/graph/get-started/node.js)
- [<span data-ttu-id="2c4ae-118">Java</span><span class="sxs-lookup"><span data-stu-id="2c4ae-118">Java</span></span>](https://developer.microsoft.com/en-us/graph/get-started/java)
- [<span data-ttu-id="2c4ae-119">PHP</span><span class="sxs-lookup"><span data-stu-id="2c4ae-119">PHP</span></span>](https://developer.microsoft.com/en-us/graph/get-started/php)
- [<span data-ttu-id="2c4ae-120">Python</span><span class="sxs-lookup"><span data-stu-id="2c4ae-120">Python</span></span>](https://developer.microsoft.com/en-us/graph/get-started/python)
- [<span data-ttu-id="2c4ae-121">Ruby</span><span class="sxs-lookup"><span data-stu-id="2c4ae-121">Ruby</span></span>](https://developer.microsoft.com/en-us/graph/get-started/ruby)

## <a name="office-365-developer-subscription"></a><span data-ttu-id="2c4ae-122">Подписка на Office 365 для разработчиков</span><span class="sxs-lookup"><span data-stu-id="2c4ae-122">Office 365 developer subscription</span></span>

<span data-ttu-id="2c4ae-123">При создании приложений с помощью Microsoft Graph рекомендуется получить бесплатную подписку на Office 365 для разработчиков, зарегистрировавшись в программе для [разработчиков office 365](https://aka.ms/OfficeDevProgram).</span><span class="sxs-lookup"><span data-stu-id="2c4ae-123">When building applications using Microsoft Graph, we recommend that you get a free Office 365 developer subscription by signing up for the [Office 365 Developer Program](https://aka.ms/OfficeDevProgram).</span></span>

## <a name="see-also"></a><span data-ttu-id="2c4ae-124">См. также</span><span class="sxs-lookup"><span data-stu-id="2c4ae-124">See also</span></span>

<span data-ttu-id="2c4ae-125">[Документация по требованиям по проектированию](https://github.com/microsoftgraph/msgraph-sdk-design) SDK содержит более подробные сведения о возможностях и возможностях SDK.</span><span class="sxs-lookup"><span data-stu-id="2c4ae-125">The SDK [design requirements documentation](https://github.com/microsoftgraph/msgraph-sdk-design) provides more details about the features and capabilities of the SDK.</span></span> <span data-ttu-id="2c4ae-126">Запрос или голосование за дополнительные функции на сайте [Microsoft Graph UserVoice](https://microsoftgraph.uservoice.com) .</span><span class="sxs-lookup"><span data-stu-id="2c4ae-126">Request or vote on additional features at the [Microsoft Graph UserVoice](https://microsoftgraph.uservoice.com) site.</span></span> <span data-ttu-id="2c4ae-127">Список пакетов SDK и примеров для Microsoft Graph представлен на [странице ресурсы Microsoft Graph](https://developer.microsoft.com/en-us/graph/gallery/?filterBy=Samples,SDKs).</span><span class="sxs-lookup"><span data-stu-id="2c4ae-127">For a list of SDKs and samples for Microsoft Graph, see the [Microsoft Graph resources page](https://developer.microsoft.com/en-us/graph/gallery/?filterBy=Samples,SDKs).</span></span>
