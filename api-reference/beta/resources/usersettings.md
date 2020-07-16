---
title: Тип ресурса userSettings
description: 'Параметры текущего пользователя для поиска контента. '
author: krbain
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8d44c21c1d41214aec8661fe696179b6976765b4
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897787"
---
# <a name="usersettings-resource-type"></a><span data-ttu-id="5198b-103">Тип ресурса userSettings</span><span class="sxs-lookup"><span data-stu-id="5198b-103">userSettings resource type</span></span>

<span data-ttu-id="5198b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5198b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5198b-105">Параметры, представляющие предпочтения пользователя для [региональных языковых стандартов и языков](../resources/regionalandlanguagesettings.md), для [планирования расписаний](../resources/shiftpreferences.md), а также для [анализа и обнаружения контента](../resources/officegraphinsights.md).</span><span class="sxs-lookup"><span data-stu-id="5198b-105">Settings that represent a user’s preferences for [regional locale and languages](../resources/regionalandlanguagesettings.md), for [shift scheduling](../resources/shiftpreferences.md), and for [insights and content discovery](../resources/officegraphinsights.md).</span></span>

<span data-ttu-id="5198b-106">Управление настройками на основе языкового стандарта пользователя:</span><span class="sxs-lookup"><span data-stu-id="5198b-106">Manage user's locale-based preferences:</span></span> 
  - <span data-ttu-id="5198b-107">Определение языка и региональных форматов, предпочитаемых пользователем для просмотра приложений.</span><span class="sxs-lookup"><span data-stu-id="5198b-107">Determining what language and regional formatting a user prefers to view applications with.</span></span>
  - <span data-ttu-id="5198b-108">Обновление языков и региональных параметров форматирования пользователя.</span><span class="sxs-lookup"><span data-stu-id="5198b-108">Updating a user's language and regional formatting preferences.</span></span>

<span data-ttu-id="5198b-109">Управление настройками рабочей смены пользователя:</span><span class="sxs-lookup"><span data-stu-id="5198b-109">Manage user's work shift preferences:</span></span> 
  - <span data-ttu-id="5198b-110">Проверка того, можно ли назначить пользователя для смены по расписанию.</span><span class="sxs-lookup"><span data-stu-id="5198b-110">Checking whether a user can be assigned to shifts in a schedule.</span></span>
  - <span data-ttu-id="5198b-111">Обновление предпочтений пользователя при смене.</span><span class="sxs-lookup"><span data-stu-id="5198b-111">Updating a user's shift preferences.</span></span>
  
<span data-ttu-id="5198b-112">Включение обнаружения контента и аналитической информации, ориентированной на документы:</span><span class="sxs-lookup"><span data-stu-id="5198b-112">Enable discovery of content and document-centric insights:</span></span>
  - <span data-ttu-id="5198b-113">Проверку участия пользователя и организации пользователя в поиске содержимого.</span><span class="sxs-lookup"><span data-stu-id="5198b-113">Checking whether a user and the user's organization contribute to content discovery.</span></span>
  - <span data-ttu-id="5198b-114">Включение и отключение поиска содержимого для конкретных пользователей.</span><span class="sxs-lookup"><span data-stu-id="5198b-114">Disabling or enabling content discovery for specific users.</span></span> <span data-ttu-id="5198b-115">При этом также отключаются документы в Office Delve.</span><span class="sxs-lookup"><span data-stu-id="5198b-115">This also disables documents in Office Delve.</span></span>

<span data-ttu-id="5198b-116">Сведения о получении и обновлении параметров пользователя см. в статьях [Получение параметров](../api/usersettings-get.md) и [Обновление параметров](../api/usersettings-update.md).</span><span class="sxs-lookup"><span data-stu-id="5198b-116">To learn how to get or update user settings, see [Get settings](../api/usersettings-get.md) and [Update settings](../api/usersettings-update.md).</span></span>

> [!NOTE]
> <span data-ttu-id="5198b-117">Эта конечная точка работает только с пользователями.</span><span class="sxs-lookup"><span data-stu-id="5198b-117">This endpoint works only with users.</span></span> <span data-ttu-id="5198b-118">Вы не можете использовать эту конечную точку с контактами.</span><span class="sxs-lookup"><span data-stu-id="5198b-118">You can't use this endpoint with contacts.</span></span>

## <a name="methods"></a><span data-ttu-id="5198b-119">Методы</span><span class="sxs-lookup"><span data-stu-id="5198b-119">Methods</span></span>
| <span data-ttu-id="5198b-120">Метод</span><span class="sxs-lookup"><span data-stu-id="5198b-120">Method</span></span>       | <span data-ttu-id="5198b-121">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5198b-121">Return Type</span></span>  |<span data-ttu-id="5198b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="5198b-122">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5198b-123">Получение параметров пользователя</span><span class="sxs-lookup"><span data-stu-id="5198b-123">Get user settings</span></span>](../api/usersettings-get.md) |[<span data-ttu-id="5198b-124">userSettings</span><span class="sxs-lookup"><span data-stu-id="5198b-124">userSettings</span></span>](../resources/usersettings.md)| <span data-ttu-id="5198b-125">Получение параметров пользователя и организации.</span><span class="sxs-lookup"><span data-stu-id="5198b-125">Get the user and organization settings.</span></span> |
|[<span data-ttu-id="5198b-126">Обновление параметров пользователя</span><span class="sxs-lookup"><span data-stu-id="5198b-126">Update user settings</span></span>](../api/usersettings-update.md) |[<span data-ttu-id="5198b-127">userSettings</span><span class="sxs-lookup"><span data-stu-id="5198b-127">userSettings</span></span>](../resources/usersettings.md)| <span data-ttu-id="5198b-128">Обновление текущих параметров пользователя.</span><span class="sxs-lookup"><span data-stu-id="5198b-128">Update the user current settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="5198b-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="5198b-129">Properties</span></span>

