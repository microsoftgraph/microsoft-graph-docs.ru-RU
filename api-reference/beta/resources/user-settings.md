---
title: Тип ресурса "Параметры"
description: 'Параметры текущего пользователя. '
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 208d232af609f92d5924267ae26831b9929e357a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554270"
---
# <a name="settings-resource-type"></a><span data-ttu-id="295a3-103">Тип ресурса "Параметры"</span><span class="sxs-lookup"><span data-stu-id="295a3-103">settings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="295a3-104">Параметры текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="295a3-104">The current user settings.</span></span> <span data-ttu-id="295a3-105">Чтобы узнать, как получить или обновить параметры пользователя, ознакомьтесь со [статьЕй получение параметров](../api/user-get-settings.md) и [Обновление параметров](../api/user-update-settings.md).</span><span class="sxs-lookup"><span data-stu-id="295a3-105">To learn how to get or update user settings, see [Get settings](../api/user-get-settings.md) and [Update settings](../api/user-update-settings.md).</span></span>

<span data-ttu-id="295a3-106">Этот ресурс поддерживает:</span><span class="sxs-lookup"><span data-stu-id="295a3-106">This resource supports:</span></span>

- <span data-ttu-id="295a3-107">Проверка того, участвует ли пользователь и пользователь в Организации для обнаружения контента.</span><span class="sxs-lookup"><span data-stu-id="295a3-107">Checking whether a user and the user's organization contribute to content discovery.</span></span>
- <span data-ttu-id="295a3-108">Отключение или Включение обнаружения контента для определенных пользователей.</span><span class="sxs-lookup"><span data-stu-id="295a3-108">Disabling or enabling content discovery for specific users.</span></span> <span data-ttu-id="295a3-109">При этом также отключаются документы в Office delve.</span><span class="sxs-lookup"><span data-stu-id="295a3-109">This also disables documents in Office Delve.</span></span>

## <a name="methods"></a><span data-ttu-id="295a3-110">Методы</span><span class="sxs-lookup"><span data-stu-id="295a3-110">Methods</span></span>
| <span data-ttu-id="295a3-111">Метод</span><span class="sxs-lookup"><span data-stu-id="295a3-111">Method</span></span>       | <span data-ttu-id="295a3-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="295a3-112">Return Type</span></span>  |<span data-ttu-id="295a3-113">Описание</span><span class="sxs-lookup"><span data-stu-id="295a3-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="295a3-114">Получение параметров пользователя</span><span class="sxs-lookup"><span data-stu-id="295a3-114">Get user settings</span></span>](../api/user-get-settings.md) |[<span data-ttu-id="295a3-115">settings</span><span class="sxs-lookup"><span data-stu-id="295a3-115">settings</span></span>](../resources/user-settings.md)| <span data-ttu-id="295a3-116">Получение параметров пользователя и Организации.</span><span class="sxs-lookup"><span data-stu-id="295a3-116">Get the user and organization settings.</span></span> |
|[<span data-ttu-id="295a3-117">Обновление параметров пользователя</span><span class="sxs-lookup"><span data-stu-id="295a3-117">Update user settings</span></span>](../api/user-update-settings.md) |[<span data-ttu-id="295a3-118">settings</span><span class="sxs-lookup"><span data-stu-id="295a3-118">settings</span></span>](../resources/user-settings.md)| <span data-ttu-id="295a3-119">Обновление текущих параметров пользователя.</span><span class="sxs-lookup"><span data-stu-id="295a3-119">Update the user current settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="295a3-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="295a3-120">Properties</span></span>

| <span data-ttu-id="295a3-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="295a3-121">Property</span></span>     | <span data-ttu-id="295a3-122">Тип</span><span class="sxs-lookup"><span data-stu-id="295a3-122">Type</span></span>   |<span data-ttu-id="295a3-123">Описание</span><span class="sxs-lookup"><span data-stu-id="295a3-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="295a3-124">Контрибутионтоконтентдисковеридисаблед</span><span class="sxs-lookup"><span data-stu-id="295a3-124">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="295a3-125">Логический</span><span class="sxs-lookup"><span data-stu-id="295a3-125">Boolean</span></span>|<span data-ttu-id="295a3-126">Если задано значение true, доступ представителя к API [трендов](insights-trending.md) пользователя отключен.</span><span class="sxs-lookup"><span data-stu-id="295a3-126">When set to true, the delegate access to the user's [trending](insights-trending.md) API is disabled.</span></span> <span data-ttu-id="295a3-127">Если задано значение true, документы в Office delve пользователя отключены.</span><span class="sxs-lookup"><span data-stu-id="295a3-127">When set to true, documents in the user's Office Delve are disabled.</span></span> <span data-ttu-id="295a3-128">Если задано значение true, то релевантность содержимого, отображаемого в Office 365, например в разделе Рекомендуемые сайты в SharePoint Home и представление "Обнаружение" в OneDrive для бизнеса влияет.</span><span class="sxs-lookup"><span data-stu-id="295a3-128">When set to true, the relevancy of the content displayed in Office 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected.</span></span> <span data-ttu-id="295a3-129">Пользователи могут управлять этим параметром в [Office delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span><span class="sxs-lookup"><span data-stu-id="295a3-129">Users can control this setting in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span> |
|<span data-ttu-id="295a3-130">Контрибутионтоконтентдисковерясорганизатиондисаблед</span><span class="sxs-lookup"><span data-stu-id="295a3-130">contributionToContentDiscoveryAsOrganizationDisabled</span></span>|<span data-ttu-id="295a3-131">Логический</span><span class="sxs-lookup"><span data-stu-id="295a3-131">Boolean</span></span>|<span data-ttu-id="295a3-132">Отражает [параметр уровня Организации](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff) , контролирующий доступ делегата [](insights-trending.md) к API тенденций.</span><span class="sxs-lookup"><span data-stu-id="295a3-132">Reflects the [organization level setting](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff) controlling delegate access to the [trending](insights-trending.md) API.</span></span> <span data-ttu-id="295a3-133">Если задано значение true, Организация не имеет доступа к Office delve.</span><span class="sxs-lookup"><span data-stu-id="295a3-133">When set to true, the organization doesn't have access to Office Delve.</span></span> <span data-ttu-id="295a3-134">Релевантность контента, отображаемого в Office 365, например в разделе Рекомендуемые сайты в SharePoint Home, а представление обнаружения в OneDrive для бизнеса влияет на всю организацию.</span><span class="sxs-lookup"><span data-stu-id="295a3-134">The relevancy of the content displayed in Office 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected for the whole organization.</span></span> <span data-ttu-id="295a3-135">Этот параметр доступен только для чтения и может быть изменен только администраторами в [центре администрирования SharePoint](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span><span class="sxs-lookup"><span data-stu-id="295a3-135">This setting is read-only and can only be changed by administrators in the [SharePoint admin center](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="295a3-136">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="295a3-136">JSON representation</span></span>

<span data-ttu-id="295a3-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="295a3-137">Here is a JSON representation of the resource.</span></span>

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
