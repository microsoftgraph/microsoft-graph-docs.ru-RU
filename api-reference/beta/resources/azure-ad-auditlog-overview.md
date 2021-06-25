---
title: Обзор API отчетов об активности
description: Используйте API отчетов об активности в Microsoft Graph для получения доступа к отчетам Azure Active Directory, чтобы отслеживать действия пользователей в клиенте.
localization_priority: Priority
doc_type: conceptualPageType
ms.prod: identity-and-access-reports
author: besiler
ms.openlocfilehash: 78afd6477988a546c7c0e2b8db34f8933423107f
ms.sourcegitcommit: 8a9be6f65f62f29973508d82e0348d4142c18f23
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2021
ms.locfileid: "53129476"
---
# <a name="activity-reports-api-overview"></a><span data-ttu-id="8597f-103">Обзор API отчетов об активности</span><span class="sxs-lookup"><span data-stu-id="8597f-103">Activity reports API overview</span></span>

<span data-ttu-id="8597f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8597f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8597f-105">Azure Active Directory (Azure AD) отслеживает действия пользователей и создает отчеты, помогающие понять, как пользователи переходят к службам Azure AD и используют их.</span><span class="sxs-lookup"><span data-stu-id="8597f-105">Azure Active Directory (Azure AD) tracks user activity and creates reports that help you understand how your users access and use Azure AD services.</span></span> <span data-ttu-id="8597f-106">Чтобы анализировать данные в этих отчетах и создавать настраиваемые решения в соответствии с конкретными требованиями организации, используйте API Microsoft Graph в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8597f-106">Use the Microsoft Graph API for Azure AD to analyze the data in these reports and to create custom solutions tailored to your organization's specific needs.</span></span>

<span data-ttu-id="8597f-107">Доступность этих отчетов об активности определяется политиками хранения данных Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8597f-107">The availability of these activity reports is governed by the Azure AD data retention policies.</span></span> <span data-ttu-id="8597f-108">Подробнее см. в статье [Политики хранение данных](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention#how-long-does-azure-ad-store-the-data).</span><span class="sxs-lookup"><span data-stu-id="8597f-108">For more information, see [data retention policies](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention#how-long-does-azure-ad-store-the-data).</span></span>

## <a name="what-are-activity-reports"></a><span data-ttu-id="8597f-109">Что такое отчеты об активности?</span><span class="sxs-lookup"><span data-stu-id="8597f-109">What are activity reports?</span></span>

<span data-ttu-id="8597f-110">Azure AD предоставляет три типа отчетов об активности:</span><span class="sxs-lookup"><span data-stu-id="8597f-110">Azure AD provides three types of activity reports:</span></span>

- <span data-ttu-id="8597f-111">Аудиты каталога</span><span class="sxs-lookup"><span data-stu-id="8597f-111">Directory audits</span></span> 
- <span data-ttu-id="8597f-112">Входы</span><span class="sxs-lookup"><span data-stu-id="8597f-112">Sign-ins</span></span>
- <span data-ttu-id="8597f-113">Подготовка</span><span class="sxs-lookup"><span data-stu-id="8597f-113">Provisioning</span></span>

### <a name="directory-audits"></a><span data-ttu-id="8597f-114">Аудиты каталога</span><span class="sxs-lookup"><span data-stu-id="8597f-114">Directory audits</span></span>

<span data-ttu-id="8597f-115">Отчет аудитов каталога предоставляет доступ к истории всех выполненных задач в клиенте.</span><span class="sxs-lookup"><span data-stu-id="8597f-115">The directory audit report provides you with access to the history of every task performed in your tenant.</span></span> <span data-ttu-id="8597f-116">Отчет аудитов каталога предоставляет записи о действиях системы для обеспечения соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="8597f-116">The directory audit report provides you with records of system activities for compliance.</span></span> <span data-ttu-id="8597f-117">Помимо прочего, предоставляемые данные позволяют рассматривать типичные сценарии, например:</span><span class="sxs-lookup"><span data-stu-id="8597f-117">Amongst others, the provided data enables you to address common scenarios such as:</span></span>

