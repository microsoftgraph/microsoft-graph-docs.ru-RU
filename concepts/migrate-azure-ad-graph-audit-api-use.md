---
title: Изучение использования приложений API Azure AD Graph
description: Описывает, как аудит API Azure Active Directory (Azure AD) для переноса приложения в API Microsoft Graph.
author: dkershaw10
localization_priority: Normal
ms.prod: applications
ms.openlocfilehash: e7e21f03cdfd8ce3d45f0201d15ec489c7322530
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760695"
---
# <a name="examine-azure-ad-graph-apis-app-usage"></a><span data-ttu-id="24382-103">Изучение использования приложений API Azure AD Graph</span><span class="sxs-lookup"><span data-stu-id="24382-103">Examine Azure AD Graph APIs app usage</span></span>

<span data-ttu-id="24382-104">Это шаг 2 процесса [миграции приложений.](migrate-azure-ad-graph-planning-checklist.md)</span><span class="sxs-lookup"><span data-stu-id="24382-104">This is step 2 of the [process to migrate apps](migrate-azure-ad-graph-planning-checklist.md).</span></span>

<span data-ttu-id="24382-105">При планировании переноса в Microsoft Graph необходимо время, чтобы просмотреть существующее приложение и каталогизировать API Azure AD Graph, которые вы используете в настоящее время.</span><span class="sxs-lookup"><span data-stu-id="24382-105">While planning your migration to Microsoft Graph, take time to review your existing application and to catalog the Azure AD Graph APIs you're currently using.</span></span>

<span data-ttu-id="24382-106">Сравните список с известными различиями.</span><span class="sxs-lookup"><span data-stu-id="24382-106">Compare your list to the known differences.</span></span>  <span data-ttu-id="24382-107">Это помогает определить конкретные изменения, которые необходимо внести для переноса приложения.</span><span class="sxs-lookup"><span data-stu-id="24382-107">This helps identify specific changes you'll need to make to migrate your app.</span></span>  <span data-ttu-id="24382-108">К ним относятся простые изменения, которые легко разрешить с помощью функций поиска и замены редактора или более сложные обновления, которые могут потребовать дополнительного анализа.</span><span class="sxs-lookup"><span data-stu-id="24382-108">These include simple changes easily resolved using an editor's search-and-replace features or more complicated updates that might require more analysis.</span></span>

<span data-ttu-id="24382-109">Microsoft Graph поддерживает многие из тех же функций и возможностей диаграммы Azure AD.</span><span class="sxs-lookup"><span data-stu-id="24382-109">Microsoft Graph supports many of the same features and capabilities of Azure AD graph.</span></span>  <span data-ttu-id="24382-110">Существует несколько ключевых отличий:</span><span class="sxs-lookup"><span data-stu-id="24382-110">There are a few key differences:</span></span>

- [<span data-ttu-id="24382-111">Различия запросов</span><span class="sxs-lookup"><span data-stu-id="24382-111">Request differences</span></span>](migrate-azure-ad-graph-request-differences.md)
- [<span data-ttu-id="24382-112">Функциональные различия</span><span class="sxs-lookup"><span data-stu-id="24382-112">Feature differences</span></span>](migrate-azure-ad-graph-feature-differences.md)
- [<span data-ttu-id="24382-113">Различия в типах ресурсов</span><span class="sxs-lookup"><span data-stu-id="24382-113">Resource type differences</span></span>](migrate-azure-ad-graph-resource-differences.md)
- [<span data-ttu-id="24382-114">Различия свойств</span><span class="sxs-lookup"><span data-stu-id="24382-114">Property differences</span></span>](migrate-azure-ad-graph-property-differences.md)
- [<span data-ttu-id="24382-115">Различия метода</span><span class="sxs-lookup"><span data-stu-id="24382-115">Method differences</span></span>](migrate-azure-ad-graph-method-differences.md)

<span data-ttu-id="24382-116">Кроме того, необходимо проверить разрешения, необходимые для функций, которые использует приложение.</span><span class="sxs-lookup"><span data-stu-id="24382-116">You'll also want to verify the permissions required for the features your app is using.</span></span>  <span data-ttu-id="24382-117">В некоторых случаях доступны дополнительные разрешения на детализацию.</span><span class="sxs-lookup"><span data-stu-id="24382-117">In some cases, more granular permissions are available.</span></span>

<span data-ttu-id="24382-118">Дополнительные сведения см. в статье [Разрешения](permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="24382-118">To learn more, see [Permissions](permissions-reference.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="24382-119">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="24382-119">Next Steps</span></span>

- <span data-ttu-id="24382-120">Узнайте о различиях в регистрации [приложений, разрешениях](migrate-azure-ad-graph-app-registration.md) и согласии между Azure AD Graph и Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="24382-120">Learn about [app registration, permissions and consent differences](migrate-azure-ad-graph-app-registration.md) between Azure AD Graph and Microsoft Graph.</span></span>
- <span data-ttu-id="24382-121">Снова [просмотрите контрольный](migrate-azure-ad-graph-planning-checklist.md) список.</span><span class="sxs-lookup"><span data-stu-id="24382-121">Review the [checklist](migrate-azure-ad-graph-planning-checklist.md) again.</span></span>

