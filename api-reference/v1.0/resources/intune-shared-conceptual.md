---
title: Общие ресурсы в Microsoft Intune
description: Эти конечные точки используются в нескольких API Graph Microsoft для рабочего процесса Intune.  Намерения, цели и разрешения, необходимые для использования данного ресурса, зависят от конкретного рабочего процесса и контекста данного вызова.  Кроме того, некоторые методы, свойства и действия поддерживаются только для определенных процессов.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: 0af56b1ec3014fdee14dc4b70d3c14208321581a
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53108889"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="a8a21-105">Общие ресурсы в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="a8a21-105">Shared resources in Microsoft Intune</span></span>

<span data-ttu-id="a8a21-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8a21-106">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a8a21-107">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a8a21-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="a8a21-108">Эти конечные точки используются в нескольких API Graph Microsoft для рабочего процесса Intune.</span><span class="sxs-lookup"><span data-stu-id="a8a21-108">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="a8a21-109">Намерения, цели и разрешения, необходимые для использования данного ресурса, зависят от конкретного рабочего процесса и контекста данного вызова.</span><span class="sxs-lookup"><span data-stu-id="a8a21-109">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="a8a21-110">Кроме того, некоторые методы, свойства и действия поддерживаются только для определенных процессов.</span><span class="sxs-lookup"><span data-stu-id="a8a21-110">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="a8a21-111">Между Graph intune общие ресурсы:</span><span class="sxs-lookup"><span data-stu-id="a8a21-111">The following Graph resources are shared between Intune workflows:</span></span>  

- [<span data-ttu-id="a8a21-112">Объект назначения всех устройств</span><span class="sxs-lookup"><span data-stu-id="a8a21-112">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="a8a21-113">Объект назначения всех лицензированных пользователей</span><span class="sxs-lookup"><span data-stu-id="a8a21-113">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="a8a21-114">Android-предприятие всегда на типе пакета VPN</span><span class="sxs-lookup"><span data-stu-id="a8a21-114">Android enterprise always on VPN package type</span></span>](intune-shared-androidenterprisealwaysonvpnpackagetype.md)
- [<span data-ttu-id="a8a21-115">Состояние соответствия</span><span class="sxs-lookup"><span data-stu-id="a8a21-115">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="a8a21-116">Цель назначения коллекции диспетчера конфигурации</span><span class="sxs-lookup"><span data-stu-id="a8a21-116">Configuration manager collection assignment target</span></span>](intune-shared-configurationmanagercollectionassignmenttarget.md)
- [<span data-ttu-id="a8a21-117">Объект назначения для управления устройствами и приложениями</span><span class="sxs-lookup"><span data-stu-id="a8a21-117">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="a8a21-118">Объект назначения группы исключения</span><span class="sxs-lookup"><span data-stu-id="a8a21-118">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="a8a21-119">Объект назначения группы</span><span class="sxs-lookup"><span data-stu-id="a8a21-119">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="a8a21-120">Намерение установки</span><span class="sxs-lookup"><span data-stu-id="a8a21-120">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="a8a21-121">Содержимое MIME</span><span class="sxs-lookup"><span data-stu-id="a8a21-121">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="a8a21-122">Сохраненные параметры создания состояния пользовательского интерфейса</span><span class="sxs-lookup"><span data-stu-id="a8a21-122">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="a8a21-123">URI</span><span class="sxs-lookup"><span data-stu-id="a8a21-123">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="a8a21-124">Тип учетной записи токена VPP</span><span class="sxs-lookup"><span data-stu-id="a8a21-124">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)