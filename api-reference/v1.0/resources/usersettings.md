---
title: Тип ресурса userSettings
description: 'Параметры текущего пользователя для поиска контента. '
author: jpettere
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 85a1a9556a5bc02224c8add5e97bc6cbd442cf77
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721878"
---
# <a name="usersettings-resource-type"></a><span data-ttu-id="b04ce-103">Тип ресурса userSettings</span><span class="sxs-lookup"><span data-stu-id="b04ce-103">userSettings resource type</span></span>

<span data-ttu-id="b04ce-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b04ce-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b04ce-105">Параметры текущего пользователя для поиска контента.</span><span class="sxs-lookup"><span data-stu-id="b04ce-105">The current user settings for content discovery.</span></span>
<span data-ttu-id="b04ce-106">Сведения о получении и обновлении параметров пользователя см. в статьях [Получение параметров](../api/usersettings-get.md) и [Обновление параметров](../api/usersettings-update.md).</span><span class="sxs-lookup"><span data-stu-id="b04ce-106">To learn how to get or update user settings, see [Get settings](../api/usersettings-get.md) and [Update settings](../api/usersettings-update.md).</span></span>

<span data-ttu-id="b04ce-107">Этот ресурс поддерживает:</span><span class="sxs-lookup"><span data-stu-id="b04ce-107">This resource supports:</span></span>

- <span data-ttu-id="b04ce-108">Проверку участия пользователя и организации пользователя в поиске содержимого.</span><span class="sxs-lookup"><span data-stu-id="b04ce-108">Checking whether a user and the user's organization contribute to content discovery.</span></span>
- <span data-ttu-id="b04ce-109">Включение и отключение поиска содержимого для конкретных пользователей.</span><span class="sxs-lookup"><span data-stu-id="b04ce-109">Disabling or enabling content discovery for specific users.</span></span> <span data-ttu-id="b04ce-110">При этом также отключаются документы в Office Delve.</span><span class="sxs-lookup"><span data-stu-id="b04ce-110">This also disables documents in Office Delve.</span></span>

> [!NOTE]
> <span data-ttu-id="b04ce-111">Эта конечная точка работает только с пользователями.</span><span class="sxs-lookup"><span data-stu-id="b04ce-111">This endpoint works only with users.</span></span> <span data-ttu-id="b04ce-112">Вы не можете использовать эту конечную точку с контактами.</span><span class="sxs-lookup"><span data-stu-id="b04ce-112">You can't use this endpoint with contacts.</span></span>

## <a name="methods"></a><span data-ttu-id="b04ce-113">Методы</span><span class="sxs-lookup"><span data-stu-id="b04ce-113">Methods</span></span>
| <span data-ttu-id="b04ce-114">Метод</span><span class="sxs-lookup"><span data-stu-id="b04ce-114">Method</span></span>       | <span data-ttu-id="b04ce-115">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b04ce-115">Return Type</span></span>  |<span data-ttu-id="b04ce-116">Описание</span><span class="sxs-lookup"><span data-stu-id="b04ce-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b04ce-117">Получение параметров пользователя</span><span class="sxs-lookup"><span data-stu-id="b04ce-117">Get user settings</span></span>](../api/usersettings-get.md) |[<span data-ttu-id="b04ce-118">userSettings</span><span class="sxs-lookup"><span data-stu-id="b04ce-118">userSettings</span></span>](../resources/usersettings.md)| <span data-ttu-id="b04ce-119">Получение параметров пользователя и организации.</span><span class="sxs-lookup"><span data-stu-id="b04ce-119">Get the user and organization settings.</span></span> |
|[<span data-ttu-id="b04ce-120">Обновление параметров пользователя</span><span class="sxs-lookup"><span data-stu-id="b04ce-120">Update user settings</span></span>](../api/usersettings-update.md) |[<span data-ttu-id="b04ce-121">userSettings</span><span class="sxs-lookup"><span data-stu-id="b04ce-121">userSettings</span></span>](../resources/usersettings.md)| <span data-ttu-id="b04ce-122">Обновление текущих параметров пользователя.</span><span class="sxs-lookup"><span data-stu-id="b04ce-122">Update the user current settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="b04ce-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="b04ce-123">Properties</span></span>

