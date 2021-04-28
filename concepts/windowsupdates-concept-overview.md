---
title: Windows обновления API обзор
description: Служба Windows обновления для бизнеса предоставляет вашей организации контроль над обновлениями, предлагаемыми на устройствах.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 98b75f278e33f56cf726a18c266000b06d817a6f
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067728"
---
# <a name="windows-updates-api-overview"></a><span data-ttu-id="1803c-103">Windows обновления API обзор</span><span class="sxs-lookup"><span data-stu-id="1803c-103">Windows updates API overview</span></span>

<span data-ttu-id="1803c-104">Служба Windows обновления для бизнеса обеспечивает контроль над обновлениями устройств с помощью возможности утверждения, расписания и защиты контента, доставленного Windows Update.</span><span class="sxs-lookup"><span data-stu-id="1803c-104">The Windows Update for Business deployment service provides control over device updates through the ability to approve, schedule and safeguard content delivered by Windows Update.</span></span> 

## <a name="why-use-the-windows-update-for-business-deployment-service"></a><span data-ttu-id="1803c-105">Зачем использовать службу обновления Windows для бизнеса?</span><span class="sxs-lookup"><span data-stu-id="1803c-105">Why use the Windows Update for Business deployment service?</span></span>

<span data-ttu-id="1803c-106">ИТ-специалисты и поставщики средств управления могут использовать службу развертывания для:</span><span class="sxs-lookup"><span data-stu-id="1803c-106">IT Professionals and management tool vendors alike can use the deployment service to:</span></span>
* <span data-ttu-id="1803c-107">Расписание развертывания обновлений для начала в определенную дату</span><span class="sxs-lookup"><span data-stu-id="1803c-107">Schedule update deployments to begin on a specific date</span></span>
* <span data-ttu-id="1803c-108">Поэтапное развертывание в течение нескольких дней или недель с использованием насыщенных выражений</span><span class="sxs-lookup"><span data-stu-id="1803c-108">Stage deployments over a period of days or weeks using rich expressions</span></span>
* <span data-ttu-id="1803c-109">Обход предварительно настроенных Windows для бизнес-политик, чтобы немедленно развернуть обновление безопасности</span><span class="sxs-lookup"><span data-stu-id="1803c-109">Bypass pre-configured Windows Update for Business policies to immediately deploy a security update</span></span>
* <span data-ttu-id="1803c-110">Обеспечение охвата оборудования и программного обеспечения в организации с помощью развертывания, адаптированного к уникальной популяции устройств (s)</span><span class="sxs-lookup"><span data-stu-id="1803c-110">Ensure coverage of hardware and software in your organization through deployments tailored to unique device population(s)</span></span>

