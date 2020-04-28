---
title: Обзор API журнала аудита Azure AD
description: Azure Active Directory (Azure AD) отслеживает действия пользователя, регистрирует показатели входа и создает отчеты журнала аудита, помогающие понять, как пользователи переходят к службам Azure AD и используют их. Чтобы анализировать данные, лежащие в основе этих отчетов, и создавать настраиваемые решения в соответствии с конкретными требованиями организации, используйте API Microsoft Graph в Azure AD.
localization_priority: Priority
doc_type: conceptualPageType
ms.prod: microsoft-identity-platform
author: kholtz
ms.openlocfilehash: 3e27d397087781e7afc35e5f5ca1b06b3ae4062c
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2020
ms.locfileid: "43917581"
---
# <a name="azure-ad-audit-log-api-overview"></a><span data-ttu-id="b4791-104">Обзор API журнала аудита Azure AD</span><span class="sxs-lookup"><span data-stu-id="b4791-104">Azure AD audit log API overview</span></span>

<span data-ttu-id="b4791-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4791-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4791-106">Azure Active Directory (Azure AD) отслеживает действия пользователя, регистрирует показатели входа и создает отчеты журнала аудита, помогающие понять, как пользователи переходят к службам Azure AD и используют их.</span><span class="sxs-lookup"><span data-stu-id="b4791-106">Azure Active Directory (Azure AD) tracks user activity and sign-in metrics and creates audit log reports that help you understand how your users access and use Azure AD services.</span></span> <span data-ttu-id="b4791-107">Чтобы анализировать данные, лежащие в основе этих отчетов, и создавать настраиваемые решения в соответствии с конкретными требованиями организации, используйте API Microsoft Graph в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b4791-107">Use the Microsoft Graph API for Azure AD to analyze the data underlying these reports and to create custom solutions tailored to your organization's specific needs.</span></span>

## <a name="what-are-azure-ad-activity-logs"></a><span data-ttu-id="b4791-108">Что такое журналы аудита Azure AD?</span><span class="sxs-lookup"><span data-stu-id="b4791-108">What are Azure AD activity logs?</span></span>

<span data-ttu-id="b4791-109">Azure AD предоставляет три типа журналов активности:</span><span class="sxs-lookup"><span data-stu-id="b4791-109">Azure AD provides three types of activity logs:</span></span>

- <span data-ttu-id="b4791-110">Журналы аудита</span><span class="sxs-lookup"><span data-stu-id="b4791-110">Audit logs</span></span> 
- <span data-ttu-id="b4791-111">Журналы входа</span><span class="sxs-lookup"><span data-stu-id="b4791-111">Sign-in logs</span></span>
- <span data-ttu-id="b4791-112">Журналы подготовки</span><span class="sxs-lookup"><span data-stu-id="b4791-112">Provisioning logs</span></span>

### <a name="audit-logs"></a><span data-ttu-id="b4791-113">Журналы аудита</span><span class="sxs-lookup"><span data-stu-id="b4791-113">Audit logs</span></span>

<span data-ttu-id="b4791-114">Отчет об активности журналов аудита предоставляет доступ к истории всех выполненных задач в клиенте.</span><span class="sxs-lookup"><span data-stu-id="b4791-114">The audit logs activity report provides you with access to the history of every task performed in your tenant.</span></span> <span data-ttu-id="b4791-115">Отчет журналов аудита предоставляет записи о действиях системы для соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="b4791-115">The audit logs report provides you with records of system activities for compliance.</span></span> <span data-ttu-id="b4791-116">Помимо прочего, предоставляемые данные позволяют рассматривать типичные сценарии, например:</span><span class="sxs-lookup"><span data-stu-id="b4791-116">Amongst others, the provided data enables you to address common scenarios such as:</span></span>

- <span data-ttu-id="b4791-117">Кто предоставил доступ группе администраторов к каталогу пользователя?</span><span class="sxs-lookup"><span data-stu-id="b4791-117">Who granted admin group access to a directory user?</span></span>

