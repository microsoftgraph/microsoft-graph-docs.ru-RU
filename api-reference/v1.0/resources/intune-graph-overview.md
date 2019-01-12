---
title: Использование API Graph для Intune
description: " Гибридные развертывания Intune не поддерживаются. "
author: tfitzmac
localization_priority: Priority
ms.prod: intune
ms.openlocfilehash: 2dfeb5ff55670f3e11b175e0472359002b09bab6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975332"
---
# <a name="working-with-intune-in-microsoft-graph"></a><span data-ttu-id="b2ea7-103">Работа с Intune в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b2ea7-103">Working with Intune in Microsoft Graph</span></span>  

> <span data-ttu-id="b2ea7-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b2ea7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="b2ea7-105">API Microsoft Graph для Intune обеспечивает программный доступ к сведениям Intune для клиента. API выполняет операции Intune, аналогичные доступным с помощью **портала Azure**.</span><span class="sxs-lookup"><span data-stu-id="b2ea7-105">The Microsoft Graph API for Intune enables programmatic access to Intune information for your tenant; the API performs the same Intune operations as those available through the **Azure Portal**.</span></span>  

<span data-ttu-id="b2ea7-106">Для сценариев мобильных устройств management (MDM) Microsoft Graph API для Intune поддерживает развертывание автономных; Intune [гибридные развертывания](https://docs.microsoft.com/en-us/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="b2ea7-106">For mobile device management (MDM) scenarios, the Microsoft Graph API for Intune supports standalone deployments; Intune [hybrid deployments](https://docs.microsoft.com/en-us/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) are not supported.</span></span> 

## <a name="using-the-microsoft-graph-api-for-intune"></a><span data-ttu-id="b2ea7-107">С помощью Microsoft Graph API для Intune</span><span class="sxs-lookup"><span data-stu-id="b2ea7-107">Using the Microsoft Graph API for Intune</span></span>

<span data-ttu-id="b2ea7-108">Intune предоставляет данные интерфейсу API Microsoft Graph аналогично другим облачным службам, предоставляя обширные сведения об объектах и обеспечивая навигацию по связям.</span><span class="sxs-lookup"><span data-stu-id="b2ea7-108">Intune provides data into the Microsoft Graph API in the same way as other cloud services do, with rich entity information and relationship navigation.</span></span><span data-ttu-id="b2ea7-109">Используйте Microsoft Graph API для объединения данных из других служб и Intune создавать полнофункциональный приложения кросс service для ИТ-специалистов и конечных пользователей.</span><span class="sxs-lookup"><span data-stu-id="b2ea7-109"> Use the Microsoft Graph API to combine information from other services and Intune to build rich cross-service applications for IT professionals or end users.</span></span>     

<span data-ttu-id="b2ea7-110">В следующем примере показано, как определить, установлено ли приложение на устройстве пользователя:</span><span class="sxs-lookup"><span data-stu-id="b2ea7-110">The following example shows how you can determine whether an application is installed on a user's device:</span></span> 

1. <span data-ttu-id="b2ea7-111">Из Azure Active Directory извлеките список устройств, зарегистрированных для пользователя:</span><span class="sxs-lookup"><span data-stu-id="b2ea7-111">Get from Azure Active Directory a list of devices registered to a user:</span></span> 

    https://graph.microsoft.com/users/{user}/ownedDevices 

2. <span data-ttu-id="b2ea7-112">Затем просмотрите список приложений для вашего клиента:</span><span class="sxs-lookup"><span data-stu-id="b2ea7-112">Then view the list of applications for your tenant:</span></span> 

    https://graph.microsoft.com/deviceAppManagement/mobileApps  

3. <span data-ttu-id="b2ea7-113">На основе идентификатора, указанного в приложении, определите состояние установки для приложения (и, следовательно, пользователя):</span><span class="sxs-lookup"><span data-stu-id="b2ea7-113">Take the ID from the application and determine the installation state for the application (and therefore user):</span></span>

    https://graph.microsoft.com/deviceAppManagement/mobileApps/{id}/deviceStatuses/


## <a name="using-permissions"></a><span data-ttu-id="b2ea7-114">Использование разрешений</span><span class="sxs-lookup"><span data-stu-id="b2ea7-114">Using permissions</span></span>

<span data-ttu-id="b2ea7-115">API-Интерфейс Microsoft Graph управляет доступом к ресурсам с помощью разрешений.</span><span class="sxs-lookup"><span data-stu-id="b2ea7-115">The Microsoft Graph API controls access to resources via permissions.</span></span> <span data-ttu-id="b2ea7-116">Являясь разработчиком необходимо указать разрешения, необходимые для доступа к ресурсам Intune.</span><span class="sxs-lookup"><span data-stu-id="b2ea7-116">As a developer, you must specify the permissions you need to access Intune resources.</span></span> <span data-ttu-id="b2ea7-117">Как правило укажите разрешения на портале Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b2ea7-117">Typically, you specify the permissions in the Azure Active Directory portal.</span></span> <span data-ttu-id="b2ea7-118">Для получения дополнительных сведений см [Microsoft Graph разрешения](https://docs.microsoft.com/en-us/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2ea7-118">For more information, see [Microsoft Graph permissions reference](https://docs.microsoft.com/en-us/graph/permissions-reference).</span></span>

## <a name="next-steps"></a><span data-ttu-id="b2ea7-119">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="b2ea7-119">Next Steps</span></span>

- <span data-ttu-id="b2ea7-120">Узнайте, [как использовать Azure AD](https://docs.microsoft.com/en-us/intune/intune-graph-apis) для доступа к Microsoft Graph API для Intune.</span><span class="sxs-lookup"><span data-stu-id="b2ea7-120">Learn [how to use Azure AD](https://docs.microsoft.com/en-us/intune/intune-graph-apis) to access the Microsoft Graph API for Intune.</span></span>  
- <span data-ttu-id="b2ea7-121">Изучите [Примеры PowerShell Intune](https://github.com/microsoftgraph/powershell-intune-samples), которой показано, как использовать Microsoft Graph API для Intune в контексте рабочие примеры.</span><span class="sxs-lookup"><span data-stu-id="b2ea7-121">Explore the [PowerShell Intune samples](https://github.com/microsoftgraph/powershell-intune-samples), which show how to use the Microsoft Graph API for Intune in context of working examples.</span></span>
