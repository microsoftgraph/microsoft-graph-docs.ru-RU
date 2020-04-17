---
title: Изучение использования приложений API Azure AD Graph
description: Сведения о том, как выполнять аудит API Azure Active Directory (Azure AD) для переноса приложения в API Microsoft Graph.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 14cc61039d97fa43f64599310cf86cce6c348fb2
ms.sourcegitcommit: ca55fc5f5711966eaa41da31cd1ae99820e9e586
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2019
ms.locfileid: "35645250"
---
# <a name="examine-azure-ad-graph-apis-app-usage"></a><span data-ttu-id="71714-103">Изучение использования приложений API Azure AD Graph</span><span class="sxs-lookup"><span data-stu-id="71714-103">Examine Azure AD Graph APIs app usage</span></span>

<span data-ttu-id="71714-104">Это шаг 2 [процесса переноса приложений](migrate-azure-ad-graph-planning-checklist.md).</span><span class="sxs-lookup"><span data-stu-id="71714-104">This is step 2 of the [process to migrate apps](migrate-azure-ad-graph-planning-checklist.md).</span></span>

<span data-ttu-id="71714-105">При планировании миграции в Microsoft Graph необходимо проанализировать существующее приложение и каталогизировать используемые API Graph Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="71714-105">While planning your migration to Microsoft Graph, take time to review your existing application and to catalog the Azure AD Graph APIs you're currently using.</span></span>

<span data-ttu-id="71714-106">Сравните список с известными отличиями.</span><span class="sxs-lookup"><span data-stu-id="71714-106">Compare your list to the known differences.</span></span>  <span data-ttu-id="71714-107">Это помогает определить конкретные изменения, которые необходимо выполнить для переноса приложения.</span><span class="sxs-lookup"><span data-stu-id="71714-107">This helps identify specific changes you'll need to make to migrate your app.</span></span>  <span data-ttu-id="71714-108">К ним относятся простые изменения, которые легко разрешить с помощью функций поиска и замены в редакторе или более сложных обновлений, которые могут потребовать большего анализа.</span><span class="sxs-lookup"><span data-stu-id="71714-108">These include simple changes easily resolved using an editor's search-and-replace features or more complicated updates that might require more analysis.</span></span>

<span data-ttu-id="71714-109">Microsoft Graph поддерживает многие функции и возможности Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="71714-109">Microsoft Graph supports many of the same features and capabilities of Azure AD graph.</span></span>  <span data-ttu-id="71714-110">Существует несколько ключевых отличий.</span><span class="sxs-lookup"><span data-stu-id="71714-110">There are a few key differences:</span></span>

- [<span data-ttu-id="71714-111">Различия в запросах</span><span class="sxs-lookup"><span data-stu-id="71714-111">Request differences</span></span>](migrate-azure-ad-graph-request-differences.md)
- [<span data-ttu-id="71714-112">Функциональные различия</span><span class="sxs-lookup"><span data-stu-id="71714-112">Feature differences</span></span>](migrate-azure-ad-graph-feature-differences.md)
- [<span data-ttu-id="71714-113">Различия между типами ресурсов</span><span class="sxs-lookup"><span data-stu-id="71714-113">Resource type differences</span></span>](migrate-azure-ad-graph-resource-differences.md)
- [<span data-ttu-id="71714-114">Различия свойств</span><span class="sxs-lookup"><span data-stu-id="71714-114">Property differences</span></span>](migrate-azure-ad-graph-property-differences.md)
- [<span data-ttu-id="71714-115">Различия в методах</span><span class="sxs-lookup"><span data-stu-id="71714-115">Method differences</span></span>](migrate-azure-ad-graph-method-differences.md)

<span data-ttu-id="71714-116">Кроме того, необходимо проверить разрешения, необходимые для функций, которые использует ваше приложение.</span><span class="sxs-lookup"><span data-stu-id="71714-116">You'll also want to verify the permissions required for the features your app is using.</span></span>  <span data-ttu-id="71714-117">В некоторых случаях доступны более детализированные разрешения.</span><span class="sxs-lookup"><span data-stu-id="71714-117">In some cases, more granular permissions are available.</span></span>

<span data-ttu-id="71714-118">Дополнительные сведения см. в статье [Разрешения](permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="71714-118">To learn more, see [Permissions](permissions-reference.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="71714-119">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="71714-119">Next Steps</span></span>

- <span data-ttu-id="71714-120">Сведения о [регистрации приложений, разрешениях и различиях](migrate-azure-ad-graph-app-registration.md) между Azure AD Graph и Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="71714-120">Learn about [app registration, permissions and consent differences](migrate-azure-ad-graph-app-registration.md) between Azure AD Graph and Microsoft Graph.</span></span>
- <span data-ttu-id="71714-121">Ознакомьтесь с основными понятиями и рекомендациями [Microsoft Graph](/graph/overview) .</span><span class="sxs-lookup"><span data-stu-id="71714-121">Explore [Microsoft Graph](/graph/overview) concepts and practices.</span></span>
- <span data-ttu-id="71714-122">Поэкспериментируйте с Microsoft Graph с помощью [проводника диаграмм](https://aka.ms/ge) .</span><span class="sxs-lookup"><span data-stu-id="71714-122">Use [Graph Explorer](https://aka.ms/ge) to experiment with Microsoft Graph.</span></span>
