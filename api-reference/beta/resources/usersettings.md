---
title: Тип ресурса Усерсеттингс
description: 'Текущие параметры пользователя для обнаружения контента. '
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0168ee426bb9c03d7a53add2d1842a498c930330
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2019
ms.locfileid: "39844255"
---
# <a name="usersettings-resource-type"></a><span data-ttu-id="83dc1-103">Тип ресурса Усерсеттингс</span><span class="sxs-lookup"><span data-stu-id="83dc1-103">userSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83dc1-104">Текущие параметры пользователя для обнаружения контента.</span><span class="sxs-lookup"><span data-stu-id="83dc1-104">The current user settings for content discovery.</span></span> <span data-ttu-id="83dc1-105">Сведения о получении и обновлении параметров пользователя см. в статьях [Получение параметров](../api/usersettings-get.md) и [Обновление параметров](../api/usersettings-update.md).</span><span class="sxs-lookup"><span data-stu-id="83dc1-105">To learn how to get or update user settings, see [Get settings](../api/usersettings-get.md) and [Update settings](../api/usersettings-update.md).</span></span>

<span data-ttu-id="83dc1-106">Этот ресурс поддерживает:</span><span class="sxs-lookup"><span data-stu-id="83dc1-106">This resource supports:</span></span>

- <span data-ttu-id="83dc1-107">Проверку участия пользователя и организации пользователя в поиске содержимого.</span><span class="sxs-lookup"><span data-stu-id="83dc1-107">Checking whether a user and the user's organization contribute to content discovery.</span></span>
- <span data-ttu-id="83dc1-108">Включение и отключение поиска содержимого для конкретных пользователей.</span><span class="sxs-lookup"><span data-stu-id="83dc1-108">Disabling or enabling content discovery for specific users.</span></span> <span data-ttu-id="83dc1-109">При этом также отключаются документы в Office Delve.</span><span class="sxs-lookup"><span data-stu-id="83dc1-109">This also disables documents in Office Delve.</span></span>

## <a name="methods"></a><span data-ttu-id="83dc1-110">Методы</span><span class="sxs-lookup"><span data-stu-id="83dc1-110">Methods</span></span>
| <span data-ttu-id="83dc1-111">Метод</span><span class="sxs-lookup"><span data-stu-id="83dc1-111">Method</span></span>       | <span data-ttu-id="83dc1-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="83dc1-112">Return Type</span></span>  |<span data-ttu-id="83dc1-113">Описание</span><span class="sxs-lookup"><span data-stu-id="83dc1-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="83dc1-114">Получение параметров пользователя</span><span class="sxs-lookup"><span data-stu-id="83dc1-114">Get user settings</span></span>](../api/usersettings-get.md) |[<span data-ttu-id="83dc1-115">userSettings</span><span class="sxs-lookup"><span data-stu-id="83dc1-115">userSettings</span></span>](../resources/usersettings.md)| <span data-ttu-id="83dc1-116">Получение параметров пользователя и организации.</span><span class="sxs-lookup"><span data-stu-id="83dc1-116">Get the user and organization settings.</span></span> |
|[<span data-ttu-id="83dc1-117">Обновление параметров пользователя</span><span class="sxs-lookup"><span data-stu-id="83dc1-117">Update user settings</span></span>](../api/usersettings-update.md) |[<span data-ttu-id="83dc1-118">userSettings</span><span class="sxs-lookup"><span data-stu-id="83dc1-118">userSettings</span></span>](../resources/usersettings.md)| <span data-ttu-id="83dc1-119">Обновление текущих параметров пользователя.</span><span class="sxs-lookup"><span data-stu-id="83dc1-119">Update the user current settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="83dc1-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="83dc1-120">Properties</span></span>

| <span data-ttu-id="83dc1-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="83dc1-121">Property</span></span>     | <span data-ttu-id="83dc1-122">Тип</span><span class="sxs-lookup"><span data-stu-id="83dc1-122">Type</span></span>   |<span data-ttu-id="83dc1-123">Описание</span><span class="sxs-lookup"><span data-stu-id="83dc1-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="83dc1-124">contributionToContentDiscoveryDisabled</span><span class="sxs-lookup"><span data-stu-id="83dc1-124">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="83dc1-125">Логический</span><span class="sxs-lookup"><span data-stu-id="83dc1-125">Boolean</span></span>|<span data-ttu-id="83dc1-126">Если задано значение true, делегированный доступ к API [trending](insights-trending.md) пользователя отключен.</span><span class="sxs-lookup"><span data-stu-id="83dc1-126">When set to true, the delegate access to the user's [trending](insights-trending.md) API is disabled.</span></span> <span data-ttu-id="83dc1-127">Если задано значение true, документы в Office Delve пользователя отключены.</span><span class="sxs-lookup"><span data-stu-id="83dc1-127">When set to true, documents in the user's Office Delve are disabled.</span></span> <span data-ttu-id="83dc1-128">Установка значения true влияет на релевантность содержимого, отображаемого в Office 365, например в рекомендуемых сайтах на домашней странице SharePoint и в представлении "Обнаружение" в OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="83dc1-128">When set to true, the relevancy of the content displayed in Office 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected.</span></span> <span data-ttu-id="83dc1-129">Пользователи могут управлять этим параметром в [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span><span class="sxs-lookup"><span data-stu-id="83dc1-129">Users can control this setting in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span> |
|<span data-ttu-id="83dc1-130">contributionToContentDiscoveryAsOrganizationDisabled</span><span class="sxs-lookup"><span data-stu-id="83dc1-130">contributionToContentDiscoveryAsOrganizationDisabled</span></span>|<span data-ttu-id="83dc1-131">Логический</span><span class="sxs-lookup"><span data-stu-id="83dc1-131">Boolean</span></span>|<span data-ttu-id="83dc1-132">Отображает [параметр на уровне организации](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff), управляющий делегированным доступом к API [trending](insights-trending.md).</span><span class="sxs-lookup"><span data-stu-id="83dc1-132">Reflects the [organization level setting](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff) controlling delegate access to the [trending](insights-trending.md) API.</span></span> <span data-ttu-id="83dc1-133">Если задано значение true, у организации отсутствует доступ к Office Delve.</span><span class="sxs-lookup"><span data-stu-id="83dc1-133">When set to true, the organization doesn't have access to Office Delve.</span></span> <span data-ttu-id="83dc1-134">Это влияет для всей организации на релевантность содержимого, отображаемого в Office 365, например в рекомендуемых сайтах на домашней странице SharePoint и в представлении "Обнаружение" в OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="83dc1-134">The relevancy of the content displayed in Office 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected for the whole organization.</span></span> <span data-ttu-id="83dc1-135">Этот параметр доступен только для чтения и может изменяться только администраторами в [Центре администрирования SharePoint](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span><span class="sxs-lookup"><span data-stu-id="83dc1-135">This setting is read-only and can only be changed by administrators in the [SharePoint admin center](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="83dc1-136">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="83dc1-136">JSON representation</span></span>

<span data-ttu-id="83dc1-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="83dc1-137">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userSettings"
}-->
```json
{
  "contributionToContentDiscoveryDisabled": false,
  "contributionToContentDiscoveryAsOrganizationDisabled": false
}

```
