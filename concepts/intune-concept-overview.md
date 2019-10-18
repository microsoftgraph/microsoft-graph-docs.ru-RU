---
title: Обзор API устройств и приложений Intune
description: 'Microsoft Intune помогает предприятиям управлять устройствами и приложениями в организации. С помощью API Intune в Microsoft Graph вы можете управлять устройствами и приложениями, а также настраивать Intune, используя привычные средства. '
author: rolyon
localization_priority: Priority
ms.prod: intune
ms.openlocfilehash: a18096f53dfa88bd37b0cad11639c3b2285206e6
ms.sourcegitcommit: 7c03131291113c343a98bb0234d31bd4535a4050
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2019
ms.locfileid: "35133770"
---
# <a name="intune-devices-and-apps-api-overview"></a><span data-ttu-id="034b1-104">Обзор API устройств и приложений Intune</span><span class="sxs-lookup"><span data-stu-id="034b1-104">Intune devices and apps API overview</span></span>

<span data-ttu-id="034b1-105">Microsoft Intune помогает предприятиям управлять устройствами и приложениями в организации.</span><span class="sxs-lookup"><span data-stu-id="034b1-105">Microsoft Intune helps enterprises manage devices and apps within an organization.</span></span> <span data-ttu-id="034b1-106">С помощью API Intune в Microsoft Graph вы можете управлять устройствами и приложениями, а также настраивать Intune, используя привычные средства.</span><span class="sxs-lookup"><span data-stu-id="034b1-106">You can use the Intune API in Microsoft Graph to manage devices, apps, and even configure Intune while using your preferred tools.</span></span> 

<span data-ttu-id="034b1-107">Если вы независимый поставщик программного обеспечения, вы также можете использовать API Intune для управления клиентами.</span><span class="sxs-lookup"><span data-stu-id="034b1-107">If you're an ISV, you can also use the Intune API to manage client tenants.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/yU1HeqNmN7A]

## <a name="why-integrate-with-intune"></a><span data-ttu-id="034b1-108">Преимущества интеграции с Intune</span><span class="sxs-lookup"><span data-stu-id="034b1-108">Why integrate with Intune?</span></span>

<span data-ttu-id="034b1-109">Вы также можете использовать API Intune в Microsoft Graph для доступа к сведениям об устройствах и приложениях из Intune, управления приложениями и автоматизации Intune.</span><span class="sxs-lookup"><span data-stu-id="034b1-109">You can use the Intune API in Microsoft Graph to access Intune device and application information, manage devices, manage apps, and automate Intune.</span></span>

### <a name="manage-devices"></a><span data-ttu-id="034b1-110">Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="034b1-110">Manage devices</span></span>

<span data-ttu-id="034b1-111">С помощью API Intune вы можете:</span><span class="sxs-lookup"><span data-stu-id="034b1-111">You can use the Intune API to:</span></span>

- <span data-ttu-id="034b1-112">Определять и применять политики [соответствия устройств различным требованиям](/graph/api/resources/intune-deviceconfig-devicecomplianceactionitem?view=graph-rest-1.0), таким как сложность и длина пароля, шифрование, уровни защиты от угроз.</span><span class="sxs-lookup"><span data-stu-id="034b1-112">Define and enforce [device compliance](/graph/api/resources/intune-deviceconfig-devicecomplianceactionitem?view=graph-rest-1.0) policies, such as password complexity and duration, encryption, threat protection levels, and so on.</span></span>  <span data-ttu-id="034b1-113">(То, поддерживается ли политика, зависит от используемой операционной системы и ее версии.)</span><span class="sxs-lookup"><span data-stu-id="034b1-113">(Supported policies vary according to operating system and version).</span></span>
- <span data-ttu-id="034b1-114">[Защищать данные компании](/graph/api/resources/intune-mam-windowsinformationprotectionpolicy?view=graph-rest-1.0) независимо от платформы устройства (Windows, Android, Mac или iOS).</span><span class="sxs-lookup"><span data-stu-id="034b1-114">[Protect company data](/graph/api/resources/intune-mam-windowsinformationprotectionpolicy?view=graph-rest-1.0), regardless of whether the device platform is Windows, Android, Mac, or iOS.</span></span>
- <span data-ttu-id="034b1-115">Создавать и развертывать политики [конфигурации устройств](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-1.0), включая платформы и версии операционной системы, членство в доменах и управление параметрами конфигурации.</span><span class="sxs-lookup"><span data-stu-id="034b1-115">Create and deploy [device configuration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-1.0) policies, including operating system platform/versioning, domain membership, and configuration setting management.</span></span>
- <span data-ttu-id="034b1-116">Создавать и развертывать политики [контроля доступа](/graph/api/resources/intune-onboarding-onpremisesconditionalaccesssettings?view=graph-rest-1.0) для устройств, включая ограниченную загрузку, доступ к сетевым аксессуарам и передачу данных.</span><span class="sxs-lookup"><span data-stu-id="034b1-116">Create and deploy device [access control](/graph/api/resources/intune-onboarding-onpremisesconditionalaccesssettings?view=graph-rest-1.0) policies, including restricted download, network accessory access, and file transfer.</span></span>
- <span data-ttu-id="034b1-117">Выполнять [удаленные действия](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0), например поиск устройства, изменение пароля и стирание данных устройства.</span><span class="sxs-lookup"><span data-stu-id="034b1-117">Perform [remote actions](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0), such as locate device, change password, and wipe device.</span></span>

