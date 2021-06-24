---
title: Тип ресурса userSettings
description: 'Параметры текущего пользователя для поиска контента. '
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: a16ab96bb04f6d7dfc4f9ceff29f49dc7d348d23
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53108875"
---
# <a name="usersettings-resource-type"></a><span data-ttu-id="1f93c-103">Тип ресурса userSettings</span><span class="sxs-lookup"><span data-stu-id="1f93c-103">userSettings resource type</span></span>

<span data-ttu-id="1f93c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f93c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f93c-105">Параметры, которые представляют предпочтения пользователя для регионального языка и [языков,](../resources/regionalandlanguagesettings.md)для планирования [смены,](../resources/shiftpreferences.md)для Delve и для [элементов.](../resources/officegraphinsights.md)</span><span class="sxs-lookup"><span data-stu-id="1f93c-105">Settings that represent a user’s preferences for [regional locale and languages](../resources/regionalandlanguagesettings.md), for [shift scheduling](../resources/shiftpreferences.md), for Delve and for [item insights](../resources/officegraphinsights.md).</span></span>

<span data-ttu-id="1f93c-106">Управление предпочтениями на основе локального пользователя:</span><span class="sxs-lookup"><span data-stu-id="1f93c-106">Manage user's locale-based preferences:</span></span> 
  - <span data-ttu-id="1f93c-107">Определение языка и регионального форматирования, с помощью чего пользователь предпочитает просматривать приложения.</span><span class="sxs-lookup"><span data-stu-id="1f93c-107">Determining what language and regional formatting a user prefers to view applications with.</span></span>
  - <span data-ttu-id="1f93c-108">Обновление языковых и региональных предпочтений форматирования пользователя.</span><span class="sxs-lookup"><span data-stu-id="1f93c-108">Updating a user's language and regional formatting preferences.</span></span>

<span data-ttu-id="1f93c-109">Управление предпочтениями смены работы пользователя:</span><span class="sxs-lookup"><span data-stu-id="1f93c-109">Manage user's work shift preferences:</span></span> 
  - <span data-ttu-id="1f93c-110">Проверка того, можно ли пользователю назначены изменения в расписании.</span><span class="sxs-lookup"><span data-stu-id="1f93c-110">Checking whether a user can be assigned to shifts in a schedule.</span></span>
  - <span data-ttu-id="1f93c-111">Обновление личных предпочтений пользователя.</span><span class="sxs-lookup"><span data-stu-id="1f93c-111">Updating a user's shift preferences.</span></span>
  
<span data-ttu-id="1f93c-112">Управление Delve доступностью:</span><span class="sxs-lookup"><span data-stu-id="1f93c-112">Manage Delve accessibility:</span></span>
  - <span data-ttu-id="1f93c-113">Проверка доступа пользователя и организации пользователя к Office Delve.</span><span class="sxs-lookup"><span data-stu-id="1f93c-113">Checking whether a user and the user's organization have access to Office Delve.</span></span>
  - <span data-ttu-id="1f93c-114">Отключение или включение документов в Office Delve для определенных пользователей.</span><span class="sxs-lookup"><span data-stu-id="1f93c-114">Disabling or enabling documents in Office Delve for specific users.</span></span> 

