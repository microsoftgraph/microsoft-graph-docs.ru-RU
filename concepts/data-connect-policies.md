---
title: Политики и лицензирование подключения к данным Microsoft Graph
description: Описаны поддерживаемые политики и способ назначения номеров SKU для доступа независимых поставщиков программного обеспечения в организации.
author: fercobo-msft
localization_priority: Priority
ms.prod: data-connect
ms.openlocfilehash: b550976f6fde1af5335fb328a9aaef8f48dea33d
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629331"
---
# <a name="microsoft-graph-data-connect-policies-and-billing"></a><span data-ttu-id="c2960-103">Политики и выставление счетов для подключения к данным Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="c2960-103">Microsoft Graph Data Connect policies and billing</span></span>

<span data-ttu-id="c2960-104">Подключение к данным Microsoft Graph осуществляется с помощью [управляемых приложений Azure](/azure/managed-applications/overview). С их помощью вы можете создать и развернуть решения в среде Azure.</span><span class="sxs-lookup"><span data-stu-id="c2960-104">Microsoft Graph Data Connect uses [Azure managed applications](/azure/managed-applications/overview) to allow you to create and deploy your solutions in your Azure environment.</span></span> <span data-ttu-id="c2960-105">С помощью управляемых приложений вы можете поддерживать определенные политики Azure, обеспечивая клиентам более высокий доверительный уровень и комфортность при использовании приложений.</span><span class="sxs-lookup"><span data-stu-id="c2960-105">Managed applications allow you to support certain Azure policies, giving customers greater confidence and comfortability when using your applications.</span></span>

## <a name="policies"></a><span data-ttu-id="c2960-106">Политики</span><span class="sxs-lookup"><span data-stu-id="c2960-106">Policies</span></span>

<span data-ttu-id="c2960-107">Управляемые приложения Azure, созданные на основе данных Microsoft 365, поддерживают следующие политики Azure:</span><span class="sxs-lookup"><span data-stu-id="c2960-107">The following Azure policies are supported for an Azure managed application built using Microsoft 365 data:</span></span>

- [<span data-ttu-id="c2960-108">Служба хранилища Azure и требуемая политика ADLS 2-го поколения</span><span class="sxs-lookup"><span data-stu-id="c2960-108">Azure Storage and ADLS Gen 2 required policy</span></span>](/azure/storage/common/policy-reference)
- [<span data-ttu-id="c2960-109">Требуемая политика ADLS 1-го поколения</span><span class="sxs-lookup"><span data-stu-id="c2960-109">ADLS Gen1 required policy</span></span>](/azure/data-lake-store/policy-reference)

> [!NOTE]
> <span data-ttu-id="c2960-110">Azure Data Lake Store 1-го и 2-го поколения используют разные политики, так как ADLS 2-го поколения реализует службу хранилища Azure.</span><span class="sxs-lookup"><span data-stu-id="c2960-110">Azure Data Lake Store Gen 1 and Gen 2 use different policies because ADLS Gen 2 implements Azure Storage.</span></span>

<span data-ttu-id="c2960-111">После проверки состояния соответствия политике, выбранной во время публикации в Azure Marketplace, она применяется ко всем установленным экземплярам приложения.</span><span class="sxs-lookup"><span data-stu-id="c2960-111">When you select any of the policies during Azure marketplace publishing, the policy compliance status will be checked and enforced for all installations of your application.</span></span> <span data-ttu-id="c2960-112">Все соответствующие выбранные политики отображаются для лиц, утверждающих данные, в рамках запроса данных.</span><span class="sxs-lookup"><span data-stu-id="c2960-112">All selected policies that are compliant will be shown to the data approvers as part of the data request.</span></span> <span data-ttu-id="c2960-113">В случае нарушения соответствия политике происходит сбой в работе канала и прекращается извлечение данных.</span><span class="sxs-lookup"><span data-stu-id="c2960-113">Any policy compliance violation would cause the pipeline run to fail and stop the data extraction.</span></span>

