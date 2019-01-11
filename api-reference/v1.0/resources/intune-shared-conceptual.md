---
title: Общие ресурсы в Microsoft Intune
description: Эти конечные точки используются в нескольких Microsoft Graph API Intune рабочих процессов.  Цель, назначения и разрешения, необходимые для использования указанного ресурса изменяется в зависимости от конкретного рабочего процесса и контекста вызова базового.  Кроме того некоторые методы, свойства и действия поддерживаются только для определенных рабочих процессов.
localization_priority: Normal
ms.openlocfilehash: d0d615be8d185c5dfe24d58f6a2e371e6baf18c9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840070"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="06641-105">Общие ресурсы в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="06641-105">Shared resources in Microsoft Intune</span></span>

> <span data-ttu-id="06641-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="06641-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="06641-107">Эти конечные точки используются в нескольких Microsoft Graph API Intune рабочих процессов.</span><span class="sxs-lookup"><span data-stu-id="06641-107">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="06641-108">Цель, назначения и разрешения, необходимые для использования указанного ресурса изменяется в зависимости от конкретного рабочего процесса и контекста вызова базового.</span><span class="sxs-lookup"><span data-stu-id="06641-108">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="06641-109">Кроме того некоторые методы, свойства и действия поддерживаются только для определенных рабочих процессов.</span><span class="sxs-lookup"><span data-stu-id="06641-109">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="06641-110">В следующих ресурсах графике совместно Intune рабочих процессов:</span><span class="sxs-lookup"><span data-stu-id="06641-110">The following Graph resources are shared between Intune workflows:</span></span>  

- [<span data-ttu-id="06641-111">Объект назначения всех устройств</span><span class="sxs-lookup"><span data-stu-id="06641-111">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="06641-112">Объект назначения всех лицензированных пользователей</span><span class="sxs-lookup"><span data-stu-id="06641-112">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="06641-113">Состояние соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="06641-113">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="06641-114">Объект назначения для управления устройствами и приложениями</span><span class="sxs-lookup"><span data-stu-id="06641-114">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="06641-115">Управление приложениями для устройств</span><span class="sxs-lookup"><span data-stu-id="06641-115">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="06641-116">Категория устройств</span><span class="sxs-lookup"><span data-stu-id="06641-116">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="06641-117">Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="06641-117">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="06641-118">Объект назначения группы исключения</span><span class="sxs-lookup"><span data-stu-id="06641-118">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="06641-119">Объект назначения группы</span><span class="sxs-lookup"><span data-stu-id="06641-119">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="06641-120">Цель установки</span><span class="sxs-lookup"><span data-stu-id="06641-120">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="06641-121">Содержимое MIME</span><span class="sxs-lookup"><span data-stu-id="06641-121">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="06641-122">Report</span><span class="sxs-lookup"><span data-stu-id="06641-122">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="06641-123">Корневой отчета</span><span class="sxs-lookup"><span data-stu-id="06641-123">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="06641-124">Сохранить параметры создания состояние пользовательского интерфейса</span><span class="sxs-lookup"><span data-stu-id="06641-124">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="06641-125">URI</span><span class="sxs-lookup"><span data-stu-id="06641-125">URI</span></span>](intune-shared-uri.md)
- <span data-ttu-id="06641-126">[пользователь](intune-shared-user.md);</span><span class="sxs-lookup"><span data-stu-id="06641-126">[User](intune-shared-user.md)</span></span>
- [<span data-ttu-id="06641-127">Тип учетной записи маркеров VPP</span><span class="sxs-lookup"><span data-stu-id="06641-127">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