- <span data-ttu-id="8597f-118">Кто предоставил доступ группе администраторов к каталогу пользователя?</span><span class="sxs-lookup"><span data-stu-id="8597f-118">Who granted admin group access to a directory user?</span></span>
- <span data-ttu-id="8597f-119">Какие пользователи входят в недавно приобретенное приложение?</span><span class="sxs-lookup"><span data-stu-id="8597f-119">Which users are signing in to a recently acquired app?</span></span>
- <span data-ttu-id="8597f-120">Сколько сбросов паролей выполнено в каталоге?</span><span class="sxs-lookup"><span data-stu-id="8597f-120">How many passwords resets were made within the directory?</span></span>

### <a name="sign-ins"></a><span data-ttu-id="8597f-121">Входы</span><span class="sxs-lookup"><span data-stu-id="8597f-121">Sign-ins</span></span>

<span data-ttu-id="8597f-122">Отчет о входах помогает определить, кто выполнял задачи, указанные в отчетах аудитов каталога.</span><span class="sxs-lookup"><span data-stu-id="8597f-122">The sign-ins report helps you determine who performed the tasks reported by directory audits.</span></span> <span data-ttu-id="8597f-123">Отчет о входах помогает ответить на представленные ниже вопросы.</span><span class="sxs-lookup"><span data-stu-id="8597f-123">The sign-ins report helps you answer questions like:</span></span>

- <span data-ttu-id="8597f-124">Какой шаблон входа использует пользователь?</span><span class="sxs-lookup"><span data-stu-id="8597f-124">What is the sign in pattern of a user?</span></span>
- <span data-ttu-id="8597f-125">Сколько пользователей выполнило вход за прошлую неделю?</span><span class="sxs-lookup"><span data-stu-id="8597f-125">How many users have signed in during the last week?</span></span>
- <span data-ttu-id="8597f-126">Какое состояние у этих входов?</span><span class="sxs-lookup"><span data-stu-id="8597f-126">What's the status of these sign-ins?</span></span>

### <a name="provisioning"></a><span data-ttu-id="8597f-127">Подготовка</span><span class="sxs-lookup"><span data-stu-id="8597f-127">Provisioning</span></span>

<span data-ttu-id="8597f-128">Отчет о подготовке позволяет просматривать все действия, выполненные службой подготовки Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8597f-128">The provisioning report helps you see all the actions performed by the Azure AD provisioning service.</span></span> <span data-ttu-id="8597f-129">Отчет о подготовке помогает ответить на представленные ниже вопросы.</span><span class="sxs-lookup"><span data-stu-id="8597f-129">The provisioning report helps you answer questions like:</span></span>

- <span data-ttu-id="8597f-130">Какие группы были успешно созданы в ServiceNow?</span><span class="sxs-lookup"><span data-stu-id="8597f-130">What groups were successfully created in ServiceNow?</span></span>
- <span data-ttu-id="8597f-131">Какие роли были импортированы из Amazon Web Services?</span><span class="sxs-lookup"><span data-stu-id="8597f-131">What roles were imported from Amazon Web Services?</span></span>
- <span data-ttu-id="8597f-132">Каких пользователей не удалось создать из Workday?</span><span class="sxs-lookup"><span data-stu-id="8597f-132">What users were unsuccessfully created from Workday?</span></span>

## <a name="what-can-i-do-with-activity-reports-in-microsoft-graph"></a><span data-ttu-id="8597f-133">Как можно использовать отчеты об активности в Microsoft Graph?</span><span class="sxs-lookup"><span data-stu-id="8597f-133">What can I do with activity reports in Microsoft Graph?</span></span>

<span data-ttu-id="8597f-134">Ниже приведены популярные запросы для работы с данными отчетов.</span><span class="sxs-lookup"><span data-stu-id="8597f-134">Here are popular requests for working with report data:</span></span>

