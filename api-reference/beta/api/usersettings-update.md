---
title: Обновление параметров
description: 'Обновление свойств объекта settings. '
author: krbain
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 1638c5716256988dc5bc36999ab3bebf7f068ee2
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896464"
---
# <a name="update-settings"></a><span data-ttu-id="4ee2e-103">Обновление параметров</span><span class="sxs-lookup"><span data-stu-id="4ee2e-103">Update settings</span></span>

<span data-ttu-id="4ee2e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ee2e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ee2e-105">Обновление свойств объекта [усерсеттингс](../resources/usersettings.md) .</span><span class="sxs-lookup"><span data-stu-id="4ee2e-105">Update the properties of the [userSettings](../resources/usersettings.md) object.</span></span> <span data-ttu-id="4ee2e-106">Пользователи в одной организации могут иметь различные параметры в зависимости от их предпочтения или политики Организации.</span><span class="sxs-lookup"><span data-stu-id="4ee2e-106">Users in the same organization can have different settings based on their preference or on the organization policies.</span></span> <span data-ttu-id="4ee2e-107">Чтобы получить текущие параметры пользователя, просмотрите [параметры текущей учетной записи пользователя](usersettings-get.md).</span><span class="sxs-lookup"><span data-stu-id="4ee2e-107">To get the user current settings, see [current user settings](usersettings-get.md).</span></span> 


### <a name="batch-request"></a><span data-ttu-id="4ee2e-108">Пакетный запрос</span><span class="sxs-lookup"><span data-stu-id="4ee2e-108">Batch request</span></span>

<span data-ttu-id="4ee2e-109">Кроме того, можно отказаться от использования нескольких пользователей из delve и отказаться от их вклада в релевантность содержимого для всей Организации с помощью пакетного запроса.</span><span class="sxs-lookup"><span data-stu-id="4ee2e-109">It's also possible to opt-out multiple users from Delve and disable their contribution on content relevancy for the whole organization through a batch request.</span></span>
<span data-ttu-id="4ee2e-110">Для получения дополнительных сведений см [Пакетная обработка JSON](/graph/json-batching).</span><span class="sxs-lookup"><span data-stu-id="4ee2e-110">To learn more, see [JSON batching](/graph/json-batching).</span></span>

