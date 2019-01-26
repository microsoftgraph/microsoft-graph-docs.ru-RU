---
title: Обзор API журнала аудита Azure AD
description: Azure Active Directory (Azure AD) отслеживает действия пользователя, регистрирует показатели и создает отчеты журнала аудита, помогающие понять, как пользователи переходят к службам Azure AD и используют их. Чтобы анализировать данные, лежащие в основе этих отчетов, и создавать настраиваемые решения в соответствии с конкретными требованиями организации, используйте API Microsoft Graph в Azure AD.
localization_priority: Priority
ms.openlocfilehash: 89be0007ae6c13fb48ba165ca991f5dfa9d9b9cf
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509604"
---
# <a name="azure-ad-audit-log-api-overview"></a><span data-ttu-id="fa687-104">Обзор API журнала аудита Azure AD</span><span class="sxs-lookup"><span data-stu-id="fa687-104">Azure AD audit log API overview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa687-105">Azure Active Directory (Azure AD) отслеживает действия пользователя, регистрирует показатели и создает отчеты журнала аудита, помогающие понять, как пользователи переходят к службам Azure AD и используют их.</span><span class="sxs-lookup"><span data-stu-id="fa687-105">Azure Active Directory (Azure AD) tracks user activity and sign-in metrics and creates audit log reports that help you understand how your users access and leverage Azure AD services.</span></span> <span data-ttu-id="fa687-106">Чтобы анализировать данные, лежащие в основе этих отчетов, и создавать настраиваемые решения в соответствии с конкретными требованиями организации, используйте API Microsoft Graph в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="fa687-106">Use the Microsoft Graph API for Azure AD to analyze the data underlying these reports and to create custom solutions tailored to your organization's specific needs.</span></span>

## <a name="what-are-azure-ad-activity-logs"></a><span data-ttu-id="fa687-107">Что такое журналы аудита Azure AD?</span><span class="sxs-lookup"><span data-stu-id="fa687-107">What are Azure AD activity logs?</span></span>

<span data-ttu-id="fa687-108">Azure AD предоставляет два типа журналов активности:</span><span class="sxs-lookup"><span data-stu-id="fa687-108">Azure AD provides two types of activity logs:</span></span>

- <span data-ttu-id="fa687-109">журналы аудита;</span><span class="sxs-lookup"><span data-stu-id="fa687-109">audit logs</span></span> 
- <span data-ttu-id="fa687-110">журналы входа.</span><span class="sxs-lookup"><span data-stu-id="fa687-110">sign-in logs</span></span>

### <a name="audit-logs"></a><span data-ttu-id="fa687-111">Журналы аудита</span><span class="sxs-lookup"><span data-stu-id="fa687-111">Audit logs</span></span>

<span data-ttu-id="fa687-112">Отчет об активности журналов аудита предоставляет доступ к истории всех выполненных задач в клиенте.</span><span class="sxs-lookup"><span data-stu-id="fa687-112">The audit logs activity report provides you with access to the history of every task performed in your tenant.</span></span> <span data-ttu-id="fa687-113">Отчет журналов аудита предоставляет записи о действиях системы для соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="fa687-113">The audit logs report provides you with records of system activities for compliance.</span></span> <span data-ttu-id="fa687-114">Помимо прочего, предоставляемые данные позволяют рассматривать типичные сценарии, например:</span><span class="sxs-lookup"><span data-stu-id="fa687-114">Amongst others, the provided data enables you to address common scenarios such as:</span></span>

- <span data-ttu-id="fa687-115">Кто предоставил доступ группе администраторов к каталогу пользователя?</span><span class="sxs-lookup"><span data-stu-id="fa687-115">Who granted admin group access to a directory user?</span></span>

- <span data-ttu-id="fa687-116">Какие пользователи входят в недавно приобретенное приложение?</span><span class="sxs-lookup"><span data-stu-id="fa687-116">Which users are signing in to a recently acquired app?</span></span>

- <span data-ttu-id="fa687-117">Сколько сбросов паролей выполнено в каталоге?</span><span class="sxs-lookup"><span data-stu-id="fa687-117">How many passwords resets were made within the directory?</span></span>

### <a name="sign-in-logs"></a><span data-ttu-id="fa687-118">Журналы входа</span><span class="sxs-lookup"><span data-stu-id="fa687-118">Sign in logs</span></span>

<span data-ttu-id="fa687-119">Отчет о действиях входа помогает определить, кто выполнял задачи, указанные в отчетах журнала аудита.</span><span class="sxs-lookup"><span data-stu-id="fa687-119">The sign-ins activity report helps you determine who performed the tasks reported by audit log reports.</span></span> <span data-ttu-id="fa687-120">Отчет о действиях входа помогает ответить на представленные ниже вопросы.</span><span class="sxs-lookup"><span data-stu-id="fa687-120">The sign-ins activity report helps you answer questions like:</span></span>

