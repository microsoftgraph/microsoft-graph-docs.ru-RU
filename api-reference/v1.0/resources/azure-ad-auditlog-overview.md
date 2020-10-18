---
title: Обзор API отчетов об активности
description: Используйте API отчетов об активности в Microsoft Graph для получения доступа к отчетам Azure Active Directory, чтобы отслеживать действия пользователей в клиенте.
localization_priority: Priority
author: khotz
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: ada166c457a5c6eb29aa7ff5dffe45491816c553
ms.sourcegitcommit: 577bfd3bb8a2e2679ef1c5942a4a496c2aa3a277
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/17/2020
ms.locfileid: "48581927"
---
# <a name="activity-reports-api-overview"></a><span data-ttu-id="db8be-103">Обзор API отчетов об активности</span><span class="sxs-lookup"><span data-stu-id="db8be-103">Activity reports API overview</span></span>

<span data-ttu-id="db8be-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db8be-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="db8be-105">Azure Active Directory (Azure AD) отслеживает действия пользователей и создает отчеты, помогающие понять, как пользователи переходят к службам Azure AD и используют их.</span><span class="sxs-lookup"><span data-stu-id="db8be-105">Azure Active Directory (Azure AD) tracks user activity and creates reports that help you understand how your users access and use Azure AD services.</span></span> <span data-ttu-id="db8be-106">Чтобы анализировать данные в этих отчетах и создавать настраиваемые решения в соответствии с конкретными требованиями организации, используйте API Microsoft Graph в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="db8be-106">Use the Microsoft Graph API for Azure AD to analyze the data in these reports and to create custom solutions tailored to your organization's specific needs.</span></span>

## <a name="what-are-azure-ad-activity-logs"></a><span data-ttu-id="db8be-107">Что такое журналы действий Azure AD?</span><span class="sxs-lookup"><span data-stu-id="db8be-107">What are Azure AD activity logs?</span></span>

<span data-ttu-id="db8be-108">Azure AD предоставляет три типа отчетов об активности:</span><span class="sxs-lookup"><span data-stu-id="db8be-108">Azure AD provides three types of activity reports:</span></span>

- <span data-ttu-id="db8be-109">журналы аудита;</span><span class="sxs-lookup"><span data-stu-id="db8be-109">audit logs</span></span>
- <span data-ttu-id="db8be-110">журналы входа.</span><span class="sxs-lookup"><span data-stu-id="db8be-110">sign-in logs</span></span>

### <a name="directory-audits"></a><span data-ttu-id="db8be-111">Аудиты каталога</span><span class="sxs-lookup"><span data-stu-id="db8be-111">Directory audits</span></span>

<span data-ttu-id="db8be-112">Отчет аудитов каталога предоставляет доступ к истории всех выполненных задач в клиенте.</span><span class="sxs-lookup"><span data-stu-id="db8be-112">The directory audit report provides you with access to the history of every task performed in your tenant.</span></span> <span data-ttu-id="db8be-113">Отчет аудитов каталога предоставляет записи о действиях системы для обеспечения соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="db8be-113">The directory audit report provides you with records of system activities for compliance.</span></span> <span data-ttu-id="db8be-114">Помимо прочего, предоставляемые данные позволяют рассматривать типичные сценарии, например:</span><span class="sxs-lookup"><span data-stu-id="db8be-114">Amongst others, the provided data enables you to address common scenarios such as:</span></span>

- <span data-ttu-id="db8be-115">Кто предоставил доступ группе администраторов к каталогу пользователя?</span><span class="sxs-lookup"><span data-stu-id="db8be-115">Who granted admin group access to a directory user?</span></span>
- <span data-ttu-id="db8be-116">Какие пользователи входят в недавно приобретенное приложение?</span><span class="sxs-lookup"><span data-stu-id="db8be-116">Which users are signing in to a recently acquired app?</span></span>
- <span data-ttu-id="db8be-117">Сколько сбросов паролей выполнено в каталоге?</span><span class="sxs-lookup"><span data-stu-id="db8be-117">How many passwords resets were made within the directory?</span></span>

### <a name="sign-ins"></a><span data-ttu-id="db8be-118">Входы</span><span class="sxs-lookup"><span data-stu-id="db8be-118">Sign-ins</span></span>

<span data-ttu-id="db8be-119">Отчет о входах помогает определить, кто выполнял задачи, указанные в отчетах аудитов каталога.</span><span class="sxs-lookup"><span data-stu-id="db8be-119">The sign-ins report helps you determine who performed the tasks reported by directory audits.</span></span> <span data-ttu-id="db8be-120">Отчет о входах помогает ответить на представленные ниже вопросы.</span><span class="sxs-lookup"><span data-stu-id="db8be-120">The sign-ins report helps you answer questions like:</span></span>

- <span data-ttu-id="db8be-121">Какой шаблон входа использует пользователь?</span><span class="sxs-lookup"><span data-stu-id="db8be-121">What is the sign in pattern of a user?</span></span>
- <span data-ttu-id="db8be-122">Сколько пользователей выполнило вход за прошлую неделю?</span><span class="sxs-lookup"><span data-stu-id="db8be-122">How many users have signed in during the last week?</span></span>
- <span data-ttu-id="db8be-123">Какое состояние у этих входов?</span><span class="sxs-lookup"><span data-stu-id="db8be-123">What's the status of these sign-ins?</span></span>

