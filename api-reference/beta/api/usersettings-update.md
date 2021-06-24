---
title: Обновление параметров
description: 'Обновление свойств объекта settings. '
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: f776bd5ac5dad802a8c977cbe32842e619c74434
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53107762"
---
# <a name="update-settings"></a><span data-ttu-id="233bc-103">Обновление параметров</span><span class="sxs-lookup"><span data-stu-id="233bc-103">Update settings</span></span>

<span data-ttu-id="233bc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="233bc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="233bc-105">Обновление свойств объекта [userSettings.](../resources/usersettings.md)</span><span class="sxs-lookup"><span data-stu-id="233bc-105">Update the properties of the [userSettings](../resources/usersettings.md) object.</span></span> <span data-ttu-id="233bc-106">Пользователи в одной организации могут иметь различные параметры в зависимости от их предпочтений или политик организации.</span><span class="sxs-lookup"><span data-stu-id="233bc-106">Users in the same organization can have different settings based on their preference or on the organization policies.</span></span> <span data-ttu-id="233bc-107">Чтобы получить текущие параметры пользователя, см. [текущие параметры пользователя.](usersettings-get.md)</span><span class="sxs-lookup"><span data-stu-id="233bc-107">To get the user current settings, see [current user settings](usersettings-get.md).</span></span> 


### <a name="batch-request"></a><span data-ttu-id="233bc-108">Пакетный запрос</span><span class="sxs-lookup"><span data-stu-id="233bc-108">Batch request</span></span>

<span data-ttu-id="233bc-109">Кроме того, можно отказать нескольким пользователям в доступе Delve пакетным запросом.</span><span class="sxs-lookup"><span data-stu-id="233bc-109">It's also possible to opt-out multiple users from Delve through a batch request.</span></span>
<span data-ttu-id="233bc-110">Дополнительные дополнительные информации см. в серии [JSON.](/graph/json-batching)</span><span class="sxs-lookup"><span data-stu-id="233bc-110">To learn more, see [JSON batching](/graph/json-batching).</span></span>

><span data-ttu-id="233bc-111">**Важно.** Только члены группы [ролей](https://support.office.com/article/permissions-in-the-office-365-security-compliance-center-d10608af-7934-490a-818e-e68f17d0e9c1?ui=en-US&rs=en-US&ad=US) управления организацией могут обновлять несколько пользователей.</span><span class="sxs-lookup"><span data-stu-id="233bc-111">**Important**: Only members of the [organization management](https://support.office.com/article/permissions-in-the-office-365-security-compliance-center-d10608af-7934-490a-818e-e68f17d0e9c1?ui=en-US&rs=en-US&ad=US) role group can update multiple users.</span></span> 



## <a name="permissions"></a><span data-ttu-id="233bc-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="233bc-112">Permissions</span></span>

<span data-ttu-id="233bc-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="233bc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="233bc-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="233bc-115">Permission type</span></span>      | <span data-ttu-id="233bc-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="233bc-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="233bc-117">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="233bc-117">Delegated (work or school account)</span></span> | <span data-ttu-id="233bc-118">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="233bc-118">User.ReadWrite, User.ReadWrite.All</span></span>   |
|<span data-ttu-id="233bc-119">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="233bc-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="233bc-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="233bc-120">Not supported.</span></span>    |
|<span data-ttu-id="233bc-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="233bc-121">Application</span></span> | <span data-ttu-id="233bc-122">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="233bc-122">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="233bc-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="233bc-123">HTTP request</span></span>

```http
PATCH /me/settings
```

<span data-ttu-id="233bc-124">Запрос с параметрами user id или userPrincipalName доступен только пользователю или пользователю с разрешениями User.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="233bc-124">Request with a 'user id' or 'userPrincipalName' is only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="233bc-125">Дополнительные сведения см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="233bc-125">To learn more, see [Permissions](/graph/permissions-reference).</span></span> 

```http
PATCH /users/{id | userPrincipalName}/settings/
```

## <a name="request-headers"></a><span data-ttu-id="233bc-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="233bc-126">Request headers</span></span>

| <span data-ttu-id="233bc-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="233bc-127">Header</span></span>       | <span data-ttu-id="233bc-128">Значение</span><span class="sxs-lookup"><span data-stu-id="233bc-128">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="233bc-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="233bc-129">Authorization</span></span>  | <span data-ttu-id="233bc-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="233bc-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="233bc-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="233bc-132">Content-Type</span></span>  | <span data-ttu-id="233bc-133">application/json</span><span class="sxs-lookup"><span data-stu-id="233bc-133">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="233bc-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="233bc-134">Request body</span></span>

<span data-ttu-id="233bc-p106">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="233bc-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="233bc-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="233bc-138">Property</span></span>     | <span data-ttu-id="233bc-139">Тип</span><span class="sxs-lookup"><span data-stu-id="233bc-139">Type</span></span>   |<span data-ttu-id="233bc-140">Описание</span><span class="sxs-lookup"><span data-stu-id="233bc-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="233bc-141">contributionToContentDiscoveryDisabled</span><span class="sxs-lookup"><span data-stu-id="233bc-141">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="233bc-142">Логический</span><span class="sxs-lookup"><span data-stu-id="233bc-142">Boolean</span></span>|<span data-ttu-id="233bc-143">Настройка true для отключения доступа к документам в Office Delve для пользователя.</span><span class="sxs-lookup"><span data-stu-id="233bc-143">Set to true to disable access to documents in Office Delve for the user.</span></span> <span data-ttu-id="233bc-144">Этот параметр отражает состояние управления в [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span><span class="sxs-lookup"><span data-stu-id="233bc-144">This setting reflects the control state in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span>|

## <a name="example"></a><span data-ttu-id="233bc-145">Пример</span><span class="sxs-lookup"><span data-stu-id="233bc-145">Example</span></span> 

##### <a name="request"></a><span data-ttu-id="233bc-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="233bc-146">Request</span></span>

<span data-ttu-id="233bc-147">Вот пример запроса о том, как отключать пользователя от Delve и отключить его вклад в содержимого для всей организации.</span><span class="sxs-lookup"><span data-stu-id="233bc-147">Here is an example request on how to opt-out a user from Delve and disable his contribution on content relevancy for the whole organization.</span></span>

```http
PATCH https://graph.microsoft.com/beta/me/settings
Content-type: application/json
Content-length: 37

{
  "contributionToContentDiscoveryDisabled": true
}
```

##### <a name="response"></a><span data-ttu-id="233bc-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="233bc-148">Response</span></span>

<span data-ttu-id="233bc-p108">Ниже представлен пример отклика. Примечание: показанный здесь объект отклика может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="233bc-p108">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": true
}
```



