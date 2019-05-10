---
title: Обзор API журнала аудита Azure AD
description: Azure Active Directory (Azure AD) отслеживает действия пользователя, регистрирует показатели и создает отчеты журнала аудита, помогающие понять, как пользователи переходят к службам Azure AD и используют их.
localization_priority: Priority
author: dhanyahk
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4df05291b4ce06312f4797b5f89ae49d74246ed5
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629322"
---
# <a name="azure-ad-audit-log-api-overview"></a><span data-ttu-id="84de4-103">Обзор API журнала аудита Azure AD</span><span class="sxs-lookup"><span data-stu-id="84de4-103">Azure AD audit log API overview</span></span>

<span data-ttu-id="84de4-104">Azure Active Directory (Azure AD) отслеживает действия пользователя, регистрирует показатели и создает отчеты журнала аудита, помогающие понять, как пользователи переходят к службам Azure AD и используют их.</span><span class="sxs-lookup"><span data-stu-id="84de4-104">Azure Active Directory (Azure AD) tracks user activity and sign-in metrics and creates audit log reports that help you understand how your users access and leverage Azure AD services.</span></span> <span data-ttu-id="84de4-105">Чтобы анализировать данные, лежащие в основе этих отчетов, и создавать настраиваемые решения в соответствии с конкретными требованиями организации, используйте API Microsoft Graph в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="84de4-105">Use the Microsoft Graph API for Azure AD to analyze the data underlying these reports and to create custom solutions tailored to your organization's specific needs.</span></span>

## <a name="what-are-azure-ad-activity-logs"></a><span data-ttu-id="84de4-106">Что такое журналы аудита Azure AD?</span><span class="sxs-lookup"><span data-stu-id="84de4-106">What are Azure AD activity logs?</span></span>

<span data-ttu-id="84de4-107">Azure AD предоставляет два типа журналов активности:</span><span class="sxs-lookup"><span data-stu-id="84de4-107">Azure AD provides two types of activity logs:</span></span>

- <span data-ttu-id="84de4-108">журналы аудита;</span><span class="sxs-lookup"><span data-stu-id="84de4-108">audit logs</span></span>
- <span data-ttu-id="84de4-109">журналы входа.</span><span class="sxs-lookup"><span data-stu-id="84de4-109">sign-in logs</span></span>

### <a name="audit-logs"></a><span data-ttu-id="84de4-110">Журналы аудита</span><span class="sxs-lookup"><span data-stu-id="84de4-110">Audit logs</span></span>

<span data-ttu-id="84de4-111">Отчет об активности журналов аудита предоставляет доступ к истории всех выполненных задач в клиенте.</span><span class="sxs-lookup"><span data-stu-id="84de4-111">The audit logs activity report provides you with access to the history of every task performed in your tenant.</span></span> <span data-ttu-id="84de4-112">Отчет журналов аудита предоставляет записи о действиях системы для соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="84de4-112">The audit logs report provides you with records of system activities for compliance.</span></span> <span data-ttu-id="84de4-113">Помимо прочего, предоставляемые данные позволяют рассматривать типичные сценарии, например:</span><span class="sxs-lookup"><span data-stu-id="84de4-113">Amongst others, the provided data enables you to address common scenarios such as:</span></span>

- <span data-ttu-id="84de4-114">Кто предоставил доступ группе администраторов к каталогу пользователя?</span><span class="sxs-lookup"><span data-stu-id="84de4-114">Who granted admin group access to a directory user?</span></span>
- <span data-ttu-id="84de4-115">Какие пользователи входят в недавно приобретенное приложение?</span><span class="sxs-lookup"><span data-stu-id="84de4-115">Which users are signing in to a recently acquired app?</span></span>
- <span data-ttu-id="84de4-116">Сколько сбросов паролей выполнено в каталоге?</span><span class="sxs-lookup"><span data-stu-id="84de4-116">How many passwords resets were made within the directory?</span></span>

### <a name="sign-in-logs"></a><span data-ttu-id="84de4-117">Журналы входа</span><span class="sxs-lookup"><span data-stu-id="84de4-117">sign-in logs</span></span>

<span data-ttu-id="84de4-118">Отчет о действиях входа помогает определить, кто выполнял задачи, указанные в отчетах журнала аудита.</span><span class="sxs-lookup"><span data-stu-id="84de4-118">The sign-ins activity report helps you determine who performed the tasks reported by audit log reports.</span></span> <span data-ttu-id="84de4-119">Отчет о действиях входа помогает ответить на представленные ниже вопросы.</span><span class="sxs-lookup"><span data-stu-id="84de4-119">The sign-ins activity report helps you answer questions like:</span></span>

- <span data-ttu-id="84de4-120">Какой шаблон входа использует пользователь?</span><span class="sxs-lookup"><span data-stu-id="84de4-120">What is the sign in pattern of a user?</span></span>
- <span data-ttu-id="84de4-121">Сколько пользователей выполнило вход за прошлую неделю?</span><span class="sxs-lookup"><span data-stu-id="84de4-121">How many users have signed in during the last week?</span></span>
- <span data-ttu-id="84de4-122">Какое состояние у этих входов?</span><span class="sxs-lookup"><span data-stu-id="84de4-122">What's the status of these sign-ins?</span></span>

