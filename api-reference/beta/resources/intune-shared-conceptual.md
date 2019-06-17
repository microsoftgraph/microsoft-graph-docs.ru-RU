---
title: Общие ресурсы в Microsoft Intune — API Microsoft Graph
description: Перечисляет API Microsoft Graph для конечных точек Intune (REST), поддерживающих несколько рабочих процессов для организации клиента.
localization_priority: Normal
author: rolyon
ms.prod: intune
ms.openlocfilehash: 2240f8ff55ca2dbcf4e7107495e07b72f95cdfa4
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34996192"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="9c2d4-103">Общие ресурсы в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="9c2d4-103">Shared resources in Microsoft Intune</span></span>

> <span data-ttu-id="9c2d4-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9c2d4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9c2d4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c2d4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9c2d4-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9c2d4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c2d4-107">Эти конечные точки используются в нескольких интерфейсах API Microsoft Graph для рабочих процессов Intune.</span><span class="sxs-lookup"><span data-stu-id="9c2d4-107">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="9c2d4-108">Цель, цель и разрешения, необходимые для использования указанного ресурса, меняются в зависимости от конкретного рабочего процесса и контекста базового вызова.</span><span class="sxs-lookup"><span data-stu-id="9c2d4-108">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="9c2d4-109">Кроме того, некоторые методы, свойства и действия поддерживаются только для определенных рабочих процессов.</span><span class="sxs-lookup"><span data-stu-id="9c2d4-109">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="9c2d4-110">Рабочие процессы Intune совместно работают со следующими ресурсами Graph:</span><span class="sxs-lookup"><span data-stu-id="9c2d4-110">The following Graph resources are shared between Intune workflows:</span></span>