### <a name="manage-apps"></a><span data-ttu-id="034b1-118">Управление приложениями</span><span class="sxs-lookup"><span data-stu-id="034b1-118">Manage apps</span></span> 

<span data-ttu-id="034b1-119">С помощью API Intune вы можете выполнять указанные ниже задачи по управлению приложениями.</span><span class="sxs-lookup"><span data-stu-id="034b1-119">You can use the Intune API to perform the following app management tasks:</span></span>

- <span data-ttu-id="034b1-120">Развертывание [приложений на устройствах](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-1.0) и запрет развертывания приложений.</span><span class="sxs-lookup"><span data-stu-id="034b1-120">Deploy [apps to devices](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-1.0) or prevent apps from being deployed.</span></span>
- <span data-ttu-id="034b1-121">Управление доступом к [электронным книгам](/graph/api/resources/intune-books-ebookinstallsummary?view=graph-rest-1.0) и соответствующим службам.</span><span class="sxs-lookup"><span data-stu-id="034b1-121">Manage access to [ebooks](/graph/api/resources/intune-books-ebookinstallsummary?view=graph-rest-1.0) and related services.</span></span>
- <span data-ttu-id="034b1-122">Определение и развертывание параметров конфигурации и защиты приложений, а также политик их использования.</span><span class="sxs-lookup"><span data-stu-id="034b1-122">Define and deploy app configuration settings, app protection settings, and app usage policies.</span></span>

### <a name="automate-intune"></a><span data-ttu-id="034b1-123">Автоматизация Intune</span><span class="sxs-lookup"><span data-stu-id="034b1-123">Automate Intune</span></span>

<span data-ttu-id="034b1-124">Автоматизируйте Intune, используя API Intune для:</span><span class="sxs-lookup"><span data-stu-id="034b1-124">Automate Intune by using the Intune API to:</span></span>

- <span data-ttu-id="034b1-125">определения и назначения правил доступа [на основе ролей](/graph/api/resources/intune-rbac-conceptual?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="034b1-125">Define and assign [role based](/graph/api/resources/intune-rbac-conceptual?view=graph-rest-1.0) access controls.</span></span>
- <span data-ttu-id="034b1-126">аудита и создания отчетов о соответствии требованиям, использовании и доступе;</span><span class="sxs-lookup"><span data-stu-id="034b1-126">Audit and report compliance, usage, and access.</span></span>
- <span data-ttu-id="034b1-127">управления [затратами на телекоммуникации](/graph/api/resources/intune-tem-conceptual?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="034b1-127">Manage [telecom expenses](/graph/api/resources/intune-tem-conceptual?view=graph-rest-1.0).</span></span>

## <a name="api-reference"></a><span data-ttu-id="034b1-128">Справочные материалы по API</span><span class="sxs-lookup"><span data-stu-id="034b1-128">API reference</span></span>
<span data-ttu-id="034b1-129">Ищете справочные материалы по API для этой службы?</span><span class="sxs-lookup"><span data-stu-id="034b1-129">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="034b1-130">API Intune в Microsoft Graph 1.0</span><span class="sxs-lookup"><span data-stu-id="034b1-130">Intune API in Microsoft Graph v1.0</span></span>](/graph/api/resources/intune-graph-overview?view=graph-rest-1.0)
- [<span data-ttu-id="034b1-131">API Intune в бета-версии Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="034b1-131">Intune API in Microsoft Graph beta</span></span>](/graph/api/resources/intune-graph-overview?view=graph-rest-beta)

## <a name="next-steps"></a><span data-ttu-id="034b1-132">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="034b1-132">Next steps</span></span>

- <span data-ttu-id="034b1-133">[Доступ к интерфейсам API Intune в Microsoft Graph с использованием Azure AD](https://docs.microsoft.com/intune/intune-graph-apis).</span><span class="sxs-lookup"><span data-stu-id="034b1-133">[Use Azure AD to access the Intune API](https://docs.microsoft.com/intune/intune-graph-apis).</span></span>
- <span data-ttu-id="034b1-134">Узнайте, как выполнять распространенные задачи, с помощью [примеров PowerShell для Intune](https://github.com/microsoftgraph/powershell-intune-samples).</span><span class="sxs-lookup"><span data-stu-id="034b1-134">See how to perform common tasks by using the [PowerShell Intune samples](https://github.com/microsoftgraph/powershell-intune-samples).</span></span>
- <span data-ttu-id="034b1-135">Узнайте, как [использовать REST API Intune](/graph/api/resources/intune-graph-overview?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="034b1-135">Find out how to [use the Intune REST API](/graph/api/resources/intune-graph-overview?view=graph-rest-1.0).</span></span>
- <span data-ttu-id="034b1-136">Сведения о новых возможностях API Intune см. в [журнале изменений](changelog.md).</span><span class="sxs-lookup"><span data-stu-id="034b1-136">See the [Changelog](changelog.md) for information about what's new in the Intune API.</span></span>
- <span data-ttu-id="034b1-137">Изучите [примеры](https://developer.microsoft.com/graph/graph/examples) с новыми идеями о том, как использовать Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="034b1-137">Explore [examples](https://developer.microsoft.com/graph/graph/examples) for more ideas about how to use Microsoft Graph.</span></span>
