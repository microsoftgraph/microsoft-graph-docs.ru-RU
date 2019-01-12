---
title: параметры типа ресурсов
description: 'Параметры текущего пользователя. '
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 433824e715940f2309619a0467179ef99ee3daec
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981408"
---
# <a name="settings-resource-type"></a><span data-ttu-id="774d2-103">параметры типа ресурсов</span><span class="sxs-lookup"><span data-stu-id="774d2-103">settings resource type</span></span>

<span data-ttu-id="774d2-104">Параметры текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="774d2-104">The current user settings.</span></span> <span data-ttu-id="774d2-105">Чтобы узнать, как получить или обновить пользовательские параметры, обратитесь к разделу [получить параметры](../api/user-get-settings.md) и [обновление параметров](../api/user-update-settings.md).</span><span class="sxs-lookup"><span data-stu-id="774d2-105">To learn how to get or update user settings, see [Get settings](../api/user-get-settings.md) and [Update settings](../api/user-update-settings.md).</span></span>

<span data-ttu-id="774d2-106">Этот ресурс поддерживает:</span><span class="sxs-lookup"><span data-stu-id="774d2-106">This resource supports:</span></span>

- <span data-ttu-id="774d2-107">Проверка ли пользователь и организации пользователя "участие" для обнаружения контента.</span><span class="sxs-lookup"><span data-stu-id="774d2-107">Checking whether a user and the user's organization contribute to content discovery.</span></span>
- <span data-ttu-id="774d2-108">Отключение и Включение контента обнаружения для определенных пользователей.</span><span class="sxs-lookup"><span data-stu-id="774d2-108">Disabling or enabling content discovery for specific users.</span></span> <span data-ttu-id="774d2-109">Кроме того, отключаются документов в Office углубимся.</span><span class="sxs-lookup"><span data-stu-id="774d2-109">This also disables documents in Office Delve.</span></span>

## <a name="methods"></a><span data-ttu-id="774d2-110">Методы</span><span class="sxs-lookup"><span data-stu-id="774d2-110">Methods</span></span>
| <span data-ttu-id="774d2-111">Метод</span><span class="sxs-lookup"><span data-stu-id="774d2-111">Method</span></span>       | <span data-ttu-id="774d2-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="774d2-112">Return Type</span></span>  |<span data-ttu-id="774d2-113">Описание</span><span class="sxs-lookup"><span data-stu-id="774d2-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="774d2-114">Получение параметров пользователя</span><span class="sxs-lookup"><span data-stu-id="774d2-114">Get user settings</span></span>](../api/user-get-settings.md) |[<span data-ttu-id="774d2-115">Параметры</span><span class="sxs-lookup"><span data-stu-id="774d2-115">settings</span></span>](../resources/user-settings.md)| <span data-ttu-id="774d2-116">Получите параметры пользователей и организаций.</span><span class="sxs-lookup"><span data-stu-id="774d2-116">Get the user and organization settings.</span></span> |
|[<span data-ttu-id="774d2-117">Изменение параметров пользователей</span><span class="sxs-lookup"><span data-stu-id="774d2-117">Update user settings</span></span>](../api/user-update-settings.md) |[<span data-ttu-id="774d2-118">Параметры</span><span class="sxs-lookup"><span data-stu-id="774d2-118">settings</span></span>](../resources/user-settings.md)| <span data-ttu-id="774d2-119">Обновление текущих параметров пользователя.</span><span class="sxs-lookup"><span data-stu-id="774d2-119">Update the user current settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="774d2-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="774d2-120">Properties</span></span>

| <span data-ttu-id="774d2-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="774d2-121">Property</span></span>     | <span data-ttu-id="774d2-122">Тип</span><span class="sxs-lookup"><span data-stu-id="774d2-122">Type</span></span>   |<span data-ttu-id="774d2-123">Описание</span><span class="sxs-lookup"><span data-stu-id="774d2-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="774d2-124">contributionToContentDiscoveryDisabled</span><span class="sxs-lookup"><span data-stu-id="774d2-124">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="774d2-125">Логический</span><span class="sxs-lookup"><span data-stu-id="774d2-125">Boolean</span></span>|<span data-ttu-id="774d2-126">Если задано значение true, делегированный доступ для пользователя отключена [прибора](/graph/api/resources/insights-trending?view=graph-rest-beta) API.</span><span class="sxs-lookup"><span data-stu-id="774d2-126">When set to true, the delegate access to the user's [trending](/graph/api/resources/insights-trending?view=graph-rest-beta) API is disabled.</span></span> <span data-ttu-id="774d2-127">Если параметр имеет значение true, документов в углубимся Office пользователя отключены.</span><span class="sxs-lookup"><span data-stu-id="774d2-127">When set to true, documents in the user's Office Delve are disabled.</span></span> <span data-ttu-id="774d2-128">Если задано значение true, релевантность содержимое, отображаемое в Office 365, например в предлагаемые сайты в Домашняя страница SharePoint и влияет на представление обнаружения в OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="774d2-128">When set to true, the relevancy of the content displayed in Office 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected.</span></span> <span data-ttu-id="774d2-129">Пользователи могут управлять этим параметром [Углубимся Office](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span><span class="sxs-lookup"><span data-stu-id="774d2-129">Users can control this setting in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span> |
|<span data-ttu-id="774d2-130">contributionToContentDiscoveryAsOrganizationDisabled</span><span class="sxs-lookup"><span data-stu-id="774d2-130">contributionToContentDiscoveryAsOrganizationDisabled</span></span>|<span data-ttu-id="774d2-131">Логический</span><span class="sxs-lookup"><span data-stu-id="774d2-131">Boolean</span></span>|<span data-ttu-id="774d2-132">Отражает [уровень организации](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff) управление делегированный доступ, [прибора](/graph/api/resources/insights-trending?view=graph-rest-beta) API.</span><span class="sxs-lookup"><span data-stu-id="774d2-132">Reflects the [organization level setting](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff) controlling delegate access to the [trending](/graph/api/resources/insights-trending?view=graph-rest-beta) API.</span></span> <span data-ttu-id="774d2-133">Если значение равно true, организации не имеет доступа к углубимся Office.</span><span class="sxs-lookup"><span data-stu-id="774d2-133">When set to true, the organization doesn't have access to Office Delve.</span></span> <span data-ttu-id="774d2-134">Релевантность содержимое, отображаемое в Office 365, например в предлагаемые сайты в Домашняя страница SharePoint и представления обнаружения в OneDrive для бизнеса контролируется для всей организации.</span><span class="sxs-lookup"><span data-stu-id="774d2-134">The relevancy of the content displayed in Office 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected for the whole organization.</span></span> <span data-ttu-id="774d2-135">Этот параметр доступен только для чтения и может быть изменено только администраторами в [центре администрирования SharePoint](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span><span class="sxs-lookup"><span data-stu-id="774d2-135">This setting is read-only and can only be changed by administrators in the [SharePoint admin center](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span></span>|


## <a name="json-representation"></a><span data-ttu-id="774d2-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="774d2-136">JSON representation</span></span>

<span data-ttu-id="774d2-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="774d2-137">Here is a JSON representation of the resource.</span></span>

```json
{
  "contributionToContentDiscoveryDisabled": false,
  "contributionToContentDiscoveryAsOrganizationDisabled": false
}

```
