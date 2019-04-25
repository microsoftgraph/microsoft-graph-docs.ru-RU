---
title: Общие ресурсы в Microsoft Intune — API Microsoft Graph
description: Перечисляет API Microsoft Graph для конечных точек Intune (REST), поддерживающих несколько рабочих процессов для организации клиента.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 6436f134ae9e95623b073f6e645f0737d45d540e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566285"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="0a4ba-103">Общие ресурсы в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="0a4ba-103">Shared resources in Microsoft Intune</span></span>

> <span data-ttu-id="0a4ba-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0a4ba-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0a4ba-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a4ba-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0a4ba-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0a4ba-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="0a4ba-107">Эти конечные точки используются в нескольких ИНТЕРФЕЙСах API Microsoft Graph для рабочих процессов Intune.</span><span class="sxs-lookup"><span data-stu-id="0a4ba-107">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="0a4ba-108">Цель, цель и разрешения, необходимые для использования указанного ресурса, меняются в зависимости от конкретного рабочего процесса и контекста базового вызова.</span><span class="sxs-lookup"><span data-stu-id="0a4ba-108">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="0a4ba-109">Кроме того, некоторые методы, свойства и действия поддерживаются только для определенных рабочих процессов.</span><span class="sxs-lookup"><span data-stu-id="0a4ba-109">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="0a4ba-110">Рабочие процессы Intune совместно работают со следующими ресурсами Graph:</span><span class="sxs-lookup"><span data-stu-id="0a4ba-110">The following Graph resources are shared between Intune workflows:</span></span>

- [<span data-ttu-id="0a4ba-111">Состояние действия</span><span class="sxs-lookup"><span data-stu-id="0a4ba-111">Action state</span></span>](intune-shared-actionstate.md)
- [<span data-ttu-id="0a4ba-112">Объект назначения всех устройств</span><span class="sxs-lookup"><span data-stu-id="0a4ba-112">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="0a4ba-113">Объект назначения всех лицензированных пользователей</span><span class="sxs-lookup"><span data-stu-id="0a4ba-113">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="0a4ba-114">Состояние соответствия</span><span class="sxs-lookup"><span data-stu-id="0a4ba-114">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="0a4ba-115">Объект назначения для управления устройствами и приложениями</span><span class="sxs-lookup"><span data-stu-id="0a4ba-115">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="0a4ba-116">Управление приложениями для устройств</span><span class="sxs-lookup"><span data-stu-id="0a4ba-116">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="0a4ba-117">Категория устройств</span><span class="sxs-lookup"><span data-stu-id="0a4ba-117">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="0a4ba-118">Тип регистрации устройства</span><span class="sxs-lookup"><span data-stu-id="0a4ba-118">Device enrollment type</span></span>](intune-shared-deviceenrollmenttype.md)
- [<span data-ttu-id="0a4ba-119">Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="0a4ba-119">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="0a4ba-120">Тип платформы устройства</span><span class="sxs-lookup"><span data-stu-id="0a4ba-120">Device platform type</span></span>](intune-shared-deviceplatformtype.md)
- [<span data-ttu-id="0a4ba-121">Тип устройства</span><span class="sxs-lookup"><span data-stu-id="0a4ba-121">Device type</span></span>](intune-shared-devicetype.md)
- [<span data-ttu-id="0a4ba-122">Включение</span><span class="sxs-lookup"><span data-stu-id="0a4ba-122">Enablement</span></span>](intune-shared-enablement.md)
- [<span data-ttu-id="0a4ba-123">Объект назначения группы исключения</span><span class="sxs-lookup"><span data-stu-id="0a4ba-123">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="0a4ba-124">Объект назначения группы</span><span class="sxs-lookup"><span data-stu-id="0a4ba-124">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="0a4ba-125">Намерение установки</span><span class="sxs-lookup"><span data-stu-id="0a4ba-125">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="0a4ba-126">Диапазон IP-адресов</span><span class="sxs-lookup"><span data-stu-id="0a4ba-126">IP range</span></span>](intune-shared-iprange.md)
- [<span data-ttu-id="0a4ba-127">Диапазон IPv4-адресов</span><span class="sxs-lookup"><span data-stu-id="0a4ba-127">IPv4 range</span></span>](intune-shared-ipv4range.md)
- [<span data-ttu-id="0a4ba-128">Диапазон IPv6-адресов</span><span class="sxs-lookup"><span data-stu-id="0a4ba-128">IPv6 range</span></span>](intune-shared-ipv6range.md)
- [<span data-ttu-id="0a4ba-129">Пара "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="0a4ba-129">Key/value pair</span></span>](intune-shared-keyvaluepair.md)
- [<span data-ttu-id="0a4ba-130">Содержимое MIME</span><span class="sxs-lookup"><span data-stu-id="0a4ba-130">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="0a4ba-131">Устранение неполадок с мобильным приложением: событие</span><span class="sxs-lookup"><span data-stu-id="0a4ba-131">Mobile app troubleshooting event</span></span>](intune-shared-mobileapptroubleshootingevent.md)
- [<span data-ttu-id="0a4ba-132">Проксируемый домен</span><span class="sxs-lookup"><span data-stu-id="0a4ba-132">Proxied domain</span></span>](intune-shared-proxieddomain.md)
- [<span data-ttu-id="0a4ba-133">Report</span><span class="sxs-lookup"><span data-stu-id="0a4ba-133">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="0a4ba-134">Корневая папка отчета</span><span class="sxs-lookup"><span data-stu-id="0a4ba-134">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="0a4ba-135">Итоговое состояние приложения</span><span class="sxs-lookup"><span data-stu-id="0a4ba-135">Resultant app state</span></span>](intune-shared-resultantappstate.md)
- [<span data-ttu-id="0a4ba-136">Цвет RGB</span><span class="sxs-lookup"><span data-stu-id="0a4ba-136">RGB color</span></span>](intune-shared-rgbcolor.md)
- [<span data-ttu-id="0a4ba-137">Тип учетной записи, от имени которой запускается приложение</span><span class="sxs-lookup"><span data-stu-id="0a4ba-137">Run as account type</span></span>](intune-shared-runasaccounttype.md)
- [<span data-ttu-id="0a4ba-138">Состояние выполнения</span><span class="sxs-lookup"><span data-stu-id="0a4ba-138">Run state</span></span>](intune-shared-runstate.md)
- [<span data-ttu-id="0a4ba-139">Сохраненные параметры создания состояния пользовательского интерфейса</span><span class="sxs-lookup"><span data-stu-id="0a4ba-139">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="0a4ba-140">URI</span><span class="sxs-lookup"><span data-stu-id="0a4ba-140">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="0a4ba-141">Пользователь</span><span class="sxs-lookup"><span data-stu-id="0a4ba-141">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="0a4ba-142">Тип учетной записи токена VPP</span><span class="sxs-lookup"><span data-stu-id="0a4ba-142">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
- [<span data-ttu-id="0a4ba-143">Причина сбоя действия с токеном VPP</span><span class="sxs-lookup"><span data-stu-id="0a4ba-143">VPP token action failure reason</span></span>](intune-shared-vpptokenactionfailurereason.md)
- [<span data-ttu-id="0a4ba-144">Конфигурация присоединения к домену Windows</span><span class="sxs-lookup"><span data-stu-id="0a4ba-144">Windows domain join configuration</span></span>](intune-shared-windowsdomainjoinconfiguration.md)
