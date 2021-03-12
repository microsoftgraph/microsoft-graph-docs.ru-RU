---
title: Обновление параметров
description: 'Обновление свойств объекта settings. '
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: d2e1cd7107065bb03e7bd9ce89208d218776fd4d
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721336"
---
# <a name="update-settings"></a><span data-ttu-id="bd9d6-103">Обновление параметров</span><span class="sxs-lookup"><span data-stu-id="bd9d6-103">Update settings</span></span>

<span data-ttu-id="bd9d6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd9d6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bd9d6-105">Обновление свойств объекта [userSettings.](../resources/usersettings.md)</span><span class="sxs-lookup"><span data-stu-id="bd9d6-105">Update the properties of the [userSettings](../resources/usersettings.md) object.</span></span> <span data-ttu-id="bd9d6-106">Пользователи в одной организации могут иметь различные параметры в зависимости от их предпочтений или политик организации.</span><span class="sxs-lookup"><span data-stu-id="bd9d6-106">Users in the same organization can have different settings based on their preference or on the organization policies.</span></span> <span data-ttu-id="bd9d6-107">Чтобы получить текущие параметры пользователя, см. [текущие параметры пользователя.](usersettings-get.md)</span><span class="sxs-lookup"><span data-stu-id="bd9d6-107">To get the user current settings, see [current user settings](usersettings-get.md).</span></span> 

### <a name="batch-request"></a><span data-ttu-id="bd9d6-108">Пакетный запрос</span><span class="sxs-lookup"><span data-stu-id="bd9d6-108">Batch request</span></span>

<span data-ttu-id="bd9d6-109">Кроме того, можно отказать нескольким пользователям в Delve и отключить их вклад в запрос на контент для всей организации.</span><span class="sxs-lookup"><span data-stu-id="bd9d6-109">It's also possible to opt-out multiple users from Delve and disable their contribution on content relevancy for the whole organization through a batch request.</span></span>
<span data-ttu-id="bd9d6-110">Дополнительные дополнительные информации см. в серии [JSON.](/graph/json-batching)</span><span class="sxs-lookup"><span data-stu-id="bd9d6-110">To learn more, see [JSON batching](/graph/json-batching).</span></span>

