---
title: Общие сведения о интерфейс API журнала аудита Azure AD
description: Azure Active Directory (Azure AD) отслеживает показатели активности и входа пользователя и создает аудита отчеты по журналу, которые помогут вам понять, как пользователям доступ к и эффективного использования служб Azure AD. Используйте Microsoft Graph API для Azure AD для анализа данных базового этих отчетов и для создания пользовательских решений для конкретных требованиям вашей организации.
localization_priority: Priority
ms.openlocfilehash: 07d285ce4e7fbf736900c1d6d4acdf159b451424
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826224"
---
# <a name="azure-ad-audit-log-api-overview"></a><span data-ttu-id="98b92-104">Общие сведения о интерфейс API журнала аудита Azure AD</span><span class="sxs-lookup"><span data-stu-id="98b92-104">Azure AD audit log API overview</span></span>

> <span data-ttu-id="98b92-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="98b92-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="98b92-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98b92-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="98b92-107">Azure Active Directory (Azure AD) отслеживает показатели активности и входа пользователя и создает аудита отчеты по журналу, которые помогут вам понять, как пользователям доступ к и эффективного использования служб Azure AD.</span><span class="sxs-lookup"><span data-stu-id="98b92-107">Azure Active Directory (Azure AD) tracks user activity and sign-in metrics and creates audit log reports that help you understand how your users access and leverage Azure AD services.</span></span> <span data-ttu-id="98b92-108">Используйте Microsoft Graph API для Azure AD для анализа данных базового этих отчетов и для создания пользовательских решений для конкретных требованиям вашей организации.</span><span class="sxs-lookup"><span data-stu-id="98b92-108">Use the Microsoft Graph API for Azure AD to analyze the data underlying these reports and to create custom solutions tailored to your organization's specific needs.</span></span>

## <a name="what-are-azure-ad-activity-logs"></a><span data-ttu-id="98b92-109">Что такое действие Azure AD журналы?</span><span class="sxs-lookup"><span data-stu-id="98b92-109">What are Azure AD activity logs?</span></span>

<span data-ttu-id="98b92-110">Azure AD обеспечивает два типа журналы активности.</span><span class="sxs-lookup"><span data-stu-id="98b92-110">Azure AD provides two types of activity logs:</span></span>

- <span data-ttu-id="98b92-111">журналы аудита</span><span class="sxs-lookup"><span data-stu-id="98b92-111">audit logs</span></span> 
- <span data-ttu-id="98b92-112">журналы входа</span><span class="sxs-lookup"><span data-stu-id="98b92-112">sign-in logs</span></span>

### <a name="audit-logs"></a><span data-ttu-id="98b92-113">Журналы аудита</span><span class="sxs-lookup"><span data-stu-id="98b92-113">Audit logs</span></span>

<span data-ttu-id="98b92-114">Отчете журналы аудита предоставляет доступ к журналу каждой задачи выполняется в вашего клиента.</span><span class="sxs-lookup"><span data-stu-id="98b92-114">The audit logs activity report provides you with access to the history of every task performed in your tenant.</span></span> <span data-ttu-id="98b92-115">Отчет о журналы аудита предоставляет записей действий системы для соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="98b92-115">The audit logs report provides you with records of system activities for compliance.</span></span> <span data-ttu-id="98b92-116">Помимо прочего предоставленных данных позволяет вам устранения распространенных сценариев, таких как:</span><span class="sxs-lookup"><span data-stu-id="98b92-116">Amongst others, the provided data enables you to address common scenarios such as:</span></span>

- <span data-ttu-id="98b92-117">Доступ к группе администрирования, предоставленные пользователю каталога?</span><span class="sxs-lookup"><span data-stu-id="98b92-117">Who granted admin group access to a directory user?</span></span>

- <span data-ttu-id="98b92-118">Пользователей, которые вход с использованием недавно приобретенного приложения?</span><span class="sxs-lookup"><span data-stu-id="98b92-118">Which users are signing in to a recently acquired app?</span></span>

- <span data-ttu-id="98b92-119">Сбрасывает пароли сколько были внесены в пределах каталога?</span><span class="sxs-lookup"><span data-stu-id="98b92-119">How many passwords resets were made within the directory?</span></span>

### <a name="sign-in-logs"></a><span data-ttu-id="98b92-120">Войдите в журналах</span><span class="sxs-lookup"><span data-stu-id="98b92-120">Sign in logs</span></span>

<span data-ttu-id="98b92-121">Войти в отчете приводятся рекомендации по определению, выполнения задач, о которых сообщает отчеты по журналу аудита.</span><span class="sxs-lookup"><span data-stu-id="98b92-121">The sign-ins activity report helps you determine who performed the tasks reported by audit log reports.</span></span> <span data-ttu-id="98b92-122">Войти в отчете помогает ответить на вопросы:</span><span class="sxs-lookup"><span data-stu-id="98b92-122">The sign-ins activity report helps you answer questions like:</span></span>

