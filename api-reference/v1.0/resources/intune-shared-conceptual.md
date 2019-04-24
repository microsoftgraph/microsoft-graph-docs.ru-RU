---
title: Общие ресурсы в Microsoft Intune
description: Эти конечные точки используются в нескольких ИНТЕРФЕЙСах API Microsoft Graph для рабочих процессов Intune.  Цель, цель и разрешения, необходимые для использования указанного ресурса, меняются в зависимости от конкретного рабочего процесса и контекста базового вызова.  Кроме того, некоторые методы, свойства и действия поддерживаются только для определенных рабочих процессов.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: cfb3acbb3b736fcb96d22773301ca6e2e3e4403f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32452185"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="b76c3-105">Общие ресурсы в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="b76c3-105">Shared resources in Microsoft Intune</span></span>

> <span data-ttu-id="b76c3-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b76c3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="b76c3-107">Эти конечные точки используются в нескольких ИНТЕРФЕЙСах API Microsoft Graph для рабочих процессов Intune.</span><span class="sxs-lookup"><span data-stu-id="b76c3-107">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="b76c3-108">Цель, цель и разрешения, необходимые для использования указанного ресурса, меняются в зависимости от конкретного рабочего процесса и контекста базового вызова.</span><span class="sxs-lookup"><span data-stu-id="b76c3-108">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="b76c3-109">Кроме того, некоторые методы, свойства и действия поддерживаются только для определенных рабочих процессов.</span><span class="sxs-lookup"><span data-stu-id="b76c3-109">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="b76c3-110">Рабочие процессы Intune совместно работают со следующими ресурсами Graph:</span><span class="sxs-lookup"><span data-stu-id="b76c3-110">The following Graph resources are shared between Intune workflows:</span></span>  

- [<span data-ttu-id="b76c3-111">Объект назначения всех устройств</span><span class="sxs-lookup"><span data-stu-id="b76c3-111">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="b76c3-112">Объект назначения всех лицензированных пользователей</span><span class="sxs-lookup"><span data-stu-id="b76c3-112">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="b76c3-113">Состояние соответствия</span><span class="sxs-lookup"><span data-stu-id="b76c3-113">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="b76c3-114">Объект назначения для управления устройствами и приложениями</span><span class="sxs-lookup"><span data-stu-id="b76c3-114">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="b76c3-115">Управление приложениями для устройств</span><span class="sxs-lookup"><span data-stu-id="b76c3-115">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="b76c3-116">Категория устройств</span><span class="sxs-lookup"><span data-stu-id="b76c3-116">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="b76c3-117">Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="b76c3-117">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="b76c3-118">Объект назначения группы исключения</span><span class="sxs-lookup"><span data-stu-id="b76c3-118">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="b76c3-119">Объект назначения группы</span><span class="sxs-lookup"><span data-stu-id="b76c3-119">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="b76c3-120">Намерение установки</span><span class="sxs-lookup"><span data-stu-id="b76c3-120">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="b76c3-121">Содержимое MIME</span><span class="sxs-lookup"><span data-stu-id="b76c3-121">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="b76c3-122">Report</span><span class="sxs-lookup"><span data-stu-id="b76c3-122">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="b76c3-123">Корневая папка отчета</span><span class="sxs-lookup"><span data-stu-id="b76c3-123">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="b76c3-124">Сохраненные параметры создания состояния пользовательского интерфейса</span><span class="sxs-lookup"><span data-stu-id="b76c3-124">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="b76c3-125">URI</span><span class="sxs-lookup"><span data-stu-id="b76c3-125">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="b76c3-126">Пользователь</span><span class="sxs-lookup"><span data-stu-id="b76c3-126">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="b76c3-127">Тип учетной записи токена VPP</span><span class="sxs-lookup"><span data-stu-id="b76c3-127">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
