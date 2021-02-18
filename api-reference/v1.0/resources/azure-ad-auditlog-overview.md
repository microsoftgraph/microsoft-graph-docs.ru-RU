---
title: Обзор API отчетов об активности
description: Используйте API отчетов об активности в Microsoft Graph для получения доступа к отчетам Azure Active Directory, чтобы отслеживать действия пользователей в клиенте.
localization_priority: Priority
author: besiler
ms.prod: identity-and-access-reports
doc_type: conceptualPageType
ms.openlocfilehash: 36cbd8a381dc3e92ee3c1dcd17e4941c308248f0
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/18/2021
ms.locfileid: "50293066"
---
# <a name="activity-reports-api-overview"></a><span data-ttu-id="2db30-103">Обзор API отчетов об активности</span><span class="sxs-lookup"><span data-stu-id="2db30-103">Activity reports API overview</span></span>

<span data-ttu-id="2db30-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2db30-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2db30-105">Azure Active Directory (Azure AD) отслеживает действия пользователей и создает отчеты, помогающие понять, как пользователи переходят к службам Azure AD и используют их.</span><span class="sxs-lookup"><span data-stu-id="2db30-105">Azure Active Directory (Azure AD) tracks user activity and creates reports that help you understand how your users access and use Azure AD services.</span></span> <span data-ttu-id="2db30-106">Чтобы анализировать данные в этих отчетах и создавать настраиваемые решения в соответствии с конкретными требованиями организации, используйте API Microsoft Graph в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="2db30-106">Use the Microsoft Graph API for Azure AD to analyze the data in these reports and to create custom solutions tailored to your organization's specific needs.</span></span>

