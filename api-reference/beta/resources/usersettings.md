---
title: Тип ресурса userSettings
description: 'Параметры текущего пользователя для поиска контента. '
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 12c75691b5b0515fbf8ef49b54ce1e4a0b806c2c
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761774"
---
# <a name="usersettings-resource-type"></a><span data-ttu-id="c34df-103">Тип ресурса userSettings</span><span class="sxs-lookup"><span data-stu-id="c34df-103">userSettings resource type</span></span>

<span data-ttu-id="c34df-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c34df-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c34df-105">Параметры, которые представляют предпочтения пользователя для регионального языка и [языков,](../resources/regionalandlanguagesettings.md)для планирования [смены,](../resources/shiftpreferences.md)а также для анализа и [обнаружения контента.](../resources/officegraphinsights.md)</span><span class="sxs-lookup"><span data-stu-id="c34df-105">Settings that represent a user’s preferences for [regional locale and languages](../resources/regionalandlanguagesettings.md), for [shift scheduling](../resources/shiftpreferences.md), and for [insights and content discovery](../resources/officegraphinsights.md).</span></span>

<span data-ttu-id="c34df-106">Управление предпочтениями на основе локального пользователя:</span><span class="sxs-lookup"><span data-stu-id="c34df-106">Manage user's locale-based preferences:</span></span> 
  - <span data-ttu-id="c34df-107">Определение языка и регионального форматирования, с помощью чего пользователь предпочитает просматривать приложения.</span><span class="sxs-lookup"><span data-stu-id="c34df-107">Determining what language and regional formatting a user prefers to view applications with.</span></span>
  - <span data-ttu-id="c34df-108">Обновление языковых и региональных предпочтений форматирования пользователя.</span><span class="sxs-lookup"><span data-stu-id="c34df-108">Updating a user's language and regional formatting preferences.</span></span>

<span data-ttu-id="c34df-109">Управление предпочтениями смены работы пользователя:</span><span class="sxs-lookup"><span data-stu-id="c34df-109">Manage user's work shift preferences:</span></span> 
  - <span data-ttu-id="c34df-110">Проверка того, можно ли пользователю назначены изменения в расписании.</span><span class="sxs-lookup"><span data-stu-id="c34df-110">Checking whether a user can be assigned to shifts in a schedule.</span></span>
  - <span data-ttu-id="c34df-111">Обновление личных предпочтений пользователя.</span><span class="sxs-lookup"><span data-stu-id="c34df-111">Updating a user's shift preferences.</span></span>
  
<span data-ttu-id="c34df-112">Включить обнаружение контента и документов, ориентированных на анализ:</span><span class="sxs-lookup"><span data-stu-id="c34df-112">Enable discovery of content and document-centric insights:</span></span>
  - <span data-ttu-id="c34df-113">Проверку участия пользователя и организации пользователя в поиске содержимого.</span><span class="sxs-lookup"><span data-stu-id="c34df-113">Checking whether a user and the user's organization contribute to content discovery.</span></span>
  - <span data-ttu-id="c34df-114">Включение и отключение поиска содержимого для конкретных пользователей.</span><span class="sxs-lookup"><span data-stu-id="c34df-114">Disabling or enabling content discovery for specific users.</span></span> <span data-ttu-id="c34df-115">При этом также отключаются документы в Office Delve.</span><span class="sxs-lookup"><span data-stu-id="c34df-115">This also disables documents in Office Delve.</span></span>

<span data-ttu-id="c34df-116">Сведения о получении и обновлении параметров пользователя см. в статьях [Получение параметров](../api/usersettings-get.md) и [Обновление параметров](../api/usersettings-update.md).</span><span class="sxs-lookup"><span data-stu-id="c34df-116">To learn how to get or update user settings, see [Get settings](../api/usersettings-get.md) and [Update settings](../api/usersettings-update.md).</span></span>

> [!NOTE]
> <span data-ttu-id="c34df-117">Эта конечная точка работает только с пользователями.</span><span class="sxs-lookup"><span data-stu-id="c34df-117">This endpoint works only with users.</span></span> <span data-ttu-id="c34df-118">Вы не можете использовать эту конечную точку с контактами.</span><span class="sxs-lookup"><span data-stu-id="c34df-118">You can't use this endpoint with contacts.</span></span>

## <a name="methods"></a><span data-ttu-id="c34df-119">Методы</span><span class="sxs-lookup"><span data-stu-id="c34df-119">Methods</span></span>
| <span data-ttu-id="c34df-120">Метод</span><span class="sxs-lookup"><span data-stu-id="c34df-120">Method</span></span>       | <span data-ttu-id="c34df-121">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c34df-121">Return Type</span></span>  |<span data-ttu-id="c34df-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c34df-122">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c34df-123">Получение параметров пользователя</span><span class="sxs-lookup"><span data-stu-id="c34df-123">Get user settings</span></span>](../api/usersettings-get.md) |[<span data-ttu-id="c34df-124">userSettings</span><span class="sxs-lookup"><span data-stu-id="c34df-124">userSettings</span></span>](../resources/usersettings.md)| <span data-ttu-id="c34df-125">Получение параметров пользователя и организации.</span><span class="sxs-lookup"><span data-stu-id="c34df-125">Get the user and organization settings.</span></span> |
|[<span data-ttu-id="c34df-126">Обновление параметров пользователя</span><span class="sxs-lookup"><span data-stu-id="c34df-126">Update user settings</span></span>](../api/usersettings-update.md) |[<span data-ttu-id="c34df-127">userSettings</span><span class="sxs-lookup"><span data-stu-id="c34df-127">userSettings</span></span>](../resources/usersettings.md)| <span data-ttu-id="c34df-128">Обновление текущих параметров пользователя.</span><span class="sxs-lookup"><span data-stu-id="c34df-128">Update the user current settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="c34df-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="c34df-129">Properties</span></span>

