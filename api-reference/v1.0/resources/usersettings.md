---
title: Тип ресурса userSettings
description: 'Параметры текущего пользователя для поиска контента. '
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 862316ba98cab7ccbbaa1c6f7cc909924e400d59
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533418"
---
# <a name="usersettings-resource-type"></a><span data-ttu-id="48f42-103">Тип ресурса userSettings</span><span class="sxs-lookup"><span data-stu-id="48f42-103">userSettings resource type</span></span>

<span data-ttu-id="48f42-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48f42-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="48f42-105">Параметры текущего пользователя для поиска контента.</span><span class="sxs-lookup"><span data-stu-id="48f42-105">The current user settings for content discovery.</span></span>
<span data-ttu-id="48f42-106">Сведения о получении и обновлении параметров пользователя см. в статьях [Получение параметров](../api/usersettings-get.md) и [Обновление параметров](../api/usersettings-update.md).</span><span class="sxs-lookup"><span data-stu-id="48f42-106">To learn how to get or update user settings, see [Get settings](../api/usersettings-get.md) and [Update settings](../api/usersettings-update.md).</span></span>

<span data-ttu-id="48f42-107">Этот ресурс поддерживает:</span><span class="sxs-lookup"><span data-stu-id="48f42-107">This resource supports:</span></span>

- <span data-ttu-id="48f42-108">Проверку участия пользователя и организации пользователя в поиске содержимого.</span><span class="sxs-lookup"><span data-stu-id="48f42-108">Checking whether a user and the user's organization contribute to content discovery.</span></span>
- <span data-ttu-id="48f42-109">Включение и отключение поиска содержимого для конкретных пользователей.</span><span class="sxs-lookup"><span data-stu-id="48f42-109">Disabling or enabling content discovery for specific users.</span></span> <span data-ttu-id="48f42-110">При этом также отключаются документы в Office Delve.</span><span class="sxs-lookup"><span data-stu-id="48f42-110">This also disables documents in Office Delve.</span></span>

## <a name="methods"></a><span data-ttu-id="48f42-111">Методы</span><span class="sxs-lookup"><span data-stu-id="48f42-111">Methods</span></span>
| <span data-ttu-id="48f42-112">Метод</span><span class="sxs-lookup"><span data-stu-id="48f42-112">Method</span></span>       | <span data-ttu-id="48f42-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="48f42-113">Return Type</span></span>  |<span data-ttu-id="48f42-114">Описание</span><span class="sxs-lookup"><span data-stu-id="48f42-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="48f42-115">Получение параметров пользователя</span><span class="sxs-lookup"><span data-stu-id="48f42-115">Get user settings</span></span>](../api/usersettings-get.md) |[<span data-ttu-id="48f42-116">userSettings</span><span class="sxs-lookup"><span data-stu-id="48f42-116">userSettings</span></span>](../resources/usersettings.md)| <span data-ttu-id="48f42-117">Получение параметров пользователя и организации.</span><span class="sxs-lookup"><span data-stu-id="48f42-117">Get the user and organization settings.</span></span> |
|[<span data-ttu-id="48f42-118">Обновление параметров пользователя</span><span class="sxs-lookup"><span data-stu-id="48f42-118">Update user settings</span></span>](../api/usersettings-update.md) |[<span data-ttu-id="48f42-119">userSettings</span><span class="sxs-lookup"><span data-stu-id="48f42-119">userSettings</span></span>](../resources/usersettings.md)| <span data-ttu-id="48f42-120">Обновление текущих параметров пользователя.</span><span class="sxs-lookup"><span data-stu-id="48f42-120">Update the user current settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="48f42-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="48f42-121">Properties</span></span>

| <span data-ttu-id="48f42-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="48f42-122">Property</span></span>     | <span data-ttu-id="48f42-123">Тип</span><span class="sxs-lookup"><span data-stu-id="48f42-123">Type</span></span>   |<span data-ttu-id="48f42-124">Описание</span><span class="sxs-lookup"><span data-stu-id="48f42-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="48f42-125">contributionToContentDiscoveryDisabled</span><span class="sxs-lookup"><span data-stu-id="48f42-125">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="48f42-126">Логический</span><span class="sxs-lookup"><span data-stu-id="48f42-126">Boolean</span></span>|<span data-ttu-id="48f42-127">Если задано значение true, делегированный доступ к API [trending](/graph/api/resources/insights-trending?view=graph-rest-beta) пользователя отключен.</span><span class="sxs-lookup"><span data-stu-id="48f42-127">When set to true, the delegate access to the user's [trending](/graph/api/resources/insights-trending?view=graph-rest-beta) API is disabled.</span></span> <span data-ttu-id="48f42-128">Если задано значение true, документы в Office Delve пользователя отключены.</span><span class="sxs-lookup"><span data-stu-id="48f42-128">When set to true, documents in the user's Office Delve are disabled.</span></span> <span data-ttu-id="48f42-129">Установка значения true влияет на релевантность содержимого, отображаемого в Office 365, например в рекомендуемых сайтах на домашней странице SharePoint и в представлении "Обнаружение" в OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="48f42-129">When set to true, the relevancy of the content displayed in Office 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected.</span></span> <span data-ttu-id="48f42-130">Пользователи могут управлять этим параметром в [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span><span class="sxs-lookup"><span data-stu-id="48f42-130">Users can control this setting in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span> |
|<span data-ttu-id="48f42-131">contributionToContentDiscoveryAsOrganizationDisabled</span><span class="sxs-lookup"><span data-stu-id="48f42-131">contributionToContentDiscoveryAsOrganizationDisabled</span></span>|<span data-ttu-id="48f42-132">Логический</span><span class="sxs-lookup"><span data-stu-id="48f42-132">Boolean</span></span>|<span data-ttu-id="48f42-133">Отображает [параметр на уровне организации](https://support.office.com/ru-RU/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff), управляющий делегированным доступом к API [trending](/graph/api/resources/insights-trending?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="48f42-133">Reflects the [organization level setting](https://support.office.com/ru-RU/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff) controlling delegate access to the [trending](/graph/api/resources/insights-trending?view=graph-rest-beta) API.</span></span> <span data-ttu-id="48f42-134">Если задано значение true, у организации отсутствует доступ к Office Delve.</span><span class="sxs-lookup"><span data-stu-id="48f42-134">When set to true, the organization doesn't have access to Office Delve.</span></span> <span data-ttu-id="48f42-135">Это влияет для всей организации на релевантность содержимого, отображаемого в Office 365, например в рекомендуемых сайтах на домашней странице SharePoint и в представлении "Обнаружение" в OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="48f42-135">The relevancy of the content displayed in Office 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected for the whole organization.</span></span> <span data-ttu-id="48f42-136">Этот параметр доступен только для чтения и может изменяться только администраторами в [Центре администрирования SharePoint](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span><span class="sxs-lookup"><span data-stu-id="48f42-136">This setting is read-only and can only be changed by administrators in the [SharePoint admin center](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span></span>|


## <a name="json-representation"></a><span data-ttu-id="48f42-137">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="48f42-137">JSON representation</span></span>

<span data-ttu-id="48f42-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="48f42-138">Here is a JSON representation of the resource.</span></span>

```json
{
  "contributionToContentDiscoveryDisabled": false,
  "contributionToContentDiscoveryAsOrganizationDisabled": false
}

```
