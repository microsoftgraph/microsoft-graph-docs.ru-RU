---
title: Общие ресурсы в Microsoft Intune — API Microsoft Graph
description: Перечисляет API Microsoft Graph для конечных точек Intune (REST), поддерживающих несколько рабочих процессов для организации клиента.
localization_priority: Normal
author: rolyon
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: c8540b7bd183d21a15ad2e38b5f1bef2caa4d983
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010534"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="7d891-103">Общие ресурсы в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="7d891-103">Shared resources in Microsoft Intune</span></span>

> <span data-ttu-id="7d891-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7d891-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7d891-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d891-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7d891-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7d891-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d891-107">Эти конечные точки используются в нескольких интерфейсах API Microsoft Graph для рабочих процессов Intune.</span><span class="sxs-lookup"><span data-stu-id="7d891-107">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="7d891-108">Цель, цель и разрешения, необходимые для использования указанного ресурса, меняются в зависимости от конкретного рабочего процесса и контекста базового вызова.</span><span class="sxs-lookup"><span data-stu-id="7d891-108">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="7d891-109">Кроме того, некоторые методы, свойства и действия поддерживаются только для определенных рабочих процессов.</span><span class="sxs-lookup"><span data-stu-id="7d891-109">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="7d891-110">Рабочие процессы Intune совместно работают со следующими ресурсами Graph:</span><span class="sxs-lookup"><span data-stu-id="7d891-110">The following Graph resources are shared between Intune workflows:</span></span>

- [<span data-ttu-id="7d891-111">Состояние действия</span><span class="sxs-lookup"><span data-stu-id="7d891-111">Action state</span></span>](intune-shared-actionstate.md)
- [<span data-ttu-id="7d891-112">Объект назначения всех устройств</span><span class="sxs-lookup"><span data-stu-id="7d891-112">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="7d891-113">Объект назначения всех лицензированных пользователей</span><span class="sxs-lookup"><span data-stu-id="7d891-113">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="7d891-114">Состояние соответствия</span><span class="sxs-lookup"><span data-stu-id="7d891-114">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="7d891-115">Объект назначения для управления устройствами и приложениями</span><span class="sxs-lookup"><span data-stu-id="7d891-115">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="7d891-116">Управление приложениями для устройств</span><span class="sxs-lookup"><span data-stu-id="7d891-116">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="7d891-117">Категория устройств</span><span class="sxs-lookup"><span data-stu-id="7d891-117">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="7d891-118">Тип регистрации устройства</span><span class="sxs-lookup"><span data-stu-id="7d891-118">Device enrollment type</span></span>](intune-shared-deviceenrollmenttype.md)
- [<span data-ttu-id="7d891-119">Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="7d891-119">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="7d891-120">Тип платформы устройства</span><span class="sxs-lookup"><span data-stu-id="7d891-120">Device platform type</span></span>](intune-shared-deviceplatformtype.md)
- [<span data-ttu-id="7d891-121">Тип устройства</span><span class="sxs-lookup"><span data-stu-id="7d891-121">Device type</span></span>](intune-shared-devicetype.md)
- [<span data-ttu-id="7d891-122">Включение</span><span class="sxs-lookup"><span data-stu-id="7d891-122">Enablement</span></span>](intune-shared-enablement.md)
- [<span data-ttu-id="7d891-123">Объект назначения группы исключения</span><span class="sxs-lookup"><span data-stu-id="7d891-123">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="7d891-124">Объект назначения группы</span><span class="sxs-lookup"><span data-stu-id="7d891-124">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="7d891-125">Намерение установки</span><span class="sxs-lookup"><span data-stu-id="7d891-125">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="7d891-126">Диапазон IP-адресов</span><span class="sxs-lookup"><span data-stu-id="7d891-126">IP range</span></span>](intune-shared-iprange.md)
- [<span data-ttu-id="7d891-127">Диапазон IPv4-адресов</span><span class="sxs-lookup"><span data-stu-id="7d891-127">IPv4 range</span></span>](intune-shared-ipv4range.md)
- [<span data-ttu-id="7d891-128">Диапазон IPv6-адресов</span><span class="sxs-lookup"><span data-stu-id="7d891-128">IPv6 range</span></span>](intune-shared-ipv6range.md)
- [<span data-ttu-id="7d891-129">Пара "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="7d891-129">Key/value pair</span></span>](intune-shared-keyvaluepair.md)
- [<span data-ttu-id="7d891-130">Содержимое MIME</span><span class="sxs-lookup"><span data-stu-id="7d891-130">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="7d891-131">Устранение неполадок с мобильным приложением: событие</span><span class="sxs-lookup"><span data-stu-id="7d891-131">Mobile app troubleshooting event</span></span>](intune-shared-mobileapptroubleshootingevent.md)
- [<span data-ttu-id="7d891-132">Проксируемый домен</span><span class="sxs-lookup"><span data-stu-id="7d891-132">Proxied domain</span></span>](intune-shared-proxieddomain.md)
- [<span data-ttu-id="7d891-133">Report</span><span class="sxs-lookup"><span data-stu-id="7d891-133">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="7d891-134">Корневая папка отчета</span><span class="sxs-lookup"><span data-stu-id="7d891-134">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="7d891-135">Итоговое состояние приложения</span><span class="sxs-lookup"><span data-stu-id="7d891-135">Resultant app state</span></span>](intune-shared-resultantappstate.md)
- [<span data-ttu-id="7d891-136">Цвет RGB</span><span class="sxs-lookup"><span data-stu-id="7d891-136">RGB color</span></span>](intune-shared-rgbcolor.md)
- [<span data-ttu-id="7d891-137">Тип учетной записи, от имени которой запускается приложение</span><span class="sxs-lookup"><span data-stu-id="7d891-137">Run as account type</span></span>](intune-shared-runasaccounttype.md)
- [<span data-ttu-id="7d891-138">Состояние выполнения</span><span class="sxs-lookup"><span data-stu-id="7d891-138">Run state</span></span>](intune-shared-runstate.md)
- [<span data-ttu-id="7d891-139">Сохраненные параметры создания состояния пользовательского интерфейса</span><span class="sxs-lookup"><span data-stu-id="7d891-139">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="7d891-140">URI</span><span class="sxs-lookup"><span data-stu-id="7d891-140">URI</span></span>](intune-shared-uri.md)
- <span data-ttu-id="7d891-141">[пользователь](intune-shared-user.md);</span><span class="sxs-lookup"><span data-stu-id="7d891-141">[User](intune-shared-user.md)</span></span>
- [<span data-ttu-id="7d891-142">Тип учетной записи токена VPP</span><span class="sxs-lookup"><span data-stu-id="7d891-142">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
- [<span data-ttu-id="7d891-143">Причина сбоя действия с токеном VPP</span><span class="sxs-lookup"><span data-stu-id="7d891-143">VPP token action failure reason</span></span>](intune-shared-vpptokenactionfailurereason.md)
- [<span data-ttu-id="7d891-144">Конфигурация присоединения к домену Windows</span><span class="sxs-lookup"><span data-stu-id="7d891-144">Windows domain join configuration</span></span>](intune-shared-windowsdomainjoinconfiguration.md)
