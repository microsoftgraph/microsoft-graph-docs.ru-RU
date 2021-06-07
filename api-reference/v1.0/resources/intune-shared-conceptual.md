---
title: Общие ресурсы в Microsoft Intune
description: Эти конечные точки используются в нескольких API Graph Microsoft для рабочего процесса Intune.  Намерения, цели и разрешения, необходимые для использования данного ресурса, зависят от конкретного рабочего процесса и контекста данного вызова.  Кроме того, некоторые методы, свойства и действия поддерживаются только для определенных процессов.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: cc5cbf0f96d3c9199ecd9b622d9724ec10dd472e
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732773"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="b1bd9-105">Общие ресурсы в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="b1bd9-105">Shared resources in Microsoft Intune</span></span>

<span data-ttu-id="b1bd9-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1bd9-106">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b1bd9-107">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b1bd9-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="b1bd9-108">Эти конечные точки используются в нескольких API Graph Microsoft для рабочего процесса Intune.</span><span class="sxs-lookup"><span data-stu-id="b1bd9-108">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="b1bd9-109">Намерения, цели и разрешения, необходимые для использования данного ресурса, зависят от конкретного рабочего процесса и контекста данного вызова.</span><span class="sxs-lookup"><span data-stu-id="b1bd9-109">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="b1bd9-110">Кроме того, некоторые методы, свойства и действия поддерживаются только для определенных процессов.</span><span class="sxs-lookup"><span data-stu-id="b1bd9-110">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="b1bd9-111">Между Graph intune общие ресурсы:</span><span class="sxs-lookup"><span data-stu-id="b1bd9-111">The following Graph resources are shared between Intune workflows:</span></span>  

- [<span data-ttu-id="b1bd9-112">Объект назначения всех устройств</span><span class="sxs-lookup"><span data-stu-id="b1bd9-112">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="b1bd9-113">Объект назначения всех лицензированных пользователей</span><span class="sxs-lookup"><span data-stu-id="b1bd9-113">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="b1bd9-114">Состояние соответствия</span><span class="sxs-lookup"><span data-stu-id="b1bd9-114">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="b1bd9-115">Объект назначения для управления устройствами и приложениями</span><span class="sxs-lookup"><span data-stu-id="b1bd9-115">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="b1bd9-116">Управление приложениями для устройств</span><span class="sxs-lookup"><span data-stu-id="b1bd9-116">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="b1bd9-117">Категория устройств</span><span class="sxs-lookup"><span data-stu-id="b1bd9-117">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="b1bd9-118">Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="b1bd9-118">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="b1bd9-119">Объект назначения группы исключения</span><span class="sxs-lookup"><span data-stu-id="b1bd9-119">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="b1bd9-120">Объект назначения группы</span><span class="sxs-lookup"><span data-stu-id="b1bd9-120">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="b1bd9-121">Намерение установки</span><span class="sxs-lookup"><span data-stu-id="b1bd9-121">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="b1bd9-122">Содержимое MIME</span><span class="sxs-lookup"><span data-stu-id="b1bd9-122">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="b1bd9-123">Отчет</span><span class="sxs-lookup"><span data-stu-id="b1bd9-123">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="b1bd9-124">Корневая папка отчета</span><span class="sxs-lookup"><span data-stu-id="b1bd9-124">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="b1bd9-125">Сохраненные параметры создания состояния пользовательского интерфейса</span><span class="sxs-lookup"><span data-stu-id="b1bd9-125">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="b1bd9-126">URI</span><span class="sxs-lookup"><span data-stu-id="b1bd9-126">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="b1bd9-127">Пользователь</span><span class="sxs-lookup"><span data-stu-id="b1bd9-127">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="b1bd9-128">Тип учетной записи токена VPP</span><span class="sxs-lookup"><span data-stu-id="b1bd9-128">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)






