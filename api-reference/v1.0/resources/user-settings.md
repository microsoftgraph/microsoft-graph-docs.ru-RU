---
title: Тип ресурса settings
description: 'Текущие параметры пользователя. '
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6a1cf4deb5da03daeb9d90e03ea63fa069a0701e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033525"
---
# <a name="settings-resource-type"></a><span data-ttu-id="f2dc2-103">Тип ресурса settings</span><span class="sxs-lookup"><span data-stu-id="f2dc2-103">settings resource type</span></span>

<span data-ttu-id="f2dc2-104">Текущие параметры пользователя.</span><span class="sxs-lookup"><span data-stu-id="f2dc2-104">The current user settings.</span></span> <span data-ttu-id="f2dc2-105">Сведения о получении и обновлении параметров пользователя см. в статьях [Получение параметров](../api/user-get-settings.md) и [Обновление параметров](../api/user-update-settings.md).</span><span class="sxs-lookup"><span data-stu-id="f2dc2-105">To learn how to get or update user settings, see [Get settings](../api/user-get-settings.md) and [Update settings](../api/user-update-settings.md).</span></span>

<span data-ttu-id="f2dc2-106">Этот ресурс поддерживает:</span><span class="sxs-lookup"><span data-stu-id="f2dc2-106">This resource supports:</span></span>

- <span data-ttu-id="f2dc2-107">Проверку участия пользователя и организации пользователя в поиске содержимого.</span><span class="sxs-lookup"><span data-stu-id="f2dc2-107">Checking whether a user and the user's organization contribute to content discovery.</span></span>
- <span data-ttu-id="f2dc2-108">Включение и отключение поиска содержимого для конкретных пользователей.</span><span class="sxs-lookup"><span data-stu-id="f2dc2-108">Disabling or enabling content discovery for specific users.</span></span> <span data-ttu-id="f2dc2-109">При этом также отключаются документы в Office Delve.</span><span class="sxs-lookup"><span data-stu-id="f2dc2-109">This also disables documents in Office Delve.</span></span>

## <a name="methods"></a><span data-ttu-id="f2dc2-110">Методы</span><span class="sxs-lookup"><span data-stu-id="f2dc2-110">Methods</span></span>
| <span data-ttu-id="f2dc2-111">Метод</span><span class="sxs-lookup"><span data-stu-id="f2dc2-111">Method</span></span>       | <span data-ttu-id="f2dc2-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f2dc2-112">Return Type</span></span>  |<span data-ttu-id="f2dc2-113">Описание</span><span class="sxs-lookup"><span data-stu-id="f2dc2-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f2dc2-114">Получение параметров пользователя</span><span class="sxs-lookup"><span data-stu-id="f2dc2-114">Get user settings</span></span>](../api/user-get-settings.md) |[<span data-ttu-id="f2dc2-115">settings</span><span class="sxs-lookup"><span data-stu-id="f2dc2-115">settings</span></span>](../resources/user-settings.md)| <span data-ttu-id="f2dc2-116">Получение параметров пользователя и организации.</span><span class="sxs-lookup"><span data-stu-id="f2dc2-116">Get the user and organization settings.</span></span> |
|[<span data-ttu-id="f2dc2-117">Обновление параметров пользователя</span><span class="sxs-lookup"><span data-stu-id="f2dc2-117">Update user settings</span></span>](../api/user-update-settings.md) |[<span data-ttu-id="f2dc2-118">settings</span><span class="sxs-lookup"><span data-stu-id="f2dc2-118">settings</span></span>](../resources/user-settings.md)| <span data-ttu-id="f2dc2-119">Обновление текущих параметров пользователя.</span><span class="sxs-lookup"><span data-stu-id="f2dc2-119">Update the user current settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="f2dc2-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="f2dc2-120">Properties</span></span>

| <span data-ttu-id="f2dc2-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="f2dc2-121">Property</span></span>     | <span data-ttu-id="f2dc2-122">Тип</span><span class="sxs-lookup"><span data-stu-id="f2dc2-122">Type</span></span>   |<span data-ttu-id="f2dc2-123">Описание</span><span class="sxs-lookup"><span data-stu-id="f2dc2-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f2dc2-124">contributionToContentDiscoveryDisabled</span><span class="sxs-lookup"><span data-stu-id="f2dc2-124">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="f2dc2-125">Логический</span><span class="sxs-lookup"><span data-stu-id="f2dc2-125">Boolean</span></span>|<span data-ttu-id="f2dc2-126">Если задано значение true, делегированный доступ к API [trending](/graph/api/resources/insights-trending?view=graph-rest-beta) пользователя отключен.</span><span class="sxs-lookup"><span data-stu-id="f2dc2-126">When set to true, the delegate access to the user's [trending](/graph/api/resources/insights-trending?view=graph-rest-beta) API is disabled.</span></span> <span data-ttu-id="f2dc2-127">Если задано значение true, документы в Office Delve пользователя отключены.</span><span class="sxs-lookup"><span data-stu-id="f2dc2-127">When set to true, documents in the user's Office Delve are disabled.</span></span> <span data-ttu-id="f2dc2-128">Установка значения true влияет на релевантность содержимого, отображаемого в Office 365, например в рекомендуемых сайтах на домашней странице SharePoint и в представлении "Обнаружение" в OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="f2dc2-128">When set to true, the relevancy of the content displayed in Office 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected.</span></span> <span data-ttu-id="f2dc2-129">Пользователи могут управлять этим параметром в [Office Delve](https://support.office.com/ru-RU/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span><span class="sxs-lookup"><span data-stu-id="f2dc2-129">Users can control this setting in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span> |
|<span data-ttu-id="f2dc2-130">contributionToContentDiscoveryAsOrganizationDisabled</span><span class="sxs-lookup"><span data-stu-id="f2dc2-130">contributionToContentDiscoveryAsOrganizationDisabled</span></span>|<span data-ttu-id="f2dc2-131">Логический</span><span class="sxs-lookup"><span data-stu-id="f2dc2-131">Boolean</span></span>|<span data-ttu-id="f2dc2-132">Отображает [параметр на уровне организации](https://support.office.com/ru-RU/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff), управляющий делегированным доступом к API [trending](/graph/api/resources/insights-trending?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="f2dc2-132">Reflects the [organization level setting](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff) controlling delegate access to the [trending](/graph/api/resources/insights-trending?view=graph-rest-beta) API.</span></span> <span data-ttu-id="f2dc2-133">Если задано значение true, у организации отсутствует доступ к Office Delve.</span><span class="sxs-lookup"><span data-stu-id="f2dc2-133">When set to true, the organization doesn't have access to Office Delve.</span></span> <span data-ttu-id="f2dc2-134">Это влияет для всей организации на релевантность содержимого, отображаемого в Office 365, например в рекомендуемых сайтах на домашней странице SharePoint и в представлении "Обнаружение" в OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="f2dc2-134">The relevancy of the content displayed in Office 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected for the whole organization.</span></span> <span data-ttu-id="f2dc2-135">Этот параметр доступен только для чтения и может изменяться только администраторами в [Центре администрирования SharePoint](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span><span class="sxs-lookup"><span data-stu-id="f2dc2-135">This setting is read-only and can only be changed by administrators in the [SharePoint admin center](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span></span>|


## <a name="json-representation"></a><span data-ttu-id="f2dc2-136">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f2dc2-136">JSON representation</span></span>

<span data-ttu-id="f2dc2-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f2dc2-137">Here is a JSON representation of the resource.</span></span>

```json
{
  "contributionToContentDiscoveryDisabled": false,
  "contributionToContentDiscoveryAsOrganizationDisabled": false
}

```
