---
title: Общие ресурсы в Microsoft Intune
description: Эти конечные точки используются в нескольких интерфейсах API Microsoft Graph для рабочих процессов Intune.  Цель, цель и разрешения, необходимые для использования указанного ресурса, меняются в зависимости от конкретного рабочего процесса и контекста базового вызова.  Кроме того, некоторые методы, свойства и действия поддерживаются только для определенных рабочих процессов.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: cc5cbf0f96d3c9199ecd9b622d9724ec10dd472e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037656"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="aed22-105">Общие ресурсы в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="aed22-105">Shared resources in Microsoft Intune</span></span>

<span data-ttu-id="aed22-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aed22-106">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aed22-107">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="aed22-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="aed22-108">Эти конечные точки используются в нескольких интерфейсах API Microsoft Graph для рабочих процессов Intune.</span><span class="sxs-lookup"><span data-stu-id="aed22-108">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="aed22-109">Цель, цель и разрешения, необходимые для использования указанного ресурса, меняются в зависимости от конкретного рабочего процесса и контекста базового вызова.</span><span class="sxs-lookup"><span data-stu-id="aed22-109">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="aed22-110">Кроме того, некоторые методы, свойства и действия поддерживаются только для определенных рабочих процессов.</span><span class="sxs-lookup"><span data-stu-id="aed22-110">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="aed22-111">Рабочие процессы Intune совместно работают со следующими ресурсами Graph:</span><span class="sxs-lookup"><span data-stu-id="aed22-111">The following Graph resources are shared between Intune workflows:</span></span>  

- [<span data-ttu-id="aed22-112">Объект назначения всех устройств</span><span class="sxs-lookup"><span data-stu-id="aed22-112">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="aed22-113">Объект назначения всех лицензированных пользователей</span><span class="sxs-lookup"><span data-stu-id="aed22-113">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="aed22-114">Состояние соответствия</span><span class="sxs-lookup"><span data-stu-id="aed22-114">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="aed22-115">Объект назначения для управления устройствами и приложениями</span><span class="sxs-lookup"><span data-stu-id="aed22-115">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="aed22-116">Управление приложениями для устройств</span><span class="sxs-lookup"><span data-stu-id="aed22-116">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="aed22-117">Категория устройств</span><span class="sxs-lookup"><span data-stu-id="aed22-117">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="aed22-118">Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="aed22-118">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="aed22-119">Объект назначения группы исключения</span><span class="sxs-lookup"><span data-stu-id="aed22-119">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="aed22-120">Объект назначения группы</span><span class="sxs-lookup"><span data-stu-id="aed22-120">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="aed22-121">Намерение установки</span><span class="sxs-lookup"><span data-stu-id="aed22-121">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="aed22-122">Содержимое MIME</span><span class="sxs-lookup"><span data-stu-id="aed22-122">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="aed22-123">Отчет</span><span class="sxs-lookup"><span data-stu-id="aed22-123">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="aed22-124">Корневая папка отчета</span><span class="sxs-lookup"><span data-stu-id="aed22-124">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="aed22-125">Сохраненные параметры создания состояния пользовательского интерфейса</span><span class="sxs-lookup"><span data-stu-id="aed22-125">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="aed22-126">URI</span><span class="sxs-lookup"><span data-stu-id="aed22-126">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="aed22-127">Пользователь</span><span class="sxs-lookup"><span data-stu-id="aed22-127">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="aed22-128">Тип учетной записи токена VPP</span><span class="sxs-lookup"><span data-stu-id="aed22-128">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)






