---
title: Тип ресурса userSettings
description: 'Параметры текущего пользователя для поиска контента. '
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1b3852afc1a4ff790f6be92e39b359ec55230c2f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519500"
---
# <a name="usersettings-resource-type"></a><span data-ttu-id="4c314-103">Тип ресурса userSettings</span><span class="sxs-lookup"><span data-stu-id="4c314-103">userSettings resource type</span></span>

<span data-ttu-id="4c314-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4c314-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c314-105">Параметры текущего пользователя для поиска контента.</span><span class="sxs-lookup"><span data-stu-id="4c314-105">The current user settings for content discovery.</span></span> <span data-ttu-id="4c314-106">Сведения о получении и обновлении параметров пользователя см. в статьях [Получение параметров](../api/usersettings-get.md) и [Обновление параметров](../api/usersettings-update.md).</span><span class="sxs-lookup"><span data-stu-id="4c314-106">To learn how to get or update user settings, see [Get settings](../api/usersettings-get.md) and [Update settings](../api/usersettings-update.md).</span></span>

<span data-ttu-id="4c314-107">Этот ресурс поддерживает:</span><span class="sxs-lookup"><span data-stu-id="4c314-107">This resource supports:</span></span>

- <span data-ttu-id="4c314-108">Проверку участия пользователя и организации пользователя в поиске содержимого.</span><span class="sxs-lookup"><span data-stu-id="4c314-108">Checking whether a user and the user's organization contribute to content discovery.</span></span>
- <span data-ttu-id="4c314-109">Включение и отключение поиска содержимого для конкретных пользователей.</span><span class="sxs-lookup"><span data-stu-id="4c314-109">Disabling or enabling content discovery for specific users.</span></span> <span data-ttu-id="4c314-110">При этом также отключаются документы в Office Delve.</span><span class="sxs-lookup"><span data-stu-id="4c314-110">This also disables documents in Office Delve.</span></span>

## <a name="methods"></a><span data-ttu-id="4c314-111">Методы</span><span class="sxs-lookup"><span data-stu-id="4c314-111">Methods</span></span>
| <span data-ttu-id="4c314-112">Метод</span><span class="sxs-lookup"><span data-stu-id="4c314-112">Method</span></span>       | <span data-ttu-id="4c314-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4c314-113">Return Type</span></span>  |<span data-ttu-id="4c314-114">Описание</span><span class="sxs-lookup"><span data-stu-id="4c314-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4c314-115">Получение параметров пользователя</span><span class="sxs-lookup"><span data-stu-id="4c314-115">Get user settings</span></span>](../api/usersettings-get.md) |[<span data-ttu-id="4c314-116">userSettings</span><span class="sxs-lookup"><span data-stu-id="4c314-116">userSettings</span></span>](../resources/usersettings.md)| <span data-ttu-id="4c314-117">Получение параметров пользователя и организации.</span><span class="sxs-lookup"><span data-stu-id="4c314-117">Get the user and organization settings.</span></span> |
|[<span data-ttu-id="4c314-118">Обновление параметров пользователя</span><span class="sxs-lookup"><span data-stu-id="4c314-118">Update user settings</span></span>](../api/usersettings-update.md) |[<span data-ttu-id="4c314-119">userSettings</span><span class="sxs-lookup"><span data-stu-id="4c314-119">userSettings</span></span>](../resources/usersettings.md)| <span data-ttu-id="4c314-120">Обновление текущих параметров пользователя.</span><span class="sxs-lookup"><span data-stu-id="4c314-120">Update the user current settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="4c314-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="4c314-121">Properties</span></span>