| <span data-ttu-id="b04ce-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="b04ce-124">Property</span></span>     | <span data-ttu-id="b04ce-125">Тип</span><span class="sxs-lookup"><span data-stu-id="b04ce-125">Type</span></span>   |<span data-ttu-id="b04ce-126">Описание</span><span class="sxs-lookup"><span data-stu-id="b04ce-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b04ce-127">contributionToContentDiscoveryDisabled</span><span class="sxs-lookup"><span data-stu-id="b04ce-127">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="b04ce-128">Логический</span><span class="sxs-lookup"><span data-stu-id="b04ce-128">Boolean</span></span>|<span data-ttu-id="b04ce-129">Если задано значение true, делегированный доступ к API [trending](/graph/api/resources/insights-trending?view=graph-rest-beta) пользователя отключен.</span><span class="sxs-lookup"><span data-stu-id="b04ce-129">When set to true, the delegate access to the user's [trending](/graph/api/resources/insights-trending?view=graph-rest-beta) API is disabled.</span></span> <span data-ttu-id="b04ce-130">Если задано значение true, документы в Office Delve пользователя отключены.</span><span class="sxs-lookup"><span data-stu-id="b04ce-130">When set to true, documents in the user's Office Delve are disabled.</span></span> <span data-ttu-id="b04ce-131">Установка значения true влияет на релевантность содержимого, отображаемого в Microsoft 365, например в рекомендуемых сайтах на домашней странице SharePoint и в представлении "Обнаружение" в OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="b04ce-131">When set to true, the relevancy of the content displayed in Microsoft 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected.</span></span> <span data-ttu-id="b04ce-132">Пользователи могут управлять этим параметром в [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span><span class="sxs-lookup"><span data-stu-id="b04ce-132">Users can control this setting in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span> |
|<span data-ttu-id="b04ce-133">contributionToContentDiscoveryAsOrganizationDisabled</span><span class="sxs-lookup"><span data-stu-id="b04ce-133">contributionToContentDiscoveryAsOrganizationDisabled</span></span>|<span data-ttu-id="b04ce-134">Логический</span><span class="sxs-lookup"><span data-stu-id="b04ce-134">Boolean</span></span>|<span data-ttu-id="b04ce-135">Отображает [параметр на уровне организации](https://support.office.com/ru-RU/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff), управляющий делегированным доступом к API [trending](/graph/api/resources/insights-trending?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="b04ce-135">Reflects the [organization level setting](https://support.office.com/ru-RU/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff) controlling delegate access to the [trending](/graph/api/resources/insights-trending?view=graph-rest-beta) API.</span></span> <span data-ttu-id="b04ce-136">Если задано значение true, у организации отсутствует доступ к Office Delve.</span><span class="sxs-lookup"><span data-stu-id="b04ce-136">When set to true, the organization doesn't have access to Office Delve.</span></span> <span data-ttu-id="b04ce-137">Это влияет на релевантность содержимого, отображаемого в Microsoft 365 для всей организации, например в рекомендуемых сайтах на домашней странице SharePoint и в представлении "Обнаружение" в OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="b04ce-137">The relevancy of the content displayed in Microsoft 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected for the whole organization.</span></span> <span data-ttu-id="b04ce-138">Этот параметр доступен только для чтения и может изменяться только администраторами в [Центре администрирования SharePoint](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span><span class="sxs-lookup"><span data-stu-id="b04ce-138">This setting is read-only and can only be changed by administrators in the [SharePoint admin center](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span></span>|


## <a name="json-representation"></a><span data-ttu-id="b04ce-139">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b04ce-139">JSON representation</span></span>

<span data-ttu-id="b04ce-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b04ce-140">Here is a JSON representation of the resource.</span></span>

```json
{
  "contributionToContentDiscoveryDisabled": false,
  "contributionToContentDiscoveryAsOrganizationDisabled": false
}

```