- <span data-ttu-id="b4791-118">Какие пользователи входят в недавно приобретенное приложение?</span><span class="sxs-lookup"><span data-stu-id="b4791-118">Which users are signing in to a recently acquired app?</span></span>

- <span data-ttu-id="b4791-119">Сколько сбросов паролей выполнено в каталоге?</span><span class="sxs-lookup"><span data-stu-id="b4791-119">How many passwords resets were made within the directory?</span></span>

### <a name="sign-in-logs"></a><span data-ttu-id="b4791-120">Журналы входа</span><span class="sxs-lookup"><span data-stu-id="b4791-120">Sign-in logs</span></span>

<span data-ttu-id="b4791-121">Отчет о действиях входа помогает определить, кто выполнял задачи, указанные в отчетах журнала аудита.</span><span class="sxs-lookup"><span data-stu-id="b4791-121">The sign-ins activity report helps you determine who performed the tasks reported by audit log reports.</span></span> <span data-ttu-id="b4791-122">Отчет о действиях входа помогает ответить на представленные ниже вопросы.</span><span class="sxs-lookup"><span data-stu-id="b4791-122">The sign-ins activity report helps you answer questions like:</span></span>

- <span data-ttu-id="b4791-123">Какой шаблон входа использует пользователь?</span><span class="sxs-lookup"><span data-stu-id="b4791-123">What is the sign in pattern of a user?</span></span>
- <span data-ttu-id="b4791-124">Сколько пользователей выполнило вход за прошлую неделю?</span><span class="sxs-lookup"><span data-stu-id="b4791-124">How many users have signed in during the last week?</span></span>
- <span data-ttu-id="b4791-125">Какое состояние у этих входов?</span><span class="sxs-lookup"><span data-stu-id="b4791-125">What's the status of these sign-ins?</span></span>

### <a name="provisioning-logs"></a><span data-ttu-id="b4791-126">Журналы подготовки</span><span class="sxs-lookup"><span data-stu-id="b4791-126">Provisioning logs</span></span>
<span data-ttu-id="b4791-127">Журналы подготовки позволяют просматривать все действия, выполненные службой подготовки Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b4791-127">The provisioning logs help you see all the actions performed by the Azure AD provisioning service.</span></span> <span data-ttu-id="b4791-128">Журналы подготовки помогают ответить на следующие вопросы:</span><span class="sxs-lookup"><span data-stu-id="b4791-128">The provisioning logs help you answer questions like:</span></span>

- <span data-ttu-id="b4791-129">Какие группы были успешно созданы в ServiceNow?</span><span class="sxs-lookup"><span data-stu-id="b4791-129">What groups were successfully created in ServiceNow?</span></span>
- <span data-ttu-id="b4791-130">Какие роли были импортированы из Amazon Web Services?</span><span class="sxs-lookup"><span data-stu-id="b4791-130">What roles were imported from Amazon Web Services?</span></span>
- <span data-ttu-id="b4791-131">Каких пользователей не удалось создать из Workday?</span><span class="sxs-lookup"><span data-stu-id="b4791-131">What users were unsuccessfully created from Workday?</span></span>

## <a name="what-can-i-do-with-audit-log-apis-in-microsoft-graph"></a><span data-ttu-id="b4791-132">Как можно использовать API журнала аудита в Microsoft Graph?</span><span class="sxs-lookup"><span data-stu-id="b4791-132">What can I do with audit log APIs in Microsoft Graph?</span></span>

<span data-ttu-id="b4791-133">Ниже приведены популярные запросы для работы с данными журнала аудита.</span><span class="sxs-lookup"><span data-stu-id="b4791-133">Here are popular requests for working with audit log data:</span></span>