| <span data-ttu-id="4c314-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c314-122">Property</span></span>     | <span data-ttu-id="4c314-123">Тип</span><span class="sxs-lookup"><span data-stu-id="4c314-123">Type</span></span>   |<span data-ttu-id="4c314-124">Описание</span><span class="sxs-lookup"><span data-stu-id="4c314-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4c314-125">contributionToContentDiscoveryDisabled</span><span class="sxs-lookup"><span data-stu-id="4c314-125">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="4c314-126">Логический</span><span class="sxs-lookup"><span data-stu-id="4c314-126">Boolean</span></span>|<span data-ttu-id="4c314-127">Если задано значение true, делегированный доступ к API [trending](insights-trending.md) пользователя отключен.</span><span class="sxs-lookup"><span data-stu-id="4c314-127">When set to true, the delegate access to the user's [trending](insights-trending.md) API is disabled.</span></span> <span data-ttu-id="4c314-128">Если задано значение true, документы в Office Delve пользователя отключены.</span><span class="sxs-lookup"><span data-stu-id="4c314-128">When set to true, documents in the user's Office Delve are disabled.</span></span> <span data-ttu-id="4c314-129">Установка значения true влияет на релевантность содержимого, отображаемого в Office 365, например в рекомендуемых сайтах на домашней странице SharePoint и в представлении "Обнаружение" в OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="4c314-129">When set to true, the relevancy of the content displayed in Office 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected.</span></span> <span data-ttu-id="4c314-130">Пользователи могут управлять этим параметром в [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span><span class="sxs-lookup"><span data-stu-id="4c314-130">Users can control this setting in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span> |
|<span data-ttu-id="4c314-131">contributionToContentDiscoveryAsOrganizationDisabled</span><span class="sxs-lookup"><span data-stu-id="4c314-131">contributionToContentDiscoveryAsOrganizationDisabled</span></span>|<span data-ttu-id="4c314-132">Логический</span><span class="sxs-lookup"><span data-stu-id="4c314-132">Boolean</span></span>|<span data-ttu-id="4c314-133">Отображает [параметр на уровне организации](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff), управляющий делегированным доступом к API [trending](insights-trending.md).</span><span class="sxs-lookup"><span data-stu-id="4c314-133">Reflects the [organization level setting](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff) controlling delegate access to the [trending](insights-trending.md) API.</span></span> <span data-ttu-id="4c314-134">Если задано значение true, у организации отсутствует доступ к Office Delve.</span><span class="sxs-lookup"><span data-stu-id="4c314-134">When set to true, the organization doesn't have access to Office Delve.</span></span> <span data-ttu-id="4c314-135">Это влияет для всей организации на релевантность содержимого, отображаемого в Office 365, например в рекомендуемых сайтах на домашней странице SharePoint и в представлении "Обнаружение" в OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="4c314-135">The relevancy of the content displayed in Office 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected for the whole organization.</span></span> <span data-ttu-id="4c314-136">Этот параметр доступен только для чтения и может изменяться только администраторами в [Центре администрирования SharePoint](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span><span class="sxs-lookup"><span data-stu-id="4c314-136">This setting is read-only and can only be changed by administrators in the [SharePoint admin center](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span></span>|

## <a name="relationships"></a><span data-ttu-id="4c314-137">Связи</span><span class="sxs-lookup"><span data-stu-id="4c314-137">Relationships</span></span>

| <span data-ttu-id="4c314-138">Связь</span><span class="sxs-lookup"><span data-stu-id="4c314-138">Relationship</span></span> | <span data-ttu-id="4c314-139">Тип</span><span class="sxs-lookup"><span data-stu-id="4c314-139">Type</span></span> | <span data-ttu-id="4c314-140">Описание</span><span class="sxs-lookup"><span data-stu-id="4c314-140">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="4c314-141">шифтпреференцес</span><span class="sxs-lookup"><span data-stu-id="4c314-141">shiftPreferences</span></span>|[<span data-ttu-id="4c314-142">шифтпреференцес</span><span class="sxs-lookup"><span data-stu-id="4c314-142">shiftPreferences</span></span>](shiftpreferences.md)| <span data-ttu-id="4c314-143">Настройки смены для пользователя.</span><span class="sxs-lookup"><span data-stu-id="4c314-143">The shift preferences for the user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4c314-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4c314-144">JSON representation</span></span>

<span data-ttu-id="4c314-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4c314-145">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userSettings",
  "baseType": "microsoft.graph.entity"
}-->
```json
{
  "contributionToContentDiscoveryDisabled": false,
  "contributionToContentDiscoveryAsOrganizationDisabled": false
}

```