><span data-ttu-id="bd9d6-111">**Важно.** Только члены группы [ролей](https://support.office.com/article/permissions-in-the-office-365-security-compliance-center-d10608af-7934-490a-818e-e68f17d0e9c1?ui=en-US&rs=en-US&ad=US) управления организацией могут обновлять несколько пользователей.</span><span class="sxs-lookup"><span data-stu-id="bd9d6-111">**Important**: Only members of the [organization management](https://support.office.com/article/permissions-in-the-office-365-security-compliance-center-d10608af-7934-490a-818e-e68f17d0e9c1?ui=en-US&rs=en-US&ad=US) role group can update multiple users.</span></span> 



## <a name="permissions"></a><span data-ttu-id="bd9d6-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bd9d6-112">Permissions</span></span>

<span data-ttu-id="bd9d6-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd9d6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd9d6-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bd9d6-115">Permission type</span></span>      | <span data-ttu-id="bd9d6-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bd9d6-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bd9d6-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bd9d6-117">Delegated (work or school account)</span></span> | <span data-ttu-id="bd9d6-118">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd9d6-118">User.ReadWrite, User.ReadWrite.All</span></span>   |
|<span data-ttu-id="bd9d6-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bd9d6-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd9d6-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd9d6-120">Not supported.</span></span>    |
|<span data-ttu-id="bd9d6-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bd9d6-121">Application</span></span> | <span data-ttu-id="bd9d6-122">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd9d6-122">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bd9d6-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bd9d6-123">HTTP request</span></span>

```http
PATCH /me/settings
```

<span data-ttu-id="bd9d6-124">Запрос с параметрами user id или userPrincipalName доступен только пользователю или пользователю с разрешениями User.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="bd9d6-124">Request with a 'user id' or 'userPrincipalName' is only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="bd9d6-125">Дополнительные сведения см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd9d6-125">To learn more, see [Permissions](/graph/permissions-reference).</span></span> 

```http
PATCH /users/{id | userPrincipalName}/settings/
```

## <a name="request-headers"></a><span data-ttu-id="bd9d6-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bd9d6-126">Request headers</span></span>

| <span data-ttu-id="bd9d6-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bd9d6-127">Header</span></span>       | <span data-ttu-id="bd9d6-128">Значение</span><span class="sxs-lookup"><span data-stu-id="bd9d6-128">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="bd9d6-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bd9d6-129">Authorization</span></span>  | <span data-ttu-id="bd9d6-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bd9d6-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bd9d6-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bd9d6-132">Content-Type</span></span>  | <span data-ttu-id="bd9d6-133">application/json</span><span class="sxs-lookup"><span data-stu-id="bd9d6-133">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bd9d6-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bd9d6-134">Request body</span></span>

<span data-ttu-id="bd9d6-p106">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="bd9d6-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="bd9d6-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="bd9d6-138">Property</span></span>     | <span data-ttu-id="bd9d6-139">Тип</span><span class="sxs-lookup"><span data-stu-id="bd9d6-139">Type</span></span>   |<span data-ttu-id="bd9d6-140">Описание</span><span class="sxs-lookup"><span data-stu-id="bd9d6-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bd9d6-141">contributionToContentDiscoveryDisabled</span><span class="sxs-lookup"><span data-stu-id="bd9d6-141">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="bd9d6-142">Логический</span><span class="sxs-lookup"><span data-stu-id="bd9d6-142">Boolean</span></span>|<span data-ttu-id="bd9d6-143">Установите для пользователя возможность отключения доступа делегатов к API [Trending](/graph/api/resources/insights-trending?view=graph-rest-1.0) и отключения доступа к документам в Office Delve для пользователя.</span><span class="sxs-lookup"><span data-stu-id="bd9d6-143">Set to true do disable delegate access to the [Trending](/graph/api/resources/insights-trending?view=graph-rest-1.0) API and to disable access to documents in Office Delve for the user.</span></span> <span data-ttu-id="bd9d6-144">Значение true также влияет на релевантность контента, отображаемого в Microsoft 365, например, рекомендуемые сайты в SharePoint Home и представление Discover в OneDrive для бизнеса показывают менее релевантные результаты.</span><span class="sxs-lookup"><span data-stu-id="bd9d6-144">Setting to true also affects the relevance of the content displayed in Microsoft 365 - for example, Suggested sites in SharePoint Home and the Discover view in OneDrive for Business show less relevant results.</span></span> <span data-ttu-id="bd9d6-145">Этот параметр отражает состояние управления [в Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span><span class="sxs-lookup"><span data-stu-id="bd9d6-145">This setting reflects the control state in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span>|

## <a name="example"></a><span data-ttu-id="bd9d6-146">Пример</span><span class="sxs-lookup"><span data-stu-id="bd9d6-146">Example</span></span> 

##### <a name="request"></a><span data-ttu-id="bd9d6-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="bd9d6-147">Request</span></span>

<span data-ttu-id="bd9d6-148">Вот пример запроса о том, как отключить пользователя из Delve и отключить его вклад в содержимого для всей организации.</span><span class="sxs-lookup"><span data-stu-id="bd9d6-148">Here is an example request on how to opt-out a user from Delve and disable his contribution on content relevancy for the whole organization.</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/me/settings
Content-type: application/json
Content-length: 37

{
  "contributionToContentDiscoveryDisabled": true
}
```

##### <a name="response"></a><span data-ttu-id="bd9d6-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd9d6-149">Response</span></span>

<span data-ttu-id="bd9d6-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bd9d6-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": true
}
```