><span data-ttu-id="4ee2e-111">**Важно!** только члены группы ролей " [Управление организацией](https://support.office.com/article/permissions-in-the-office-365-security-compliance-center-d10608af-7934-490a-818e-e68f17d0e9c1?ui=en-US&rs=en-US&ad=US) " могут обновлять нескольких пользователей.</span><span class="sxs-lookup"><span data-stu-id="4ee2e-111">**Important**: Only members of the [organization management](https://support.office.com/article/permissions-in-the-office-365-security-compliance-center-d10608af-7934-490a-818e-e68f17d0e9c1?ui=en-US&rs=en-US&ad=US) role group can update multiple users.</span></span> 



## <a name="permissions"></a><span data-ttu-id="4ee2e-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4ee2e-112">Permissions</span></span>

<span data-ttu-id="4ee2e-113">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="4ee2e-113">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="4ee2e-114">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ee2e-114">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ee2e-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4ee2e-115">Permission type</span></span>      | <span data-ttu-id="4ee2e-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4ee2e-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ee2e-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4ee2e-117">Delegated (work or school account)</span></span> | <span data-ttu-id="4ee2e-118">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="4ee2e-118">User.ReadWrite, User.ReadWrite.All</span></span>   |
|<span data-ttu-id="4ee2e-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4ee2e-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ee2e-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ee2e-120">Not supported.</span></span>    |
|<span data-ttu-id="4ee2e-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4ee2e-121">Application</span></span> | <span data-ttu-id="4ee2e-122">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ee2e-122">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4ee2e-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4ee2e-123">HTTP request</span></span>

```http
PATCH /me/settings
```

<span data-ttu-id="4ee2e-124">Запрос с параметрами user id или userPrincipalName доступен только пользователю или пользователю с разрешениями User.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="4ee2e-124">Request with a 'user id' or 'userPrincipalName' is only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="4ee2e-125">Дополнительные сведения см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ee2e-125">To learn more, see [Permissions](/graph/permissions-reference).</span></span> 

```http
PATCH /users/{id | userPrincipalName}/settings/
```

## <a name="request-headers"></a><span data-ttu-id="4ee2e-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4ee2e-126">Request headers</span></span>

| <span data-ttu-id="4ee2e-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4ee2e-127">Header</span></span>       | <span data-ttu-id="4ee2e-128">Значение</span><span class="sxs-lookup"><span data-stu-id="4ee2e-128">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="4ee2e-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4ee2e-129">Authorization</span></span>  | <span data-ttu-id="4ee2e-130">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="4ee2e-130">Bearer {token}.</span></span> <span data-ttu-id="4ee2e-131">Required.</span><span class="sxs-lookup"><span data-stu-id="4ee2e-131">Required.</span></span>  |
| <span data-ttu-id="4ee2e-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4ee2e-132">Content-Type</span></span>  | <span data-ttu-id="4ee2e-133">application/json</span><span class="sxs-lookup"><span data-stu-id="4ee2e-133">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4ee2e-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4ee2e-134">Request body</span></span>

<span data-ttu-id="4ee2e-135">In the request body, supply the values for relevant fields that should be updated.</span><span class="sxs-lookup"><span data-stu-id="4ee2e-135">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="4ee2e-136">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span><span class="sxs-lookup"><span data-stu-id="4ee2e-136">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="4ee2e-137">For best performance you shouldn't include existing values that haven't changed.</span><span class="sxs-lookup"><span data-stu-id="4ee2e-137">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4ee2e-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="4ee2e-138">Property</span></span>     | <span data-ttu-id="4ee2e-139">Тип</span><span class="sxs-lookup"><span data-stu-id="4ee2e-139">Type</span></span>   |<span data-ttu-id="4ee2e-140">Описание</span><span class="sxs-lookup"><span data-stu-id="4ee2e-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4ee2e-141">contributionToContentDiscoveryDisabled</span><span class="sxs-lookup"><span data-stu-id="4ee2e-141">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="4ee2e-142">Логический</span><span class="sxs-lookup"><span data-stu-id="4ee2e-142">Boolean</span></span>|<span data-ttu-id="4ee2e-143">Установите значение true, чтобы запретить представителю доступ к API [тенденций](../resources/insights-trending.md) и отключить доступ к документам в Office delve для пользователя.</span><span class="sxs-lookup"><span data-stu-id="4ee2e-143">Set to true do disable delegate access to the [Trending](../resources/insights-trending.md) API and to disable access to documents in Office Delve for the user.</span></span> <span data-ttu-id="4ee2e-144">Значение true также влияет на релевантность контента, отображаемого в Microsoft 365 — например, Рекомендуемые сайты в SharePoint Home и представление обнаружение в OneDrive для бизнеса содержат менее релевантные результаты.</span><span class="sxs-lookup"><span data-stu-id="4ee2e-144">Setting to true also affects the relevance of the content displayed in Microsoft 365 - for example, Suggested sites in SharePoint Home and the Discover view in OneDrive for Business show less relevant results.</span></span> <span data-ttu-id="4ee2e-145">Этот параметр отражает состояние элемента управления в [Office delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span><span class="sxs-lookup"><span data-stu-id="4ee2e-145">This setting reflects the control state in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span>|

## <a name="example"></a><span data-ttu-id="4ee2e-146">Пример</span><span class="sxs-lookup"><span data-stu-id="4ee2e-146">Example</span></span> 

##### <a name="request"></a><span data-ttu-id="4ee2e-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ee2e-147">Request</span></span>

<span data-ttu-id="4ee2e-148">Ниже приведен пример запроса на отказаться от участия пользователя в delve и отказаться от его участия в релевантности контента для всей Организации.</span><span class="sxs-lookup"><span data-stu-id="4ee2e-148">Here is an example request on how to opt-out a user from Delve and disable his contribution on content relevancy for the whole organization.</span></span>

```http
PATCH https://graph.microsoft.com/beta/me/settings
Content-type: application/json
Content-length: 37

{
  "contributionToContentDiscoveryDisabled": true
}
```

##### <a name="response"></a><span data-ttu-id="4ee2e-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ee2e-149">Response</span></span>

<span data-ttu-id="4ee2e-150">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="4ee2e-150">Here is an example of the response.</span></span> <span data-ttu-id="4ee2e-151">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="4ee2e-151">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="4ee2e-152">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="4ee2e-152">All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": true
}
```