<span data-ttu-id="1f93c-115">Настройка видимости [itemInsights и](../resources/iteminsights.md) [собраний.](https://support.microsoft.com/en-us/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1)</span><span class="sxs-lookup"><span data-stu-id="1f93c-115">Configure the visibility of [itemInsights](../resources/iteminsights.md) and [meeting hours insights](https://support.microsoft.com/en-us/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1).</span></span> <span data-ttu-id="1f93c-116">ItemInsights являются производными между пользователями и другими элементами (например, документами или сайтами) в Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="1f93c-116">ItemInsights are derived between users and other items (such as documents or sites) in Microsoft 365:</span></span>
  - <span data-ttu-id="1f93c-117">Проверка включения элементов и часов собраний пользователя.</span><span class="sxs-lookup"><span data-stu-id="1f93c-117">Checking whether a user's item and meeting hours insights are enabled.</span></span>
  - <span data-ttu-id="1f93c-118">Отключение или включение данных о элементах и часах собраний для конкретного пользователя.</span><span class="sxs-lookup"><span data-stu-id="1f93c-118">Disabling or enabling item and meeting hours insights for specific user.</span></span>

<span data-ttu-id="1f93c-119">Сведения о получении и обновлении параметров пользователя см. в статьях [Получение параметров](../api/usersettings-get.md) и [Обновление параметров](../api/usersettings-update.md).</span><span class="sxs-lookup"><span data-stu-id="1f93c-119">To learn how to get or update user settings, see [Get settings](../api/usersettings-get.md) and [Update settings](../api/usersettings-update.md).</span></span>

> [!NOTE]
> <span data-ttu-id="1f93c-120">Эта конечная точка работает только с пользователями.</span><span class="sxs-lookup"><span data-stu-id="1f93c-120">This endpoint works only with users.</span></span> <span data-ttu-id="1f93c-121">Вы не можете использовать эту конечную точку с контактами.</span><span class="sxs-lookup"><span data-stu-id="1f93c-121">You can't use this endpoint with contacts.</span></span>

## <a name="methods"></a><span data-ttu-id="1f93c-122">Методы</span><span class="sxs-lookup"><span data-stu-id="1f93c-122">Methods</span></span>
| <span data-ttu-id="1f93c-123">Метод</span><span class="sxs-lookup"><span data-stu-id="1f93c-123">Method</span></span>       | <span data-ttu-id="1f93c-124">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1f93c-124">Return Type</span></span>  |<span data-ttu-id="1f93c-125">Описание</span><span class="sxs-lookup"><span data-stu-id="1f93c-125">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1f93c-126">Получение параметров пользователя</span><span class="sxs-lookup"><span data-stu-id="1f93c-126">Get user settings</span></span>](../api/usersettings-get.md) |[<span data-ttu-id="1f93c-127">userSettings</span><span class="sxs-lookup"><span data-stu-id="1f93c-127">userSettings</span></span>](../resources/usersettings.md)| <span data-ttu-id="1f93c-128">Получение параметров пользователя и организации.</span><span class="sxs-lookup"><span data-stu-id="1f93c-128">Get the user and organization settings.</span></span> |
|[<span data-ttu-id="1f93c-129">Обновление параметров пользователя</span><span class="sxs-lookup"><span data-stu-id="1f93c-129">Update user settings</span></span>](../api/usersettings-update.md) |[<span data-ttu-id="1f93c-130">userSettings</span><span class="sxs-lookup"><span data-stu-id="1f93c-130">userSettings</span></span>](../resources/usersettings.md)| <span data-ttu-id="1f93c-131">Обновление текущих параметров пользователя.</span><span class="sxs-lookup"><span data-stu-id="1f93c-131">Update the user current settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="1f93c-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="1f93c-132">Properties</span></span>