<span data-ttu-id="2db30-107">Доступность этих отчетов об активности определяется политиками хранения данных Azure AD.</span><span class="sxs-lookup"><span data-stu-id="2db30-107">The availability of these activity reports is governed by the Azure AD data retention policies.</span></span> <span data-ttu-id="2db30-108">Подробнее см. в статье [Политики хранение данных](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention#how-long-does-azure-ad-store-the-data).</span><span class="sxs-lookup"><span data-stu-id="2db30-108">For more information, see [data retention policies](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention#how-long-does-azure-ad-store-the-data).</span></span>

## <a name="what-are-azure-ad-activity-logs"></a><span data-ttu-id="2db30-109">Что такое журналы аудита Azure AD?</span><span class="sxs-lookup"><span data-stu-id="2db30-109">What are Azure AD activity logs?</span></span>

<span data-ttu-id="2db30-110">Azure AD предоставляет следующие типы отчетов об активности:</span><span class="sxs-lookup"><span data-stu-id="2db30-110">Azure AD provides the following types of activity reports:</span></span>

- <span data-ttu-id="2db30-111">Аудиты каталога</span><span class="sxs-lookup"><span data-stu-id="2db30-111">Directory audits</span></span>
- <span data-ttu-id="2db30-112">Входы</span><span class="sxs-lookup"><span data-stu-id="2db30-112">Sign-ins</span></span>

### <a name="directory-audits"></a><span data-ttu-id="2db30-113">Аудиты каталога</span><span class="sxs-lookup"><span data-stu-id="2db30-113">Directory audits</span></span>

<span data-ttu-id="2db30-114">Отчет аудитов каталога предоставляет доступ к истории всех выполненных задач в клиенте.</span><span class="sxs-lookup"><span data-stu-id="2db30-114">The directory audit report provides you with access to the history of every task performed in your tenant.</span></span> <span data-ttu-id="2db30-115">Отчет аудитов каталога предоставляет записи о действиях системы для обеспечения соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="2db30-115">The directory audit report provides you with records of system activities for compliance.</span></span> <span data-ttu-id="2db30-116">Помимо прочего, предоставляемые данные позволяют рассматривать типичные сценарии, например:</span><span class="sxs-lookup"><span data-stu-id="2db30-116">Amongst others, the provided data enables you to address common scenarios such as:</span></span>

- <span data-ttu-id="2db30-117">Кто предоставил доступ группе администраторов к каталогу пользователя?</span><span class="sxs-lookup"><span data-stu-id="2db30-117">Who granted admin group access to a directory user?</span></span>
- <span data-ttu-id="2db30-118">Какие пользователи входят в недавно приобретенное приложение?</span><span class="sxs-lookup"><span data-stu-id="2db30-118">Which users are signing in to a recently acquired app?</span></span>
- <span data-ttu-id="2db30-119">Сколько сбросов паролей выполнено в каталоге?</span><span class="sxs-lookup"><span data-stu-id="2db30-119">How many passwords resets were made within the directory?</span></span>

### <a name="sign-ins"></a><span data-ttu-id="2db30-120">Входы</span><span class="sxs-lookup"><span data-stu-id="2db30-120">Sign-ins</span></span>

<span data-ttu-id="2db30-121">Отчет о входах помогает определить, кто выполнял задачи, указанные в отчетах аудитов каталога.</span><span class="sxs-lookup"><span data-stu-id="2db30-121">The sign-ins report helps you determine who performed the tasks reported by directory audits.</span></span> <span data-ttu-id="2db30-122">Отчет о входах помогает ответить на представленные ниже вопросы.</span><span class="sxs-lookup"><span data-stu-id="2db30-122">The sign-ins report helps you answer questions like:</span></span>

- <span data-ttu-id="2db30-123">Какой шаблон входа использует пользователь?</span><span class="sxs-lookup"><span data-stu-id="2db30-123">What is the sign in pattern of a user?</span></span>
- <span data-ttu-id="2db30-124">Сколько пользователей выполнило вход за прошлую неделю?</span><span class="sxs-lookup"><span data-stu-id="2db30-124">How many users have signed in during the last week?</span></span>
- <span data-ttu-id="2db30-125">Какое состояние у этих входов?</span><span class="sxs-lookup"><span data-stu-id="2db30-125">What's the status of these sign-ins?</span></span>

## <a name="what-can-i-do-with-audit-log-apis-in-microsoft-graph"></a><span data-ttu-id="2db30-126">Как можно использовать API журнала аудита в Microsoft Graph?</span><span class="sxs-lookup"><span data-stu-id="2db30-126">What can I do with audit log APIs in Microsoft Graph?</span></span>

<span data-ttu-id="2db30-127">Ниже приведены популярные запросы для работы с данными журнала аудита.</span><span class="sxs-lookup"><span data-stu-id="2db30-127">The following are popular requests for working with audit log data:</span></span>

<span data-ttu-id="2db30-128">Operation</span><span class="sxs-lookup"><span data-stu-id="2db30-128">Operation</span></span> | <span data-ttu-id="2db30-129">URL-адрес</span><span class="sxs-lookup"><span data-stu-id="2db30-129">URL</span></span>
:----------|:----
<span data-ttu-id="2db30-130">Получение действий пользователей клиента</span><span class="sxs-lookup"><span data-stu-id="2db30-130">GET tenant user activities</span></span> | [<span data-ttu-id="2db30-131">GET https://graph.microsoft.com/v1.0/auditLogs/directoryAudits</span><span class="sxs-lookup"><span data-stu-id="2db30-131">GET https://graph.microsoft.com/v1.0/auditLogs/directoryAudits</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/directoryAudits&version=v1.0)
<span data-ttu-id="2db30-132">Получение входов пользователей клиента</span><span class="sxs-lookup"><span data-stu-id="2db30-132">GET tenant user sign-ins</span></span> | [<span data-ttu-id="2db30-133">GET https://graph.microsoft.com/v1.0/auditLogs/signIns</span><span class="sxs-lookup"><span data-stu-id="2db30-133">GET https://graph.microsoft.com/v1.0/auditLogs/signIns</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/signIns&version=v1.0)

## <a name="what-licenses-do-i-need"></a><span data-ttu-id="2db30-134">Какие лицензии нужны?</span><span class="sxs-lookup"><span data-stu-id="2db30-134">What licenses do I need?</span></span>

<span data-ttu-id="2db30-135">Отчеты об активности доступны для компонентов, на которые у вас есть лицензии.</span><span class="sxs-lookup"><span data-stu-id="2db30-135">Activity reports are available for features that you've licensed.</span></span> <span data-ttu-id="2db30-136">Если у вас есть лицензия на определенный компонент, вам будет предоставлен доступ к соответствующим отчетам.</span><span class="sxs-lookup"><span data-stu-id="2db30-136">If you have a license for a specific feature, you also have access to the reports.</span></span>

<span data-ttu-id="2db30-137">Например, вам нужна лицензия на Azure AD Premium P1, чтобы получить доступ к отчетам аудита самостоятельного изменения паролей.</span><span class="sxs-lookup"><span data-stu-id="2db30-137">For example, you need an Azure AD Premium P1 license to access self-service password audit reports.</span></span>  <span data-ttu-id="2db30-138">Дополнительные сведения см. на странице [лицензий Azure AD](https://azure.microsoft.com/pricing/details/active-directory/).</span><span class="sxs-lookup"><span data-stu-id="2db30-138">To learn more, see [Azure AD licensing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

<span data-ttu-id="2db30-139">Для отчетов входов требуется лицензия на Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="2db30-139">Sign-in reports require an Azure AD Premium license.</span></span>

<span data-ttu-id="2db30-140">Дополнительные сведения см. на странице [Цены на Azure AD](https://azure.microsoft.com/pricing/details/active-directory/).</span><span class="sxs-lookup"><span data-stu-id="2db30-140">To learn more, see [Azure AD pricing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

## <a name="next-steps"></a><span data-ttu-id="2db30-141">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="2db30-141">Next Steps</span></span>

- <span data-ttu-id="2db30-142">[Зарегистрируйте приложение](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal), чтобы соответствовать предварительным требованиям отчетов.</span><span class="sxs-lookup"><span data-stu-id="2db30-142">[Register your app](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to satisfy report prerequisites.</span></span> 
- <span data-ttu-id="2db30-143">Ознакомьтесь с примерами журналов [аудита](/azure/active-directory/active-directory-reporting-api-audit-samples) и [входа](/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples).</span><span class="sxs-lookup"><span data-stu-id="2db30-143">Learn from [audit log](/azure/active-directory/active-directory-reporting-api-audit-samples) and [sign-in samples](/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples).</span></span>  
- <span data-ttu-id="2db30-144">Изучите действия и ресурс [directoryAudit](directoryaudit.md).</span><span class="sxs-lookup"><span data-stu-id="2db30-144">Review [directoryAudit](directoryaudit.md) resource and actions.</span></span>
- <span data-ttu-id="2db30-145">Изучите действия и ресурс [signIn](signin.md).</span><span class="sxs-lookup"><span data-stu-id="2db30-145">Review [signIn](signin.md) resource and actions.</span></span> 
<!--
{
  "type": "#page.annotation",
  "suppressions": [
  ]
}
-->