## <a name="what-can-i-do-with-audit-log-apis-in-microsoft-graph"></a><span data-ttu-id="84de4-123">Как можно использовать API журнала аудита в Microsoft Graph?</span><span class="sxs-lookup"><span data-stu-id="84de4-123">What can I do with audit log APIs in Microsoft Graph?</span></span>

<span data-ttu-id="84de4-124">Ниже приведены популярные запросы для работы с данными журнала аудита.</span><span class="sxs-lookup"><span data-stu-id="84de4-124">Here are popular requests for working with audit log data:</span></span>

<span data-ttu-id="84de4-125">Operation</span><span class="sxs-lookup"><span data-stu-id="84de4-125">Operation</span></span> | <span data-ttu-id="84de4-126">URL-адрес</span><span class="sxs-lookup"><span data-stu-id="84de4-126">URL</span></span>
:----------|:----
<span data-ttu-id="84de4-127">Получение действий пользователей клиента</span><span class="sxs-lookup"><span data-stu-id="84de4-127">GET tenant user activities</span></span> | [<span data-ttu-id="84de4-128">GET https://graph.microsoft.com/v1.0/auditLogs/directoryAudits</span><span class="sxs-lookup"><span data-stu-id="84de4-128">GEThttps://graph.microsoft.com/v1.0/auditLogs/directoryAudits</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/directoryAudits&version=v1.0)
<span data-ttu-id="84de4-129">Получение входов пользователей клиента</span><span class="sxs-lookup"><span data-stu-id="84de4-129">GET tenant user sign-ins</span></span> | [<span data-ttu-id="84de4-130">GET https://graph.microsoft.com/v1.0/auditLogs/signIns</span><span class="sxs-lookup"><span data-stu-id="84de4-130">GEThttps://graph.microsoft.com/v1.0/auditLogs/signIns</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/signIns&version=v1.0)

## <a name="what-licenses-do-i-need"></a><span data-ttu-id="84de4-131">Какие лицензии нужны?</span><span class="sxs-lookup"><span data-stu-id="84de4-131">What licenses do I need?</span></span>

<span data-ttu-id="84de4-132">Отчеты журнала аудита доступны для компонентов, на которые у вас есть лицензии.</span><span class="sxs-lookup"><span data-stu-id="84de4-132">Audit log reports are available for features that you've licensed.</span></span>  <span data-ttu-id="84de4-133">Если у вас есть лицензия на определенный компонент, вам будет предоставлен доступ к соответствующим журналам аудита.</span><span class="sxs-lookup"><span data-stu-id="84de4-133">If you have a license for a specific feature, you also have access to its audit logs.</span></span>

<span data-ttu-id="84de4-134">Например, вам нужна лицензия на Azure AD Premium P1, чтобы получить доступ к отчетам аудита самостоятельного изменения паролей.</span><span class="sxs-lookup"><span data-stu-id="84de4-134">For example, you need an Azure AD Premium P1 license to access self-service password audit reports.</span></span>  <span data-ttu-id="84de4-135">Дополнительные сведения см. на странице [лицензий Azure AD](https://azure.microsoft.com/pricing/details/active-directory/).</span><span class="sxs-lookup"><span data-stu-id="84de4-135">To learn more, see [Azure AD licensing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

<span data-ttu-id="84de4-136">Для отчетов входов требуется лицензия на Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="84de4-136">Sign-in reports require an Azure AD Premium license.</span></span>

<span data-ttu-id="84de4-137">Дополнительные сведения см. на странице [Цены на Azure AD](https://azure.microsoft.com/pricing/details/active-directory/).</span><span class="sxs-lookup"><span data-stu-id="84de4-137">To learn more, see [Azure AD pricing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

## <a name="next-steps"></a><span data-ttu-id="84de4-138">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="84de4-138">Next Steps</span></span>

- <span data-ttu-id="84de4-139">[Зарегистрируйте приложение](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal), чтобы соответствовать предварительным требованиям журнала аудита.</span><span class="sxs-lookup"><span data-stu-id="84de4-139">[Register your app](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to satisfy audit log prerequisites.</span></span> 
- <span data-ttu-id="84de4-140">Ознакомьтесь с примерами журналов [аудита](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-audit-samples) и [входа](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples).</span><span class="sxs-lookup"><span data-stu-id="84de4-140">Learn from [audit log](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-audit-samples) and [sign-in samples](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples).</span></span>  
- <span data-ttu-id="84de4-141">Изучите действия и ресурс [directoryAudit](directoryaudit.md).</span><span class="sxs-lookup"><span data-stu-id="84de4-141">Review [directoryAudit](directoryaudit.md) resource and actions.</span></span>
- <span data-ttu-id="84de4-142">Изучите действия и ресурс [signIn](signin.md).</span><span class="sxs-lookup"><span data-stu-id="84de4-142">Review [signIn](signin.md) resource and actions.</span></span> 
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/azure-ad-auditlog-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