- [<span data-ttu-id="9c2d4-111">Состояние действия</span><span class="sxs-lookup"><span data-stu-id="9c2d4-111">Action state</span></span>](intune-shared-actionstate.md)
- [<span data-ttu-id="9c2d4-112">Объект назначения всех устройств</span><span class="sxs-lookup"><span data-stu-id="9c2d4-112">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="9c2d4-113">Объект назначения всех лицензированных пользователей</span><span class="sxs-lookup"><span data-stu-id="9c2d4-113">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="9c2d4-114">Состояние соответствия</span><span class="sxs-lookup"><span data-stu-id="9c2d4-114">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="9c2d4-115">Объект назначения для управления устройствами и приложениями</span><span class="sxs-lookup"><span data-stu-id="9c2d4-115">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="9c2d4-116">Управление приложениями для устройств</span><span class="sxs-lookup"><span data-stu-id="9c2d4-116">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="9c2d4-117">Категория устройств</span><span class="sxs-lookup"><span data-stu-id="9c2d4-117">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="9c2d4-118">Тип регистрации устройства</span><span class="sxs-lookup"><span data-stu-id="9c2d4-118">Device enrollment type</span></span>](intune-shared-deviceenrollmenttype.md)
- [<span data-ttu-id="9c2d4-119">Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="9c2d4-119">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="9c2d4-120">Тип платформы устройства</span><span class="sxs-lookup"><span data-stu-id="9c2d4-120">Device platform type</span></span>](intune-shared-deviceplatformtype.md)
- [<span data-ttu-id="9c2d4-121">Тип устройства</span><span class="sxs-lookup"><span data-stu-id="9c2d4-121">Device type</span></span>](intune-shared-devicetype.md)
- [<span data-ttu-id="9c2d4-122">Включение</span><span class="sxs-lookup"><span data-stu-id="9c2d4-122">Enablement</span></span>](intune-shared-enablement.md)
- [<span data-ttu-id="9c2d4-123">Объект назначения группы исключения</span><span class="sxs-lookup"><span data-stu-id="9c2d4-123">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="9c2d4-124">Объект назначения группы</span><span class="sxs-lookup"><span data-stu-id="9c2d4-124">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="9c2d4-125">Намерение установки</span><span class="sxs-lookup"><span data-stu-id="9c2d4-125">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="9c2d4-126">Диапазон IP-адресов</span><span class="sxs-lookup"><span data-stu-id="9c2d4-126">IP range</span></span>](intune-shared-iprange.md)
- [<span data-ttu-id="9c2d4-127">Диапазон IPv4-адресов</span><span class="sxs-lookup"><span data-stu-id="9c2d4-127">IPv4 range</span></span>](intune-shared-ipv4range.md)
- [<span data-ttu-id="9c2d4-128">Диапазон IPv6-адресов</span><span class="sxs-lookup"><span data-stu-id="9c2d4-128">IPv6 range</span></span>](intune-shared-ipv6range.md)
- [<span data-ttu-id="9c2d4-129">Пара "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="9c2d4-129">Key/value pair</span></span>](intune-shared-keyvaluepair.md)
- [<span data-ttu-id="9c2d4-130">Содержимое MIME</span><span class="sxs-lookup"><span data-stu-id="9c2d4-130">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="9c2d4-131">Устранение неполадок с мобильным приложением: событие</span><span class="sxs-lookup"><span data-stu-id="9c2d4-131">Mobile app troubleshooting event</span></span>](intune-shared-mobileapptroubleshootingevent.md)
- [<span data-ttu-id="9c2d4-132">Проксируемый домен</span><span class="sxs-lookup"><span data-stu-id="9c2d4-132">Proxied domain</span></span>](intune-shared-proxieddomain.md)
- [<span data-ttu-id="9c2d4-133">Report</span><span class="sxs-lookup"><span data-stu-id="9c2d4-133">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="9c2d4-134">Корневая папка отчета</span><span class="sxs-lookup"><span data-stu-id="9c2d4-134">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="9c2d4-135">Итоговое состояние приложения</span><span class="sxs-lookup"><span data-stu-id="9c2d4-135">Resultant app state</span></span>](intune-shared-resultantappstate.md)
- [<span data-ttu-id="9c2d4-136">Цвет RGB</span><span class="sxs-lookup"><span data-stu-id="9c2d4-136">RGB color</span></span>](intune-shared-rgbcolor.md)
- [<span data-ttu-id="9c2d4-137">Тип учетной записи, от имени которой запускается приложение</span><span class="sxs-lookup"><span data-stu-id="9c2d4-137">Run as account type</span></span>](intune-shared-runasaccounttype.md)
- [<span data-ttu-id="9c2d4-138">Состояние выполнения</span><span class="sxs-lookup"><span data-stu-id="9c2d4-138">Run state</span></span>](intune-shared-runstate.md)
- [<span data-ttu-id="9c2d4-139">Сохраненные параметры создания состояния пользовательского интерфейса</span><span class="sxs-lookup"><span data-stu-id="9c2d4-139">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="9c2d4-140">URI</span><span class="sxs-lookup"><span data-stu-id="9c2d4-140">URI</span></span>](intune-shared-uri.md)
- <span data-ttu-id="9c2d4-141">[пользователь](intune-shared-user.md);</span><span class="sxs-lookup"><span data-stu-id="9c2d4-141">[User](intune-shared-user.md)</span></span>
- [<span data-ttu-id="9c2d4-142">Тип учетной записи токена VPP</span><span class="sxs-lookup"><span data-stu-id="9c2d4-142">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
- [<span data-ttu-id="9c2d4-143">Причина сбоя действия с токеном VPP</span><span class="sxs-lookup"><span data-stu-id="9c2d4-143">VPP token action failure reason</span></span>](intune-shared-vpptokenactionfailurereason.md)
- [<span data-ttu-id="9c2d4-144">Конфигурация присоединения к домену Windows</span><span class="sxs-lookup"><span data-stu-id="9c2d4-144">Windows domain join configuration</span></span>](intune-shared-windowsdomainjoinconfiguration.md)
