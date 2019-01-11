---
title: Общие ресурсы в Microsoft Intune
description: Эти конечные точки используются в нескольких Microsoft Graph API Intune рабочих процессов.  Цель, назначения и разрешения, необходимые для использования указанного ресурса изменяется в зависимости от конкретного рабочего процесса и контекста вызова базового.  Кроме того некоторые методы, свойства и действия поддерживаются только для определенных рабочих процессов.
localization_priority: Normal
ms.openlocfilehash: c381ba84c9240a2b8e7428a3c055b8baf35fb243
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852628"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="6051c-105">Общие ресурсы в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="6051c-105">Shared resources in Microsoft Intune</span></span>

> <span data-ttu-id="6051c-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6051c-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6051c-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6051c-107">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6051c-108">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6051c-108">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="6051c-109">Эти конечные точки используются в нескольких Microsoft Graph API Intune рабочих процессов.</span><span class="sxs-lookup"><span data-stu-id="6051c-109">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="6051c-110">Цель, назначения и разрешения, необходимые для использования указанного ресурса изменяется в зависимости от конкретного рабочего процесса и контекста вызова базового.</span><span class="sxs-lookup"><span data-stu-id="6051c-110">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="6051c-111">Кроме того некоторые методы, свойства и действия поддерживаются только для определенных рабочих процессов.</span><span class="sxs-lookup"><span data-stu-id="6051c-111">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="6051c-112">В следующих ресурсах графике совместно Intune рабочих процессов:</span><span class="sxs-lookup"><span data-stu-id="6051c-112">The following Graph resources are shared between Intune workflows:</span></span>

- [<span data-ttu-id="6051c-113">Состояние действия</span><span class="sxs-lookup"><span data-stu-id="6051c-113">Action state</span></span>](intune-shared-actionstate.md)
- [<span data-ttu-id="6051c-114">Объект назначения всех устройств</span><span class="sxs-lookup"><span data-stu-id="6051c-114">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="6051c-115">Объект назначения всех лицензированных пользователей</span><span class="sxs-lookup"><span data-stu-id="6051c-115">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="6051c-116">Состояние соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="6051c-116">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="6051c-117">Объект назначения для управления устройствами и приложениями</span><span class="sxs-lookup"><span data-stu-id="6051c-117">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="6051c-118">Управление приложениями для устройств</span><span class="sxs-lookup"><span data-stu-id="6051c-118">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="6051c-119">Категория устройств</span><span class="sxs-lookup"><span data-stu-id="6051c-119">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="6051c-120">Тип регистрации устройства</span><span class="sxs-lookup"><span data-stu-id="6051c-120">Device enrollment type</span></span>](intune-shared-deviceenrollmenttype.md)
- [<span data-ttu-id="6051c-121">Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="6051c-121">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="6051c-122">Тип платформы устройства</span><span class="sxs-lookup"><span data-stu-id="6051c-122">Device platform type</span></span>](intune-shared-deviceplatformtype.md)
- [<span data-ttu-id="6051c-123">Тип устройства</span><span class="sxs-lookup"><span data-stu-id="6051c-123">Device type</span></span>](intune-shared-devicetype.md)
- [<span data-ttu-id="6051c-124">Включение</span><span class="sxs-lookup"><span data-stu-id="6051c-124">Enablement</span></span>](intune-shared-enablement.md)
- [<span data-ttu-id="6051c-125">Объект назначения группы исключения</span><span class="sxs-lookup"><span data-stu-id="6051c-125">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="6051c-126">Объект назначения группы</span><span class="sxs-lookup"><span data-stu-id="6051c-126">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="6051c-127">Цель установки</span><span class="sxs-lookup"><span data-stu-id="6051c-127">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="6051c-128">Диапазон IP-адресов</span><span class="sxs-lookup"><span data-stu-id="6051c-128">IP range</span></span>](intune-shared-iprange.md)
- [<span data-ttu-id="6051c-129">Диапазон IPv4-адресов</span><span class="sxs-lookup"><span data-stu-id="6051c-129">IPv4 range</span></span>](intune-shared-ipv4range.md)
- [<span data-ttu-id="6051c-130">Диапазон IPv6-адресов</span><span class="sxs-lookup"><span data-stu-id="6051c-130">IPv6 range</span></span>](intune-shared-ipv6range.md)
- [<span data-ttu-id="6051c-131">Пара "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="6051c-131">Key/value pair</span></span>](intune-shared-keyvaluepair.md)
- [<span data-ttu-id="6051c-132">Содержимое MIME</span><span class="sxs-lookup"><span data-stu-id="6051c-132">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="6051c-133">Проксируемый домен</span><span class="sxs-lookup"><span data-stu-id="6051c-133">Proxied domain</span></span>](intune-shared-proxieddomain.md)
- [<span data-ttu-id="6051c-134">Report</span><span class="sxs-lookup"><span data-stu-id="6051c-134">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="6051c-135">Корневой отчета</span><span class="sxs-lookup"><span data-stu-id="6051c-135">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="6051c-136">Состояния результирующее приложения</span><span class="sxs-lookup"><span data-stu-id="6051c-136">Resultant app state</span></span>](intune-shared-resultantappstate.md)
- [<span data-ttu-id="6051c-137">Цвет RGB</span><span class="sxs-lookup"><span data-stu-id="6051c-137">RGB color</span></span>](intune-shared-rgbcolor.md)
- [<span data-ttu-id="6051c-138">Запуск от имени типа учетной записи</span><span class="sxs-lookup"><span data-stu-id="6051c-138">Run as account type</span></span>](intune-shared-runasaccounttype.md)
- [<span data-ttu-id="6051c-139">Состояние выполнения</span><span class="sxs-lookup"><span data-stu-id="6051c-139">Run state</span></span>](intune-shared-runstate.md)
- [<span data-ttu-id="6051c-140">Сохранить параметры создания состояние пользовательского интерфейса</span><span class="sxs-lookup"><span data-stu-id="6051c-140">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="6051c-141">URI</span><span class="sxs-lookup"><span data-stu-id="6051c-141">URI</span></span>](intune-shared-uri.md)
- <span data-ttu-id="6051c-142">[пользователь](intune-shared-user.md);</span><span class="sxs-lookup"><span data-stu-id="6051c-142">[User](intune-shared-user.md)</span></span>
- [<span data-ttu-id="6051c-143">Тип учетной записи маркеров VPP</span><span class="sxs-lookup"><span data-stu-id="6051c-143">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
- [<span data-ttu-id="6051c-144">Причина сбоя VPP маркеров действие</span><span class="sxs-lookup"><span data-stu-id="6051c-144">VPP token action failure reason</span></span>](intune-shared-vpptokenactionfailurereason.md)
- [<span data-ttu-id="6051c-145">Конфигурация join домена Windows</span><span class="sxs-lookup"><span data-stu-id="6051c-145">Windows domain join configuration</span></span>](intune-shared-windowsdomainjoinconfiguration.md)