<span data-ttu-id="b4791-134">Операция</span><span class="sxs-lookup"><span data-stu-id="b4791-134">Operation</span></span> | <span data-ttu-id="b4791-135">URL-адрес</span><span class="sxs-lookup"><span data-stu-id="b4791-135">URL</span></span>
:----------|:----
<span data-ttu-id="b4791-136">Получение действий пользователей клиента</span><span class="sxs-lookup"><span data-stu-id="b4791-136">GET tenant user activities</span></span> | [https://graph.microsoft.com/beta/auditLogs/directoryAudits](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/directoryAudits&version=beta)
<span data-ttu-id="b4791-137">Получение входов пользователей клиента</span><span class="sxs-lookup"><span data-stu-id="b4791-137">GET tenant user sign-ins</span></span> | [https://graph.microsoft.com/beta/auditLogs/signIns](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/signIns&version=beta)
<span data-ttu-id="b4791-138">Получение журналов подготовки</span><span class="sxs-lookup"><span data-stu-id="b4791-138">GET provisioning logs</span></span> | [https://graph.microsoft.com/beta/auditLogs/provisioning](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/Provisioning&version=beta)

## <a name="what-licenses-do-i-need"></a><span data-ttu-id="b4791-139">Какие лицензии нужны?</span><span class="sxs-lookup"><span data-stu-id="b4791-139">What licenses do I need?</span></span>

<span data-ttu-id="b4791-140">Отчеты журнала аудита доступны для компонентов, на которые у вас есть лицензии.</span><span class="sxs-lookup"><span data-stu-id="b4791-140">Audit log reports are available for features that you've licensed.</span></span>  <span data-ttu-id="b4791-141">Если у вас есть лицензия на определенный компонент, вам будет предоставлен доступ к соответствующим журналам аудита.</span><span class="sxs-lookup"><span data-stu-id="b4791-141">If you have a license for a specific feature, you also have access to its audit logs.</span></span>

<span data-ttu-id="b4791-142">Например, вам нужна лицензия на Azure AD Premium P1, чтобы получить доступ к отчетам аудита самостоятельного изменения паролей.</span><span class="sxs-lookup"><span data-stu-id="b4791-142">For example, you need an Azure AD Premium P1 license to access self-service password audit reports.</span></span>  <span data-ttu-id="b4791-143">Дополнительные сведения см. на странице [лицензий Azure AD](https://azure.microsoft.com/pricing/details/active-directory/).</span><span class="sxs-lookup"><span data-stu-id="b4791-143">To learn more, see [Azure AD licensing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

<span data-ttu-id="b4791-144">Для отчетов входов требуется лицензия на Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="b4791-144">Sign-in reports require an Azure AD Premium license.</span></span>

<span data-ttu-id="b4791-145">Дополнительные сведения см. на странице [Цены на Azure AD](https://azure.microsoft.com/pricing/details/active-directory/).</span><span class="sxs-lookup"><span data-stu-id="b4791-145">To learn more, see [Azure AD pricing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

## <a name="next-steps"></a><span data-ttu-id="b4791-146">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="b4791-146">Next steps</span></span>

- <span data-ttu-id="b4791-147">[Зарегистрируйте приложение](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal), чтобы соответствовать предварительным требованиям журнала аудита.</span><span class="sxs-lookup"><span data-stu-id="b4791-147">[Register your app](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to satisfy audit log prerequisites.</span></span> 
- <span data-ttu-id="b4791-148">Ознакомьтесь с примерами журналов [аудита](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-audit-samples) и [входа](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples).</span><span class="sxs-lookup"><span data-stu-id="b4791-148">Learn from [audit log](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-audit-samples) and [sign-in samples](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples).</span></span>  
- <span data-ttu-id="b4791-149">Изучите действия и ресурс [directoryAudit](directoryaudit.md).</span><span class="sxs-lookup"><span data-stu-id="b4791-149">Review the [directoryAudit](directoryaudit.md) resource and actions.</span></span>
- <span data-ttu-id="b4791-150">Изучите действия и ресурс [signIn](signin.md).</span><span class="sxs-lookup"><span data-stu-id="b4791-150">Review the [signIn](signin.md) resource and actions.</span></span> 
- <span data-ttu-id="b4791-151">Изучите ресурс [provisioningObjectSummary](provisioningobjectsummary.md).</span><span class="sxs-lookup"><span data-stu-id="b4791-151">Review the [provisioningObjectSummary](provisioningobjectsummary.md) resource.</span></span>