| <span data-ttu-id="c34df-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c34df-130">Property</span></span>     | <span data-ttu-id="c34df-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c34df-131">Type</span></span>   |<span data-ttu-id="c34df-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c34df-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c34df-133">contributionToContentDiscoveryDisabled</span><span class="sxs-lookup"><span data-stu-id="c34df-133">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="c34df-134">Логический</span><span class="sxs-lookup"><span data-stu-id="c34df-134">Boolean</span></span>|<span data-ttu-id="c34df-135">Если задано значение true, делегированный доступ к API [trending](insights-trending.md) пользователя отключен.</span><span class="sxs-lookup"><span data-stu-id="c34df-135">When set to true, the delegate access to the user's [trending](insights-trending.md) API is disabled.</span></span> <span data-ttu-id="c34df-136">Если задано значение true, документы в Office Delve пользователя отключены.</span><span class="sxs-lookup"><span data-stu-id="c34df-136">When set to true, documents in the user's Office Delve are disabled.</span></span> <span data-ttu-id="c34df-137">Установка значения true влияет на релевантность содержимого, отображаемого в Microsoft 365, например в рекомендуемых сайтах на домашней странице SharePoint и в представлении "Обнаружение" в OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="c34df-137">When set to true, the relevancy of the content displayed in Microsoft 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected.</span></span> <span data-ttu-id="c34df-138">Пользователи могут управлять этим параметром в [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span><span class="sxs-lookup"><span data-stu-id="c34df-138">Users can control this setting in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span> |
|<span data-ttu-id="c34df-139">contributionToContentDiscoveryAsOrganizationDisabled</span><span class="sxs-lookup"><span data-stu-id="c34df-139">contributionToContentDiscoveryAsOrganizationDisabled</span></span>|<span data-ttu-id="c34df-140">Логический</span><span class="sxs-lookup"><span data-stu-id="c34df-140">Boolean</span></span>|<span data-ttu-id="c34df-141">Отображает [параметр на уровне организации](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff), управляющий делегированным доступом к API [trending](insights-trending.md).</span><span class="sxs-lookup"><span data-stu-id="c34df-141">Reflects the [organization level setting](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff) controlling delegate access to the [trending](insights-trending.md) API.</span></span> <span data-ttu-id="c34df-142">Если задано значение true, у организации отсутствует доступ к Office Delve.</span><span class="sxs-lookup"><span data-stu-id="c34df-142">When set to true, the organization doesn't have access to Office Delve.</span></span> <span data-ttu-id="c34df-143">Это влияет на релевантность содержимого, отображаемого в Microsoft 365 для всей организации, например в рекомендуемых сайтах на домашней странице SharePoint и в представлении "Обнаружение" в OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="c34df-143">The relevancy of the content displayed in Microsoft 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected for the whole organization.</span></span> <span data-ttu-id="c34df-144">Этот параметр доступен только для чтения и может изменяться только администраторами в [Центре администрирования SharePoint](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span><span class="sxs-lookup"><span data-stu-id="c34df-144">This setting is read-only and can only be changed by administrators in the [SharePoint admin center](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span></span>|

## <a name="relationships"></a><span data-ttu-id="c34df-145">Отношения</span><span class="sxs-lookup"><span data-stu-id="c34df-145">Relationships</span></span>

| <span data-ttu-id="c34df-146">Связь</span><span class="sxs-lookup"><span data-stu-id="c34df-146">Relationship</span></span> | <span data-ttu-id="c34df-147">Тип</span><span class="sxs-lookup"><span data-stu-id="c34df-147">Type</span></span> | <span data-ttu-id="c34df-148">Описание</span><span class="sxs-lookup"><span data-stu-id="c34df-148">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="c34df-149">shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="c34df-149">shiftPreferences</span></span>|[<span data-ttu-id="c34df-150">shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="c34df-150">shiftPreferences</span></span>](shiftpreferences.md)| <span data-ttu-id="c34df-151">Параметры переноса для пользователя.</span><span class="sxs-lookup"><span data-stu-id="c34df-151">The shift preferences for the user.</span></span> |
|<span data-ttu-id="c34df-152">regionalAndLanguageSettings</span><span class="sxs-lookup"><span data-stu-id="c34df-152">regionalAndLanguageSettings</span></span>|[<span data-ttu-id="c34df-153">regionalAndLanguageSettings</span><span class="sxs-lookup"><span data-stu-id="c34df-153">regionalAndLanguageSettings</span></span>](regionalandlanguagesettings.md)| <span data-ttu-id="c34df-154">Предпочтения пользователя для языков, регионального языка и форматирования даты и времени.</span><span class="sxs-lookup"><span data-stu-id="c34df-154">The user's preferences for languages, regional locale and date/time formatting.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c34df-155">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c34df-155">JSON representation</span></span>

<span data-ttu-id="c34df-156">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c34df-156">Here is a JSON representation of the resource.</span></span>
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


