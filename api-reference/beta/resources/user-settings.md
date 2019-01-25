---
title: параметры типа ресурсов
description: 'Параметры текущего пользователя. '
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 208d232af609f92d5924267ae26831b9929e357a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521098"
---
# <a name="settings-resource-type"></a><span data-ttu-id="61968-103">параметры типа ресурсов</span><span class="sxs-lookup"><span data-stu-id="61968-103">settings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61968-104">Параметры текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="61968-104">The current user settings.</span></span> <span data-ttu-id="61968-105">Чтобы узнать, как получить или обновить пользовательские параметры, обратитесь к разделу [получить параметры](../api/user-get-settings.md) и [обновление параметров](../api/user-update-settings.md).</span><span class="sxs-lookup"><span data-stu-id="61968-105">To learn how to get or update user settings, see [Get settings](../api/user-get-settings.md) and [Update settings](../api/user-update-settings.md).</span></span>

<span data-ttu-id="61968-106">Этот ресурс поддерживает:</span><span class="sxs-lookup"><span data-stu-id="61968-106">This resource supports:</span></span>

- <span data-ttu-id="61968-107">Проверка ли пользователь и организации пользователя "участие" для обнаружения контента.</span><span class="sxs-lookup"><span data-stu-id="61968-107">Checking whether a user and the user's organization contribute to content discovery.</span></span>
- <span data-ttu-id="61968-108">Отключение и Включение контента обнаружения для определенных пользователей.</span><span class="sxs-lookup"><span data-stu-id="61968-108">Disabling or enabling content discovery for specific users.</span></span> <span data-ttu-id="61968-109">Кроме того, отключаются документов в Office углубимся.</span><span class="sxs-lookup"><span data-stu-id="61968-109">This also disables documents in Office Delve.</span></span>

## <a name="methods"></a><span data-ttu-id="61968-110">Методы</span><span class="sxs-lookup"><span data-stu-id="61968-110">Methods</span></span>
| <span data-ttu-id="61968-111">Метод</span><span class="sxs-lookup"><span data-stu-id="61968-111">Method</span></span>       | <span data-ttu-id="61968-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="61968-112">Return Type</span></span>  |<span data-ttu-id="61968-113">Описание</span><span class="sxs-lookup"><span data-stu-id="61968-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="61968-114">Получение параметров пользователя</span><span class="sxs-lookup"><span data-stu-id="61968-114">[Get user settings](../api/user-get-settings.md)</span></span> |[<span data-ttu-id="61968-115">Settings</span><span class="sxs-lookup"><span data-stu-id="61968-115">settings</span></span>](../resources/user-settings.md)| <span data-ttu-id="61968-116">Получите параметры пользователей и организаций.</span><span class="sxs-lookup"><span data-stu-id="61968-116">Get the user and organization settings.</span></span> |
|[<span data-ttu-id="61968-117">Изменение параметров пользователей</span><span class="sxs-lookup"><span data-stu-id="61968-117">Update user settings</span></span>](../api/user-update-settings.md) |[<span data-ttu-id="61968-118">Settings</span><span class="sxs-lookup"><span data-stu-id="61968-118">settings</span></span>](../resources/user-settings.md)| <span data-ttu-id="61968-119">Обновление текущих параметров пользователя.</span><span class="sxs-lookup"><span data-stu-id="61968-119">Update the user current settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="61968-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="61968-120">Properties</span></span>

| <span data-ttu-id="61968-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="61968-121">Property</span></span>     | <span data-ttu-id="61968-122">Тип</span><span class="sxs-lookup"><span data-stu-id="61968-122">Type</span></span>   |<span data-ttu-id="61968-123">Описание</span><span class="sxs-lookup"><span data-stu-id="61968-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="61968-124">contributionToContentDiscoveryDisabled</span><span class="sxs-lookup"><span data-stu-id="61968-124">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="61968-125">Логическое</span><span class="sxs-lookup"><span data-stu-id="61968-125">Boolean</span></span>|<span data-ttu-id="61968-126">Если задано значение true, делегированный доступ для пользователя отключена [прибора](insights-trending.md) API.</span><span class="sxs-lookup"><span data-stu-id="61968-126">When set to true, the delegate access to the user's [trending](insights-trending.md) API is disabled.</span></span> <span data-ttu-id="61968-127">Если параметр имеет значение true, документов в углубимся Office пользователя отключены.</span><span class="sxs-lookup"><span data-stu-id="61968-127">When set to true, documents in the user's Office Delve are disabled.</span></span> <span data-ttu-id="61968-128">Если задано значение true, релевантность содержимое, отображаемое в Office 365, например в предлагаемые сайты в Домашняя страница SharePoint и влияет на представление обнаружения в OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="61968-128">When set to true, the relevancy of the content displayed in Office 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected.</span></span> <span data-ttu-id="61968-129">Пользователи могут управлять этим параметром [Углубимся Office](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span><span class="sxs-lookup"><span data-stu-id="61968-129">Users can control this setting in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span> |
|<span data-ttu-id="61968-130">contributionToContentDiscoveryAsOrganizationDisabled</span><span class="sxs-lookup"><span data-stu-id="61968-130">contributionToContentDiscoveryAsOrganizationDisabled</span></span>|<span data-ttu-id="61968-131">Логическое</span><span class="sxs-lookup"><span data-stu-id="61968-131">Boolean</span></span>|<span data-ttu-id="61968-132">Отражает [уровень организации](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff) управление делегированный доступ, [прибора](insights-trending.md) API.</span><span class="sxs-lookup"><span data-stu-id="61968-132">Reflects the [organization level setting](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff) controlling delegate access to the [trending](insights-trending.md) API.</span></span> <span data-ttu-id="61968-133">Если значение равно true, организации не имеет доступа к углубимся Office.</span><span class="sxs-lookup"><span data-stu-id="61968-133">When set to true, the organization doesn't have access to Office Delve.</span></span> <span data-ttu-id="61968-134">Релевантность содержимое, отображаемое в Office 365, например в предлагаемые сайты в Домашняя страница SharePoint и представления обнаружения в OneDrive для бизнеса контролируется для всей организации.</span><span class="sxs-lookup"><span data-stu-id="61968-134">The relevancy of the content displayed in Office 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected for the whole organization.</span></span> <span data-ttu-id="61968-135">Этот параметр доступен только для чтения и может быть изменено только администраторами в [центре администрирования SharePoint](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span><span class="sxs-lookup"><span data-stu-id="61968-135">This setting is read-only and can only be changed by administrators in the [SharePoint admin center](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="61968-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="61968-136">JSON representation</span></span>

<span data-ttu-id="61968-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="61968-137">Here is a JSON representation of the resource.</span></span>

```json
{
  "contributionToContentDiscoveryDisabled": false,
  "contributionToContentDiscoveryAsOrganizationDisabled": false
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/user-settings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