- <span data-ttu-id="98b92-123">Что такое входа в шаблоне пользователя?</span><span class="sxs-lookup"><span data-stu-id="98b92-123">What is the sign in pattern of a user?</span></span>
- <span data-ttu-id="98b92-124">Сколько пользователей вышли ходе за прошлую неделю?</span><span class="sxs-lookup"><span data-stu-id="98b92-124">How many users have signed in during the last week?</span></span>
- <span data-ttu-id="98b92-125">Что такое состояние этих войти в систему?</span><span class="sxs-lookup"><span data-stu-id="98b92-125">What's the status of these sign-ins?</span></span>

## <a name="what-can-i-do-with-audit-log-apis-in-microsoft-graph"></a><span data-ttu-id="98b92-126">Что можно сделать с помощью журнала аудита интерфейсы API в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="98b92-126">What can I do with audit log APIs in Microsoft Graph?</span></span>

<span data-ttu-id="98b92-127">Вот популярные запросы для работы с данными журнала аудита.</span><span class="sxs-lookup"><span data-stu-id="98b92-127">Here are popular requests for working with audit log data:</span></span>

<span data-ttu-id="98b92-128">Операция</span><span class="sxs-lookup"><span data-stu-id="98b92-128">Operation</span></span> | <span data-ttu-id="98b92-129">URL-адрес</span><span class="sxs-lookup"><span data-stu-id="98b92-129">URL</span></span>
:----------|:----
<span data-ttu-id="98b92-130">Получение клиентом действия пользователя</span><span class="sxs-lookup"><span data-stu-id="98b92-130">GET tenant user activities</span></span> | [https://graph.microsoft.com/beta/auditLogs/directoryAudits](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/directoryAudits&version=beta)
<span data-ttu-id="98b92-131">Получение клиентом входы</span><span class="sxs-lookup"><span data-stu-id="98b92-131">GET tenant user sign-ins</span></span> | [https://graph.microsoft.com/beta/auditLogs/signIns](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/signIns&version=beta)

## <a name="what-licenses-do-i-need"></a><span data-ttu-id="98b92-132">Какие лицензий требуется?</span><span class="sxs-lookup"><span data-stu-id="98b92-132">What licenses do I need?</span></span>

<span data-ttu-id="98b92-133">Отчеты по журналу аудита, доступных для функции, которые ли применена лицензия.</span><span class="sxs-lookup"><span data-stu-id="98b92-133">Audit log reports are available for features that you've licensed.</span></span>  <span data-ttu-id="98b92-134">Если у вас есть лицензии для конкретного компонента, также имеют доступ к его журналы аудита.</span><span class="sxs-lookup"><span data-stu-id="98b92-134">If you have a license for a specific feature, you also have access to its audit logs.</span></span>

<span data-ttu-id="98b92-135">Например требуется лицензия P1 Azure AD Premium для доступа к отчетам аудита самостоятельного пароль.</span><span class="sxs-lookup"><span data-stu-id="98b92-135">For example, you need an Azure AD Premium P1 license to access self-service password audit reports.</span></span>  <span data-ttu-id="98b92-136">Для получения дополнительных сведений см. [: Лицензирование Azure AD](https://azure.microsoft.com/pricing/details/active-directory/).</span><span class="sxs-lookup"><span data-stu-id="98b92-136">To learn more, see [Azure AD licensing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

<span data-ttu-id="98b92-137">Входа в отчетах требуется лицензия на Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="98b92-137">Sign-in reports require an Azure AD Premium license.</span></span>

<span data-ttu-id="98b92-138">Для получения дополнительных сведений см [Цена Azure AD](https://azure.microsoft.com/pricing/details/active-directory/).</span><span class="sxs-lookup"><span data-stu-id="98b92-138">To learn more, see [Azure AD pricing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

## <a name="next-steps"></a><span data-ttu-id="98b92-139">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="98b92-139">Next Steps</span></span>

- <span data-ttu-id="98b92-140">[Регистрация приложения](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) для удовлетворения необходимых компонентов журнала аудита.</span><span class="sxs-lookup"><span data-stu-id="98b92-140">[Register your app](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to satisfy audit log prerequisites.</span></span> 
- <span data-ttu-id="98b92-141">Сведения из [журнала аудита](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-audit-samples) и [примеры, вход](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples).</span><span class="sxs-lookup"><span data-stu-id="98b92-141">Learn from [audit log](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-audit-samples) and [sign-in samples](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples).</span></span>  
- <span data-ttu-id="98b92-142">Ознакомьтесь с [directoryAudit](directoryaudit.md) ресурсов и действия.</span><span class="sxs-lookup"><span data-stu-id="98b92-142">Review [directoryAudit](directoryaudit.md) resource and actions.</span></span>
- <span data-ttu-id="98b92-143">Просмотрите [входить](signin.md) ресурсов и действия.</span><span class="sxs-lookup"><span data-stu-id="98b92-143">Review [signIn](signin.md) resource and actions.</span></span> 