- <span data-ttu-id="fa687-121">Какой шаблон входа использует пользователь?</span><span class="sxs-lookup"><span data-stu-id="fa687-121">What is the sign in pattern of a user?</span></span>
- <span data-ttu-id="fa687-122">Сколько пользователей выполнило вход за прошлую неделю?</span><span class="sxs-lookup"><span data-stu-id="fa687-122">How many users have signed in during the last week?</span></span>
- <span data-ttu-id="fa687-123">Какое состояние у этих входов?</span><span class="sxs-lookup"><span data-stu-id="fa687-123">What's the status of these sign-ins?</span></span>

## <a name="what-can-i-do-with-audit-log-apis-in-microsoft-graph"></a><span data-ttu-id="fa687-124">Как можно использовать API журнала аудита в Microsoft Graph?</span><span class="sxs-lookup"><span data-stu-id="fa687-124">What can I do with audit log APIs in Microsoft Graph?</span></span>

<span data-ttu-id="fa687-125">Ниже приведены популярные запросы для работы с данными журнала аудита.</span><span class="sxs-lookup"><span data-stu-id="fa687-125">Here are popular requests for working with audit log data:</span></span>

<span data-ttu-id="fa687-126">Операция</span><span class="sxs-lookup"><span data-stu-id="fa687-126">Operation</span></span> | <span data-ttu-id="fa687-127">URL-адрес</span><span class="sxs-lookup"><span data-stu-id="fa687-127">URL</span></span>
:----------|:----
<span data-ttu-id="fa687-128">Получение действий пользователей клиента</span><span class="sxs-lookup"><span data-stu-id="fa687-128">GET tenant user activities</span></span> | [https://graph.microsoft.com/beta/auditLogs/directoryAudits](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/directoryAudits&version=beta)
<span data-ttu-id="fa687-129">Получение входов пользователей клиента</span><span class="sxs-lookup"><span data-stu-id="fa687-129">GET tenant user sign-ins</span></span> | [https://graph.microsoft.com/beta/auditLogs/signIns](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/signIns&version=beta)

## <a name="what-licenses-do-i-need"></a><span data-ttu-id="fa687-130">Какие лицензии нужны?</span><span class="sxs-lookup"><span data-stu-id="fa687-130">What licenses do I need?</span></span>

<span data-ttu-id="fa687-131">Отчеты журнала аудита доступны для компонентов, на которые у вас есть лицензии.</span><span class="sxs-lookup"><span data-stu-id="fa687-131">Audit log reports are available for features that you've licensed.</span></span>  <span data-ttu-id="fa687-132">Если у вас есть лицензия на определенный компонент, вам будет предоставлен доступ к соответствующим журналам аудита.</span><span class="sxs-lookup"><span data-stu-id="fa687-132">If you have a license for a specific feature, you also have access to its audit logs.</span></span>

<span data-ttu-id="fa687-133">Например, вам нужна лицензия на Azure AD Premium P1, чтобы получить доступ к отчетам аудита самостоятельного изменения паролей.</span><span class="sxs-lookup"><span data-stu-id="fa687-133">For example, you need an Azure AD Premium P1 license to access self-service password audit reports.</span></span>  <span data-ttu-id="fa687-134">Дополнительные сведения см. на странице [лицензий Azure AD](https://azure.microsoft.com/pricing/details/active-directory/).</span><span class="sxs-lookup"><span data-stu-id="fa687-134">To learn more, see [Azure AD licensing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

<span data-ttu-id="fa687-135">Для отчетов входов требуется лицензия на Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="fa687-135">Sign-in reports require an Azure AD Premium license.</span></span>

<span data-ttu-id="fa687-136">Дополнительные сведения см. на странице [Цены на Azure AD](https://azure.microsoft.com/pricing/details/active-directory/).</span><span class="sxs-lookup"><span data-stu-id="fa687-136">To learn more, see [Azure AD pricing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

## <a name="next-steps"></a><span data-ttu-id="fa687-137">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="fa687-137">Next Steps</span></span>

- <span data-ttu-id="fa687-138">[Зарегистрируйте приложение](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal), чтобы соответствовать предварительным требованиям журнала аудита.</span><span class="sxs-lookup"><span data-stu-id="fa687-138">[Register your app](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to satisfy audit log prerequisites.</span></span> 
- <span data-ttu-id="fa687-139">Ознакомьтесь с примерами журналов [аудита](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-audit-samples) и [входа](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples).</span><span class="sxs-lookup"><span data-stu-id="fa687-139">Learn from [audit log](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-audit-samples) and [sign-in samples](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples).</span></span>  
- <span data-ttu-id="fa687-140">Изучите действия и ресурс [directoryAudit](directoryaudit.md).</span><span class="sxs-lookup"><span data-stu-id="fa687-140">Review [directoryAudit](directoryaudit.md) resource and actions.</span></span>
- <span data-ttu-id="fa687-141">Изучите действия и ресурс [signIn](signin.md).</span><span class="sxs-lookup"><span data-stu-id="fa687-141">Review [signIn](signin.md) resource and actions.</span></span> 
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/azure-ad-auditlog-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