## <a name="billing-for-microsoft-graph-data-connect"></a><span data-ttu-id="c2960-114">Выставление счетов за подключение к данным Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="c2960-114">Billing for Microsoft Graph Data Connect</span></span>

<span data-ttu-id="c2960-115">Счет будет связан с подпиской на Azure вашей Фабрики данных Azure.</span><span class="sxs-lookup"><span data-stu-id="c2960-115">The bill will be associated with the Azure Subscription of the Azure Data Factory you are using.</span></span> <span data-ttu-id="c2960-116">Цена в этой новой модели выставления счетов зависит от количества объектов Microsoft Graph, к которым вы обращаетесь.</span><span class="sxs-lookup"><span data-stu-id="c2960-116">The price in this new billing model is based on the number of Microsoft Graph objects you are accessing.</span></span>

<span data-ttu-id="c2960-117">Эта новая возможность выставления счетов доступна в предварительной версии. Ставка составляет 0,375 долл. США за 1 000 объектов Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c2960-117">While this new billing capability is in preview, the rate is $0.375 for 1,000 Microsoft Graph objects.</span></span> <span data-ttu-id="c2960-118">Например, если вы обращаетесь к 10 000 объектов, вы получите счет Azure на 3,75 долл. США.</span><span class="sxs-lookup"><span data-stu-id="c2960-118">For example, if you access 10,000 total objects, you will receive an Azure bill for $3.75.</span></span> <span data-ttu-id="c2960-119">По окончании действия предварительной версии ставка составит 0,75 долл. США за 1 000 объектов Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c2960-119">At the end of the preview period, the rate will be $0.75 per 1,000 Microsoft Graph objects.</span></span>

<span data-ttu-id="c2960-120">Объекты каталога, за которые не выставляются счета:</span><span class="sxs-lookup"><span data-stu-id="c2960-120">Directory objects that will not be charged are:</span></span>

- <span data-ttu-id="c2960-121">BasicDataSet_v0.User</span><span class="sxs-lookup"><span data-stu-id="c2960-121">BasicDataSet_v0.User</span></span>
- <span data-ttu-id="c2960-122">BasicDataSet_v0.MailboxSettings</span><span class="sxs-lookup"><span data-stu-id="c2960-122">BasicDataSet_v0.MailboxSettings</span></span>
- <span data-ttu-id="c2960-123">BasicDataSet_v0.Manager</span><span class="sxs-lookup"><span data-stu-id="c2960-123">BasicDataSet_v0.Manager</span></span>
- <span data-ttu-id="c2960-124">BasicDataSet_v0.DirectReport</span><span class="sxs-lookup"><span data-stu-id="c2960-124">BasicDataSet_v0.DirectReport</span></span>

## <a name="see-also"></a><span data-ttu-id="c2960-125">См. также</span><span class="sxs-lookup"><span data-stu-id="c2960-125">See also</span></span>

- [<span data-ttu-id="c2960-126">Политики служба хранилища Azure</span><span class="sxs-lookup"><span data-stu-id="c2960-126">Azure Storage policies</span></span>](/azure/storage/common/policy-reference)
- [<span data-ttu-id="c2960-127">Выставление счетов за подключение к данным Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="c2960-127">Microsoft Graph Data Connect billing</span></span>](https://azure.microsoft.com/pricing/details/graph-data-connect/)
- [<span data-ttu-id="c2960-128">Управляемые приложения Azure</span><span class="sxs-lookup"><span data-stu-id="c2960-128">Azure managed applications</span></span>](/azure/managed-applications/overview)
- [<span data-ttu-id="c2960-129">Выбор и фильтрация пользователей</span><span class="sxs-lookup"><span data-stu-id="c2960-129">User selection and filtering</span></span>](data-connect-filtering.md)
- [<span data-ttu-id="c2960-130">Вопросы и ответы о подключении к данным</span><span class="sxs-lookup"><span data-stu-id="c2960-130">Data Connect frequently asked questions</span></span>](data-connect-faq.md)
