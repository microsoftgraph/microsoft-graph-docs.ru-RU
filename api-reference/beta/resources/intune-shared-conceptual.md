---
title: Общие ресурсы в Microsoft Intune — API Microsoft Graph
description: Перечисляет API Microsoft Graph для конечных точек Intune (REST), поддерживающих несколько рабочих процессов для организации клиента.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 6436f134ae9e95623b073f6e645f0737d45d540e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158312"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="5a8d8-103">Общие ресурсы в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="5a8d8-103">Shared resources in Microsoft Intune</span></span>

> <span data-ttu-id="5a8d8-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5a8d8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5a8d8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a8d8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5a8d8-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5a8d8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="5a8d8-107">Эти конечные точки используются в нескольких ИНТЕРФЕЙСах API Microsoft Graph для рабочих процессов Intune.</span><span class="sxs-lookup"><span data-stu-id="5a8d8-107">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="5a8d8-108">Цель, цель и разрешения, необходимые для использования указанного ресурса, меняются в зависимости от конкретного рабочего процесса и контекста базового вызова.</span><span class="sxs-lookup"><span data-stu-id="5a8d8-108">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="5a8d8-109">Кроме того, некоторые методы, свойства и действия поддерживаются только для определенных рабочих процессов.</span><span class="sxs-lookup"><span data-stu-id="5a8d8-109">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="5a8d8-110">Рабочие процессы Intune совместно работают со следующими ресурсами Graph:</span><span class="sxs-lookup"><span data-stu-id="5a8d8-110">The following Graph resources are shared between Intune workflows:</span></span>

- [<span data-ttu-id="5a8d8-111">Состояние действия</span><span class="sxs-lookup"><span data-stu-id="5a8d8-111">Action state</span></span>](intune-shared-actionstate.md)
- [<span data-ttu-id="5a8d8-112">Объект назначения всех устройств</span><span class="sxs-lookup"><span data-stu-id="5a8d8-112">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="5a8d8-113">Объект назначения всех лицензированных пользователей</span><span class="sxs-lookup"><span data-stu-id="5a8d8-113">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="5a8d8-114">Состояние соответствия</span><span class="sxs-lookup"><span data-stu-id="5a8d8-114">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="5a8d8-115">Объект назначения для управления устройствами и приложениями</span><span class="sxs-lookup"><span data-stu-id="5a8d8-115">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="5a8d8-116">Управление приложениями для устройств</span><span class="sxs-lookup"><span data-stu-id="5a8d8-116">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="5a8d8-117">Категория устройств</span><span class="sxs-lookup"><span data-stu-id="5a8d8-117">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="5a8d8-118">Тип регистрации устройства</span><span class="sxs-lookup"><span data-stu-id="5a8d8-118">Device enrollment type</span></span>](intune-shared-deviceenrollmenttype.md)
- [<span data-ttu-id="5a8d8-119">Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="5a8d8-119">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="5a8d8-120">Тип платформы устройства</span><span class="sxs-lookup"><span data-stu-id="5a8d8-120">Device platform type</span></span>](intune-shared-deviceplatformtype.md)
- [<span data-ttu-id="5a8d8-121">Тип устройства</span><span class="sxs-lookup"><span data-stu-id="5a8d8-121">Device type</span></span>](intune-shared-devicetype.md)
- [<span data-ttu-id="5a8d8-122">Включение</span><span class="sxs-lookup"><span data-stu-id="5a8d8-122">Enablement</span></span>](intune-shared-enablement.md)
- [<span data-ttu-id="5a8d8-123">Объект назначения группы исключения</span><span class="sxs-lookup"><span data-stu-id="5a8d8-123">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="5a8d8-124">Объект назначения группы</span><span class="sxs-lookup"><span data-stu-id="5a8d8-124">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="5a8d8-125">Намерение установки</span><span class="sxs-lookup"><span data-stu-id="5a8d8-125">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="5a8d8-126">Диапазон IP-адресов</span><span class="sxs-lookup"><span data-stu-id="5a8d8-126">IP range</span></span>](intune-shared-iprange.md)
- [<span data-ttu-id="5a8d8-127">Диапазон IPv4-адресов</span><span class="sxs-lookup"><span data-stu-id="5a8d8-127">IPv4 range</span></span>](intune-shared-ipv4range.md)
- [<span data-ttu-id="5a8d8-128">Диапазон IPv6-адресов</span><span class="sxs-lookup"><span data-stu-id="5a8d8-128">IPv6 range</span></span>](intune-shared-ipv6range.md)
- [<span data-ttu-id="5a8d8-129">Пара "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="5a8d8-129">Key/value pair</span></span>](intune-shared-keyvaluepair.md)
- [<span data-ttu-id="5a8d8-130">Содержимое MIME</span><span class="sxs-lookup"><span data-stu-id="5a8d8-130">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="5a8d8-131">Устранение неполадок с мобильным приложением: событие</span><span class="sxs-lookup"><span data-stu-id="5a8d8-131">Mobile app troubleshooting event</span></span>](intune-shared-mobileapptroubleshootingevent.md)
- [<span data-ttu-id="5a8d8-132">Проксируемый домен</span><span class="sxs-lookup"><span data-stu-id="5a8d8-132">Proxied domain</span></span>](intune-shared-proxieddomain.md)
- [<span data-ttu-id="5a8d8-133">Report</span><span class="sxs-lookup"><span data-stu-id="5a8d8-133">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="5a8d8-134">Корневая папка отчета</span><span class="sxs-lookup"><span data-stu-id="5a8d8-134">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="5a8d8-135">Итоговое состояние приложения</span><span class="sxs-lookup"><span data-stu-id="5a8d8-135">Resultant app state</span></span>](intune-shared-resultantappstate.md)
- [<span data-ttu-id="5a8d8-136">Цвет RGB</span><span class="sxs-lookup"><span data-stu-id="5a8d8-136">RGB color</span></span>](intune-shared-rgbcolor.md)
- [<span data-ttu-id="5a8d8-137">Тип учетной записи, от имени которой запускается приложение</span><span class="sxs-lookup"><span data-stu-id="5a8d8-137">Run as account type</span></span>](intune-shared-runasaccounttype.md)
- [<span data-ttu-id="5a8d8-138">Состояние выполнения</span><span class="sxs-lookup"><span data-stu-id="5a8d8-138">Run state</span></span>](intune-shared-runstate.md)
- [<span data-ttu-id="5a8d8-139">Сохраненные параметры создания состояния пользовательского интерфейса</span><span class="sxs-lookup"><span data-stu-id="5a8d8-139">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="5a8d8-140">URI</span><span class="sxs-lookup"><span data-stu-id="5a8d8-140">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="5a8d8-141">user</span><span class="sxs-lookup"><span data-stu-id="5a8d8-141">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="5a8d8-142">Тип учетной записи токена VPP</span><span class="sxs-lookup"><span data-stu-id="5a8d8-142">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
- [<span data-ttu-id="5a8d8-143">Причина сбоя действия с токеном VPP</span><span class="sxs-lookup"><span data-stu-id="5a8d8-143">VPP token action failure reason</span></span>](intune-shared-vpptokenactionfailurereason.md)
- [<span data-ttu-id="5a8d8-144">Конфигурация присоединения к домену Windows</span><span class="sxs-lookup"><span data-stu-id="5a8d8-144">Windows domain join configuration</span></span>](intune-shared-windowsdomainjoinconfiguration.md)