<span data-ttu-id="8597f-135">Operation</span><span class="sxs-lookup"><span data-stu-id="8597f-135">Operation</span></span> | <span data-ttu-id="8597f-136">URL-адрес</span><span class="sxs-lookup"><span data-stu-id="8597f-136">URL</span></span>
:----------|:----
<span data-ttu-id="8597f-137">Получение действий пользователей клиента</span><span class="sxs-lookup"><span data-stu-id="8597f-137">GET tenant user activities</span></span> | [https://graph.microsoft.com/beta/auditLogs/directoryAudits](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/directoryAudits&version=beta)
<span data-ttu-id="8597f-138">Получение входов пользователей клиента</span><span class="sxs-lookup"><span data-stu-id="8597f-138">GET tenant user sign-ins</span></span> | [https://graph.microsoft.com/beta/auditLogs/signIns](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/signIns&version=beta)
<span data-ttu-id="8597f-139">Получение журналов подготовки</span><span class="sxs-lookup"><span data-stu-id="8597f-139">GET provisioning logs</span></span> | [https://graph.microsoft.com/beta/auditLogs/provisioning](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/Provisioning&version=beta)

## <a name="what-licenses-do-i-need"></a><span data-ttu-id="8597f-140">Какие лицензии нужны?</span><span class="sxs-lookup"><span data-stu-id="8597f-140">What licenses do I need?</span></span>

<span data-ttu-id="8597f-141">Отчеты об активности доступны для компонентов, на которые у вас есть лицензии.</span><span class="sxs-lookup"><span data-stu-id="8597f-141">Activity reports are available for features that you've licensed.</span></span> <span data-ttu-id="8597f-142">Если у вас есть лицензия на определенный компонент, вам будет предоставлен доступ к соответствующим отчетам.</span><span class="sxs-lookup"><span data-stu-id="8597f-142">If you have a license for a specific feature, you also have access to the reports.</span></span>

<span data-ttu-id="8597f-143">Например, вам нужна лицензия на Azure AD Premium P1, чтобы получить доступ к отчетам аудита самостоятельного изменения паролей.</span><span class="sxs-lookup"><span data-stu-id="8597f-143">For example, you need an Azure AD Premium P1 license to access self-service password audit reports.</span></span>  <span data-ttu-id="8597f-144">Дополнительные сведения см. на странице [лицензий Azure AD](https://azure.microsoft.com/pricing/details/active-directory/).</span><span class="sxs-lookup"><span data-stu-id="8597f-144">To learn more, see [Azure AD licensing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

<span data-ttu-id="8597f-145">Для отчетов входов требуется лицензия на Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="8597f-145">Sign-in reports require an Azure AD Premium license.</span></span>

<span data-ttu-id="8597f-146">Дополнительные сведения см. на странице [Цены на Azure AD](https://azure.microsoft.com/pricing/details/active-directory/).</span><span class="sxs-lookup"><span data-stu-id="8597f-146">To learn more, see [Azure AD pricing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

## <a name="next-steps"></a><span data-ttu-id="8597f-147">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="8597f-147">Next steps</span></span>

- <span data-ttu-id="8597f-148">[Зарегистрируйте приложение](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal), чтобы соответствовать предварительным требованиям отчетов.</span><span class="sxs-lookup"><span data-stu-id="8597f-148">[Register your app](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to satisfy report prerequisites.</span></span> 
- <span data-ttu-id="8597f-149">Сведения о том, как получить журналы аудита при проверке подлинности с помощью сертификатов, см. в [руководстве по получению данных с помощью API отчетов Azure Active Directory с сертификатами](/azure/active-directory/reports-monitoring/tutorial-access-api-with-certificates).</span><span class="sxs-lookup"><span data-stu-id="8597f-149">To learn how to retrieve audit logs while authenticated using certificates, see [Tutorial: Get data using the Azure Active Directory reporting API with certificates](/azure/active-directory/reports-monitoring/tutorial-access-api-with-certificates).</span></span>  
- <span data-ttu-id="8597f-150">Изучите действия и ресурс [directoryAudit](directoryaudit.md).</span><span class="sxs-lookup"><span data-stu-id="8597f-150">Review the [directoryAudit](directoryaudit.md) resource and actions.</span></span>
- <span data-ttu-id="8597f-151">Изучите действия и ресурс [signIn](signin.md).</span><span class="sxs-lookup"><span data-stu-id="8597f-151">Review the [signIn](signin.md) resource and actions.</span></span> 
- <span data-ttu-id="8597f-152">Изучите ресурс [provisioningObjectSummary](provisioningobjectsummary.md).</span><span class="sxs-lookup"><span data-stu-id="8597f-152">Review the [provisioningObjectSummary](provisioningobjectsummary.md) resource.</span></span>