<span data-ttu-id="1803c-111">Сегодня служба развертывания поддерживает управление обновлениями Windows 10 и ускорение Windows 10 безопасности.</span><span class="sxs-lookup"><span data-stu-id="1803c-111">Today, the deployment service supports managing Windows 10 feature updates and expediting Windows 10 security updates.</span></span> <span data-ttu-id="1803c-112">Дополнительные сведения о службе развертывания в контексте Windows для бизнеса см. в [обзоре службы развертывания.](https://docs.microsoft.com/windows/deployment/update/deployment-service-overview)</span><span class="sxs-lookup"><span data-stu-id="1803c-112">To learn more about the deployment service in the context of Windows Update for Business, please see [Overview of the deployment service](https://docs.microsoft.com/windows/deployment/update/deployment-service-overview).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1803c-113">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="1803c-113">Prerequisites</span></span>    

<span data-ttu-id="1803c-114">Чтобы использовать службу развертывания, организация должна иметь одну из следующих подписок:</span><span class="sxs-lookup"><span data-stu-id="1803c-114">To use the deployment service, your organization must have one of the following subscriptions:</span></span>
* <span data-ttu-id="1803c-115">Windows 10 Корпоративная E3 или E5 (входит в Microsoft 365 F3, E3 или E5)</span><span class="sxs-lookup"><span data-stu-id="1803c-115">Windows 10 Enterprise E3 or E5 (included in Microsoft 365 F3, E3, or E5)</span></span>
* <span data-ttu-id="1803c-116">Windows 10 для образовательных учреждений A3 или A5 (входит в Microsoft 365 A3 или A5)</span><span class="sxs-lookup"><span data-stu-id="1803c-116">Windows 10 Education A3 or A5 (included in Microsoft 365 A3 or A5)</span></span>
* <span data-ttu-id="1803c-117">Windows Виртуальный настольный доступ E3 или E5</span><span class="sxs-lookup"><span data-stu-id="1803c-117">Windows Virtual Desktop Access E3 or E5</span></span>
* <span data-ttu-id="1803c-118">Microsoft 365 бизнес премиум</span><span class="sxs-lookup"><span data-stu-id="1803c-118">Microsoft 365 Business Premium</span></span>

<span data-ttu-id="1803c-119">Кроме того, устройства, управляемые службой развертывания, должны:</span><span class="sxs-lookup"><span data-stu-id="1803c-119">Additionally, devices managed by the deployment service must:</span></span>
* <span data-ttu-id="1803c-120">Присоединить Azure AD или к гибридной AD</span><span class="sxs-lookup"><span data-stu-id="1803c-120">Be Azure AD joined or Hybrid AD joined</span></span>
* <span data-ttu-id="1803c-121">Запустите одно из следующих Windows 10: Windows 10 Pro, Windows 10 Корпоративная, Windows 10 для образовательных учреждений, Windows 10 Pro для образовательных учреждений</span><span class="sxs-lookup"><span data-stu-id="1803c-121">Run one of the following Windows 10 editions: Windows 10 Pro, Windows 10 Enterprise, Windows 10 Education, Windows 10 Pro Education</span></span>
* <span data-ttu-id="1803c-122">Установлены Windows 10 версии 1709 или более поздней версии</span><span class="sxs-lookup"><span data-stu-id="1803c-122">Have installed Windows 10 version 1709 or later</span></span>

## <a name="enroll-devices-to-be-managed"></a><span data-ttu-id="1803c-123">Регистрация устройств, которыми необходимо управлять</span><span class="sxs-lookup"><span data-stu-id="1803c-123">Enroll devices to be managed</span></span>

<span data-ttu-id="1803c-124">Чтобы начать использовать службу развертывания, [зарегистрив устройства в управлении обновлениями.](windowsupdates-enroll.md)</span><span class="sxs-lookup"><span data-stu-id="1803c-124">To start using the deployment service, [enroll devices in update management](windowsupdates-enroll.md).</span></span>

## <a name="approve-and-schedule-windows-content-delivered-from-windows-update"></a><span data-ttu-id="1803c-125">Утверждение и расписание Windows, доставленных из Windows Update</span><span class="sxs-lookup"><span data-stu-id="1803c-125">Approve and schedule Windows content delivered from Windows Update</span></span>

<span data-ttu-id="1803c-126">Служба развертывания упрощает проверку, согласование, планирование и развертывание контента для разнообразной экосистемы устройств.</span><span class="sxs-lookup"><span data-stu-id="1803c-126">The deployment service simplifies reviewing, approving, scheduling, and deploying content for a diverse device ecosystem.</span></span> <span data-ttu-id="1803c-127">Каталог обновлений существует, чтобы предоставить представление, адаптированное для утверждений, помогая сосредоточиться на важных решениях по утверждению и избегая необходимости сортировки глубоких списков связанных обновлений.</span><span class="sxs-lookup"><span data-stu-id="1803c-127">An updates catalog exists to provide a view tailored for approvals, helping you focus on approval decisions that matter and avoiding the need to sort through deep lists of related updates.</span></span>

<span data-ttu-id="1803c-128">После развертывания обновления можно запланировать развертывание в будущем или развернуть в течение определенного периода времени.</span><span class="sxs-lookup"><span data-stu-id="1803c-128">Once you choose an update to deploy, you can schedule deployments to start at a future time, or deploy over a period of time.</span></span> <span data-ttu-id="1803c-129">Если вы решите развернуть обновление в течение определенного периода времени, служба развертывания автоматически оптимизирует порядок, в котором устройствам предлагаются обновления.</span><span class="sxs-lookup"><span data-stu-id="1803c-129">If you choose to deploy an update over a period of time, the deployment service automatically optimizes the order in which devices are offered updates.</span></span> <span data-ttu-id="1803c-130">По возможности службы заказов устройств, чтобы убедиться, что разнообразие аппаратных и программных активов представлены на ранних стадиях развертывания, чтобы свести к минимуму количество устройств, которые могут столкнуться с неожиданной проблемой обновления.</span><span class="sxs-lookup"><span data-stu-id="1803c-130">When possible, the service orders devices to ensure that a diversity of hardware and software assets are represented early in the deployment to minimize the number of devices that may encounter an unexpected update issue.</span></span> 

<span data-ttu-id="1803c-131">Дополнительные информацию о службе развертывания:</span><span class="sxs-lookup"><span data-stu-id="1803c-131">Learn more about the deployment service:</span></span>
* [<span data-ttu-id="1803c-132">Обновления программного обеспечения</span><span class="sxs-lookup"><span data-stu-id="1803c-132">Software updates</span></span>](windowsupdates-software-updates.md)
* [<span data-ttu-id="1803c-133">Развертывания</span><span class="sxs-lookup"><span data-stu-id="1803c-133">Deployments</span></span>](windowsupdates-deployments.md)
* [<span data-ttu-id="1803c-134">Расписание развертывания</span><span class="sxs-lookup"><span data-stu-id="1803c-134">Schedule a deployment</span></span>](windowsupdates-schedule-deployment.md)

## <a name="immediately-deploy-an-update-when-critical-needs-arise"></a><span data-ttu-id="1803c-135">Немедленно развертывание обновления при необходимости</span><span class="sxs-lookup"><span data-stu-id="1803c-135">Immediately deploy an update when critical needs arise</span></span>

<span data-ttu-id="1803c-136">В случае критической проблемы с безопасностью можно использовать службу развертывания, чтобы обойти стандартную политику обновления и ускорить развертывание обновления безопасности.</span><span class="sxs-lookup"><span data-stu-id="1803c-136">In the case of a critical security issue, you can use the deployment service to bypass a standard update policy and expedite deployment of a security update.</span></span>

<span data-ttu-id="1803c-137">Дополнительные новости см. в [статью Развертывание ускоренного обновления безопасности.](windowsupdates-deploy-expedited-update.md)</span><span class="sxs-lookup"><span data-stu-id="1803c-137">To learn more, see [Deploy an expedited security update](windowsupdates-deploy-expedited-update.md).</span></span>

## <a name="protect-devices-by-default"></a><span data-ttu-id="1803c-138">Защита устройств по умолчанию</span><span class="sxs-lookup"><span data-stu-id="1803c-138">Protect devices by default</span></span>

<span data-ttu-id="1803c-139">Пользуйтеся [преимуществами](https://docs.microsoft.com/windows/deployment/update/safeguard-holds) защитных удерживающих устройств, которые мешают устройствам с проблемой качества или совместимости устанавливать обновление, что в противном случае приводит к сбою или откату.</span><span class="sxs-lookup"><span data-stu-id="1803c-139">Enjoy the benefit of [safeguard holds](https://docs.microsoft.com/windows/deployment/update/safeguard-holds) which prevent devices with a quality or compatibility issue from installing an update, resulting in failure or rollback otherwise.</span></span>

<span data-ttu-id="1803c-140">Кроме того, можно настроить правила мониторинга, уникальные для вашей организации.</span><span class="sxs-lookup"><span data-stu-id="1803c-140">Additionally, you can configure monitoring rules that are unique to your organization.</span></span> <span data-ttu-id="1803c-141">Эти правила могут отправить оповещение или приостановить развертывание на основе таких сигналов устройства, как откаты.</span><span class="sxs-lookup"><span data-stu-id="1803c-141">These rules can send an alert or pause a deployment based on device signals such as rollbacks.</span></span>

<span data-ttu-id="1803c-142">Дополнительные данные см. в [см. в "Управление правилами мониторинга развертывания".](windowsupdates-manage-monitoring-rules.md)</span><span class="sxs-lookup"><span data-stu-id="1803c-142">To learn more, see [Manage monitoring rules for a deployment](windowsupdates-manage-monitoring-rules.md).</span></span>

## <a name="api-reference"></a><span data-ttu-id="1803c-143">Справочные материалы по API</span><span class="sxs-lookup"><span data-stu-id="1803c-143">API reference</span></span>

<span data-ttu-id="1803c-144">Ищете справочные материалы по API для этой службы?</span><span class="sxs-lookup"><span data-stu-id="1803c-144">Looking for the API reference for this service?</span></span>

<span data-ttu-id="1803c-145">См. [Windows API обновлений в бета Graph Microsoft.](/graph/api/resources/windowsupdates-updates?view=graph-rest-beta&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="1803c-145">See [Windows updates API in Microsoft Graph beta](/graph/api/resources/windowsupdates-updates?view=graph-rest-beta&preserve-view=true).</span></span>