| <span data-ttu-id="1f93c-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="1f93c-133">Property</span></span>     | <span data-ttu-id="1f93c-134">Тип</span><span class="sxs-lookup"><span data-stu-id="1f93c-134">Type</span></span>   |<span data-ttu-id="1f93c-135">Описание</span><span class="sxs-lookup"><span data-stu-id="1f93c-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1f93c-136">contributionToContentDiscoveryDisabled</span><span class="sxs-lookup"><span data-stu-id="1f93c-136">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="1f93c-137">Логический</span><span class="sxs-lookup"><span data-stu-id="1f93c-137">Boolean</span></span>|<span data-ttu-id="1f93c-138">Если задано значение true, документы в Office Delve пользователя отключены.</span><span class="sxs-lookup"><span data-stu-id="1f93c-138">When set to true, documents in the user's Office Delve are disabled.</span></span> <span data-ttu-id="1f93c-139">Пользователи могут управлять этим параметром в [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span><span class="sxs-lookup"><span data-stu-id="1f93c-139">Users can control this setting in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span> |
|<span data-ttu-id="1f93c-140">contributionToContentDiscoveryAsOrganizationDisabled</span><span class="sxs-lookup"><span data-stu-id="1f93c-140">contributionToContentDiscoveryAsOrganizationDisabled</span></span>|<span data-ttu-id="1f93c-141">Логический</span><span class="sxs-lookup"><span data-stu-id="1f93c-141">Boolean</span></span>|<span data-ttu-id="1f93c-142">Отражает параметр [уровня Office Delve организации.](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff)</span><span class="sxs-lookup"><span data-stu-id="1f93c-142">Reflects the [Office Delve organization level setting](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff).</span></span> <span data-ttu-id="1f93c-143">Если задано значение true, у организации отсутствует доступ к Office Delve.</span><span class="sxs-lookup"><span data-stu-id="1f93c-143">When set to true, the organization doesn't have access to Office Delve.</span></span> <span data-ttu-id="1f93c-144">Этот параметр доступен только для чтения и может изменяться только администраторами в [Центре администрирования SharePoint](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span><span class="sxs-lookup"><span data-stu-id="1f93c-144">This setting is read-only and can only be changed by administrators in the [SharePoint admin center](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span></span>|

## <a name="relationships"></a><span data-ttu-id="1f93c-145">Отношения</span><span class="sxs-lookup"><span data-stu-id="1f93c-145">Relationships</span></span>

| <span data-ttu-id="1f93c-146">Связь</span><span class="sxs-lookup"><span data-stu-id="1f93c-146">Relationship</span></span> | <span data-ttu-id="1f93c-147">Тип</span><span class="sxs-lookup"><span data-stu-id="1f93c-147">Type</span></span> | <span data-ttu-id="1f93c-148">Описание</span><span class="sxs-lookup"><span data-stu-id="1f93c-148">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="1f93c-149">shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="1f93c-149">shiftPreferences</span></span>|[<span data-ttu-id="1f93c-150">shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="1f93c-150">shiftPreferences</span></span>](shiftpreferences.md)| <span data-ttu-id="1f93c-151">Параметры переноса для пользователя.</span><span class="sxs-lookup"><span data-stu-id="1f93c-151">The shift preferences for the user.</span></span> |
|<span data-ttu-id="1f93c-152">regionalAndLanguageSettings</span><span class="sxs-lookup"><span data-stu-id="1f93c-152">regionalAndLanguageSettings</span></span>|[<span data-ttu-id="1f93c-153">regionalAndLanguageSettings</span><span class="sxs-lookup"><span data-stu-id="1f93c-153">regionalAndLanguageSettings</span></span>](regionalandlanguagesettings.md)| <span data-ttu-id="1f93c-154">Предпочтения пользователя для языков, регионального языка и форматирования даты и времени.</span><span class="sxs-lookup"><span data-stu-id="1f93c-154">The user's preferences for languages, regional locale and date/time formatting.</span></span> |
|<span data-ttu-id="1f93c-155">itemInsights</span><span class="sxs-lookup"><span data-stu-id="1f93c-155">itemInsights</span></span>|[<span data-ttu-id="1f93c-156">userInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="1f93c-156">userInsightsSettings</span></span>](userinsightssettings.md)| <span data-ttu-id="1f93c-157">Параметры пользователя для видимости информации о часах собраний и сведения, полученные между пользователем и другими элементами в Microsoft 365, например документами или сайтами.</span><span class="sxs-lookup"><span data-stu-id="1f93c-157">The user's settings for the visibility of meeting hour insights, and insights derived between a user and other items in Microsoft 365, such as documents or sites.</span></span> <span data-ttu-id="1f93c-158">[Получите userInsightsSettings через](../api/userinsightssettings-get.md) это свойство навигации.</span><span class="sxs-lookup"><span data-stu-id="1f93c-158">[Get userInsightsSettings](../api/userinsightssettings-get.md) through this navigation property.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1f93c-159">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1f93c-159">JSON representation</span></span>

<span data-ttu-id="1f93c-160">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1f93c-160">Here is a JSON representation of the resource.</span></span>
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