| <span data-ttu-id="5198b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5198b-130">Property</span></span>     | <span data-ttu-id="5198b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5198b-131">Type</span></span>   |<span data-ttu-id="5198b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5198b-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5198b-133">contributionToContentDiscoveryDisabled</span><span class="sxs-lookup"><span data-stu-id="5198b-133">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="5198b-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="5198b-134">Boolean</span></span>|<span data-ttu-id="5198b-135">Если задано значение true, делегированный доступ к API [trending](insights-trending.md) пользователя отключен.</span><span class="sxs-lookup"><span data-stu-id="5198b-135">When set to true, the delegate access to the user's [trending](insights-trending.md) API is disabled.</span></span> <span data-ttu-id="5198b-136">Если задано значение true, документы в Office Delve пользователя отключены.</span><span class="sxs-lookup"><span data-stu-id="5198b-136">When set to true, documents in the user's Office Delve are disabled.</span></span> <span data-ttu-id="5198b-137">Если задано значение true, то релевантность содержимого, отображаемого в Microsoft 365, например в разделе Рекомендуемые сайты в SharePoint Home и представление "Обнаружение" в OneDrive для бизнеса влияет.</span><span class="sxs-lookup"><span data-stu-id="5198b-137">When set to true, the relevancy of the content displayed in Microsoft 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected.</span></span> <span data-ttu-id="5198b-138">Пользователи могут управлять этим параметром в [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span><span class="sxs-lookup"><span data-stu-id="5198b-138">Users can control this setting in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span> |
|<span data-ttu-id="5198b-139">contributionToContentDiscoveryAsOrganizationDisabled</span><span class="sxs-lookup"><span data-stu-id="5198b-139">contributionToContentDiscoveryAsOrganizationDisabled</span></span>|<span data-ttu-id="5198b-140">Логический</span><span class="sxs-lookup"><span data-stu-id="5198b-140">Boolean</span></span>|<span data-ttu-id="5198b-141">Отображает [параметр на уровне организации](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff), управляющий делегированным доступом к API [trending](insights-trending.md).</span><span class="sxs-lookup"><span data-stu-id="5198b-141">Reflects the [organization level setting](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff) controlling delegate access to the [trending](insights-trending.md) API.</span></span> <span data-ttu-id="5198b-142">Если задано значение true, у организации отсутствует доступ к Office Delve.</span><span class="sxs-lookup"><span data-stu-id="5198b-142">When set to true, the organization doesn't have access to Office Delve.</span></span> <span data-ttu-id="5198b-143">Релевантность содержимого, отображаемого в Microsoft 365, например в разделе Рекомендуемые сайты в SharePoint Home, а представление обнаружения в OneDrive для бизнеса влияет на всю организацию.</span><span class="sxs-lookup"><span data-stu-id="5198b-143">The relevancy of the content displayed in Microsoft 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected for the whole organization.</span></span> <span data-ttu-id="5198b-144">Этот параметр доступен только для чтения и может изменяться только администраторами в [Центре администрирования SharePoint](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span><span class="sxs-lookup"><span data-stu-id="5198b-144">This setting is read-only and can only be changed by administrators in the [SharePoint admin center](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span></span>|

## <a name="relationships"></a><span data-ttu-id="5198b-145">Связи</span><span class="sxs-lookup"><span data-stu-id="5198b-145">Relationships</span></span>

| <span data-ttu-id="5198b-146">Связь</span><span class="sxs-lookup"><span data-stu-id="5198b-146">Relationship</span></span> | <span data-ttu-id="5198b-147">Тип</span><span class="sxs-lookup"><span data-stu-id="5198b-147">Type</span></span> | <span data-ttu-id="5198b-148">Описание</span><span class="sxs-lookup"><span data-stu-id="5198b-148">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="5198b-149">шифтпреференцес</span><span class="sxs-lookup"><span data-stu-id="5198b-149">shiftPreferences</span></span>|[<span data-ttu-id="5198b-150">шифтпреференцес</span><span class="sxs-lookup"><span data-stu-id="5198b-150">shiftPreferences</span></span>](shiftpreferences.md)| <span data-ttu-id="5198b-151">Настройки смены для пользователя.</span><span class="sxs-lookup"><span data-stu-id="5198b-151">The shift preferences for the user.</span></span> |
|<span data-ttu-id="5198b-152">регионаландлангуажесеттингс</span><span class="sxs-lookup"><span data-stu-id="5198b-152">regionalAndLanguageSettings</span></span>|[<span data-ttu-id="5198b-153">регионаландлангуажесеттингс</span><span class="sxs-lookup"><span data-stu-id="5198b-153">regionalAndLanguageSettings</span></span>](regionalandlanguagesettings.md)| <span data-ttu-id="5198b-154">Предпочтения пользователя для языков, региональных стандартов и форматирования даты и времени.</span><span class="sxs-lookup"><span data-stu-id="5198b-154">The user's preferences for languages, regional locale and date/time formatting.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5198b-155">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="5198b-155">JSON representation</span></span>

<span data-ttu-id="5198b-156">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5198b-156">Here is a JSON representation of the resource.</span></span>
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