## <a name="what-can-i-do-with-audit-log-apis-in-microsoft-graph"></a><span data-ttu-id="db8be-124">Как можно использовать API журнала аудита в Microsoft Graph?</span><span class="sxs-lookup"><span data-stu-id="db8be-124">What can I do with audit log APIs in Microsoft Graph?</span></span>

<span data-ttu-id="db8be-125">Ниже приведены популярные запросы для работы с данными журнала аудита.</span><span class="sxs-lookup"><span data-stu-id="db8be-125">The following are popular requests for working with audit log data:</span></span>

<span data-ttu-id="db8be-126">Operation</span><span class="sxs-lookup"><span data-stu-id="db8be-126">Operation</span></span> | <span data-ttu-id="db8be-127">URL-адрес</span><span class="sxs-lookup"><span data-stu-id="db8be-127">URL</span></span>
:----------|:----
<span data-ttu-id="db8be-128">Получение действий пользователей клиента</span><span class="sxs-lookup"><span data-stu-id="db8be-128">GET tenant user activities</span></span> | [<span data-ttu-id="db8be-129">GET https://graph.microsoft.com/v1.0/auditLogs/directoryAudits</span><span class="sxs-lookup"><span data-stu-id="db8be-129">GET https://graph.microsoft.com/v1.0/auditLogs/directoryAudits</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/directoryAudits&version=v1.0)
<span data-ttu-id="db8be-130">Получение входов пользователей клиента</span><span class="sxs-lookup"><span data-stu-id="db8be-130">GET tenant user sign-ins</span></span> | [<span data-ttu-id="db8be-131">GET https://graph.microsoft.com/v1.0/auditLogs/signIns</span><span class="sxs-lookup"><span data-stu-id="db8be-131">GET https://graph.microsoft.com/v1.0/auditLogs/signIns</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/signIns&version=v1.0)

## <a name="what-licenses-do-i-need"></a><span data-ttu-id="db8be-132">Какие лицензии нужны?</span><span class="sxs-lookup"><span data-stu-id="db8be-132">What licenses do I need?</span></span>

<span data-ttu-id="db8be-133">Отчеты об активности доступны для компонентов, на которые у вас есть лицензии.</span><span class="sxs-lookup"><span data-stu-id="db8be-133">Activity reports are available for features that you've licensed.</span></span> <span data-ttu-id="db8be-134">Если у вас есть лицензия на определенный компонент, вам будет предоставлен доступ к соответствующим отчетам.</span><span class="sxs-lookup"><span data-stu-id="db8be-134">If you have a license for a specific feature, you also have access to the reports.</span></span>

<span data-ttu-id="db8be-135">Например, вам нужна лицензия на Azure AD Premium P1, чтобы получить доступ к отчетам аудита самостоятельного изменения паролей.</span><span class="sxs-lookup"><span data-stu-id="db8be-135">For example, you need an Azure AD Premium P1 license to access self-service password audit reports.</span></span>  <span data-ttu-id="db8be-136">Дополнительные сведения см. на странице [лицензий Azure AD](https://azure.microsoft.com/pricing/details/active-directory/).</span><span class="sxs-lookup"><span data-stu-id="db8be-136">To learn more, see [Azure AD licensing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

<span data-ttu-id="db8be-137">Для отчетов входов требуется лицензия на Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="db8be-137">Sign-in reports require an Azure AD Premium license.</span></span>

<span data-ttu-id="db8be-138">Дополнительные сведения см. на странице [Цены на Azure AD](https://azure.microsoft.com/pricing/details/active-directory/).</span><span class="sxs-lookup"><span data-stu-id="db8be-138">To learn more, see [Azure AD pricing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

## <a name="next-steps"></a><span data-ttu-id="db8be-139">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="db8be-139">Next Steps</span></span>

- <span data-ttu-id="db8be-140">[Зарегистрируйте приложение](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal), чтобы соответствовать предварительным требованиям отчетов.</span><span class="sxs-lookup"><span data-stu-id="db8be-140">[Register your app](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to satisfy report prerequisites.</span></span> 
- <span data-ttu-id="db8be-141">Ознакомьтесь с примерами журналов [аудита](/azure/active-directory/active-directory-reporting-api-audit-samples) и [входа](/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples).</span><span class="sxs-lookup"><span data-stu-id="db8be-141">Learn from [audit log](/azure/active-directory/active-directory-reporting-api-audit-samples) and [sign-in samples](/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples).</span></span>  
- <span data-ttu-id="db8be-142">Изучите действия и ресурс [directoryAudit](directoryaudit.md).</span><span class="sxs-lookup"><span data-stu-id="db8be-142">Review [directoryAudit](directoryaudit.md) resource and actions.</span></span>
- <span data-ttu-id="db8be-143">Изучите действия и ресурс [signIn](signin.md).</span><span class="sxs-lookup"><span data-stu-id="db8be-143">Review [signIn](signin.md) resource and actions.</span></span> 
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/azure-ad-auditlog-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->