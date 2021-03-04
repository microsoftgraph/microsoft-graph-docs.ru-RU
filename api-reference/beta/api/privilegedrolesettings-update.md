---
title: Обновление privilegedRoleSettings
description: Обновление параметров ролей для данного параметра ролей. Объект privilegedRoleSettings будет возвращен.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 80797ba6965cade1625f6cc46abaf3f9fcbfadd2
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441104"
---
# <a name="update-privilegedrolesettings"></a><span data-ttu-id="52104-104">Обновление privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="52104-104">Update privilegedRoleSettings</span></span>

<span data-ttu-id="52104-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52104-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52104-106">Обновление параметров ролей для данного параметра ролей.</span><span class="sxs-lookup"><span data-stu-id="52104-106">Update the role settings for the given role setting.</span></span> <span data-ttu-id="52104-107">Объект [privilegedRoleSettings](../resources/privilegedrolesettings.md) будет возвращен.</span><span class="sxs-lookup"><span data-stu-id="52104-107">A [privilegedRoleSettings](../resources/privilegedrolesettings.md) object will be returned.</span></span>
## <a name="permissions"></a><span data-ttu-id="52104-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="52104-108">Permissions</span></span>

<span data-ttu-id="52104-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52104-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="52104-111">**Примечание:** Запрашиватель должен иметь роль администратора привилегированных ролей для обновления параметров ролей.</span><span class="sxs-lookup"><span data-stu-id="52104-111">**Note:** The requester must have the Privileged Role Administrator role to update role settings.</span></span> 

|<span data-ttu-id="52104-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="52104-112">Permission type</span></span>      | <span data-ttu-id="52104-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="52104-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="52104-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="52104-114">Delegated (work or school account)</span></span> | <span data-ttu-id="52104-115">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="52104-115">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="52104-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="52104-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52104-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52104-117">Not supported.</span></span>    |
|<span data-ttu-id="52104-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="52104-118">Application</span></span> | <span data-ttu-id="52104-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52104-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="52104-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="52104-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /privilegedRoles/{id}/settings
```

## <a name="request-headers"></a><span data-ttu-id="52104-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="52104-121">Request headers</span></span>
| <span data-ttu-id="52104-122">Имя</span><span class="sxs-lookup"><span data-stu-id="52104-122">Name</span></span>      |<span data-ttu-id="52104-123">Описание</span><span class="sxs-lookup"><span data-stu-id="52104-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="52104-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="52104-124">Authorization</span></span>  | <span data-ttu-id="52104-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="52104-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="52104-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="52104-127">Request body</span></span>
<span data-ttu-id="52104-128">В теле запроса поставляем представление JSON объекта [privilegedRoleSettings.](../resources/privilegedrolesettings.md)</span><span class="sxs-lookup"><span data-stu-id="52104-128">In the request body, supply a JSON representation of a [privilegedRoleSettings](../resources/privilegedrolesettings.md) object.</span></span>

<span data-ttu-id="52104-129">В следующей таблице перечислены свойства, которые можно предоставить при обновлении параметра роли.</span><span class="sxs-lookup"><span data-stu-id="52104-129">The following table lists the properties that you can supply when you update a role setting.</span></span>

|<span data-ttu-id="52104-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="52104-130">Property</span></span>|<span data-ttu-id="52104-131">Тип</span><span class="sxs-lookup"><span data-stu-id="52104-131">Type</span></span>|<span data-ttu-id="52104-132">Описание</span><span class="sxs-lookup"><span data-stu-id="52104-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="52104-133">elevationDuration</span><span class="sxs-lookup"><span data-stu-id="52104-133">elevationDuration</span></span>|<span data-ttu-id="52104-134">duration</span><span class="sxs-lookup"><span data-stu-id="52104-134">duration</span></span>|<span data-ttu-id="52104-135">Продолжительность активации роли.</span><span class="sxs-lookup"><span data-stu-id="52104-135">The duration when the role is activated.</span></span> <span data-ttu-id="52104-136">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="52104-136">Required.</span></span>|
|<span data-ttu-id="52104-137">id</span><span class="sxs-lookup"><span data-stu-id="52104-137">id</span></span>|<span data-ttu-id="52104-138">string</span><span class="sxs-lookup"><span data-stu-id="52104-138">string</span></span>|<span data-ttu-id="52104-139">Уникальный идентификатор параметров ролей.</span><span class="sxs-lookup"><span data-stu-id="52104-139">The unique identifier for the role settings.</span></span> <span data-ttu-id="52104-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="52104-140">Read-only.</span></span> <span data-ttu-id="52104-141">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="52104-141">Required.</span></span>|
|<span data-ttu-id="52104-142">isMfaOnElevationConfigurable</span><span class="sxs-lookup"><span data-stu-id="52104-142">isMfaOnElevationConfigurable</span></span>|<span data-ttu-id="52104-143">boolean</span><span class="sxs-lookup"><span data-stu-id="52104-143">boolean</span></span>|<span data-ttu-id="52104-144">**верно,** если mfaOnElevation настраивается.</span><span class="sxs-lookup"><span data-stu-id="52104-144">**true** if mfaOnElevation is configurable.</span></span> <span data-ttu-id="52104-145">**false,** если mfaOnElevation не настраивается.</span><span class="sxs-lookup"><span data-stu-id="52104-145">**false** if mfaOnElevation is not configurable.</span></span> <span data-ttu-id="52104-146">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="52104-146">Required.</span></span>|
|<span data-ttu-id="52104-147">lastGlobalAdmin</span><span class="sxs-lookup"><span data-stu-id="52104-147">lastGlobalAdmin</span></span>|<span data-ttu-id="52104-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="52104-148">Boolean</span></span>|<span data-ttu-id="52104-149">Только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="52104-149">For internal use only.</span></span>|
|<span data-ttu-id="52104-150">maxElavationDuration</span><span class="sxs-lookup"><span data-stu-id="52104-150">maxElavationDuration</span></span>|<span data-ttu-id="52104-151">duration</span><span class="sxs-lookup"><span data-stu-id="52104-151">duration</span></span>|<span data-ttu-id="52104-152">Максимальная продолжительность для активированной роли.</span><span class="sxs-lookup"><span data-stu-id="52104-152">Maximum duration for the activated role.</span></span> <span data-ttu-id="52104-153">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="52104-153">Required.</span></span>|
|<span data-ttu-id="52104-154">mfaOnElevation</span><span class="sxs-lookup"><span data-stu-id="52104-154">mfaOnElevation</span></span>|<span data-ttu-id="52104-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="52104-155">Boolean</span></span>|<span data-ttu-id="52104-156">**значение true,** если для активации роли требуется MFA.</span><span class="sxs-lookup"><span data-stu-id="52104-156">**true** if MFA is required to activate the role.</span></span> <span data-ttu-id="52104-157">**false,** если MFA не требуется для активации роли.</span><span class="sxs-lookup"><span data-stu-id="52104-157">**false** if MFA is not required to activate the role.</span></span> <span data-ttu-id="52104-158">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="52104-158">Required.</span></span>|
|<span data-ttu-id="52104-159">minElevationDuration</span><span class="sxs-lookup"><span data-stu-id="52104-159">minElevationDuration</span></span>|<span data-ttu-id="52104-160">duration</span><span class="sxs-lookup"><span data-stu-id="52104-160">duration</span></span>|<span data-ttu-id="52104-161">Минимальная продолжительность для активированной роли.</span><span class="sxs-lookup"><span data-stu-id="52104-161">Minimum duration for the activated role.</span></span> <span data-ttu-id="52104-162">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="52104-162">Required.</span></span>|
|<span data-ttu-id="52104-163">notificationToUserOnElevation</span><span class="sxs-lookup"><span data-stu-id="52104-163">notificationToUserOnElevation</span></span>|<span data-ttu-id="52104-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="52104-164">Boolean</span></span>|<span data-ttu-id="52104-165">**значение true,** если отправить уведомление конечному пользователю при активации роли.</span><span class="sxs-lookup"><span data-stu-id="52104-165">**true** if send notification to the end user when the role is activated.</span></span> <span data-ttu-id="52104-166">**false,** если не отправлять уведомления при активации роли.</span><span class="sxs-lookup"><span data-stu-id="52104-166">**false** if do not send notification when the role is activated.</span></span> <span data-ttu-id="52104-167">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="52104-167">Required.</span></span>|
|<span data-ttu-id="52104-168">ticketingInfoOnElevation</span><span class="sxs-lookup"><span data-stu-id="52104-168">ticketingInfoOnElevation</span></span>|<span data-ttu-id="52104-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="52104-169">Boolean</span></span>|<span data-ttu-id="52104-170">**значение true,** если при активации роли требуется информация о билетах.</span><span class="sxs-lookup"><span data-stu-id="52104-170">**true** if the ticketing information is required when activate the role.</span></span> <span data-ttu-id="52104-171">**false,** если сведения о билетах не требуются при активации роли.</span><span class="sxs-lookup"><span data-stu-id="52104-171">**false** if the ticketing information is not required when activate the role.</span></span> <span data-ttu-id="52104-172">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="52104-172">Required.</span></span>|
|<span data-ttu-id="52104-173">approvalOnElevation</span><span class="sxs-lookup"><span data-stu-id="52104-173">approvalOnElevation</span></span>|<span data-ttu-id="52104-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="52104-174">Boolean</span></span>|<span data-ttu-id="52104-175">**значение true,** если требуется утверждение при активации роли.</span><span class="sxs-lookup"><span data-stu-id="52104-175">**true** if the approval is required when activate the role.</span></span> <span data-ttu-id="52104-176">**false,** если утверждение не требуется при активации роли.</span><span class="sxs-lookup"><span data-stu-id="52104-176">**false** if the approval is not required when activate the role.</span></span> <span data-ttu-id="52104-177">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="52104-177">Required.</span></span>|
|<span data-ttu-id="52104-178">approverIds</span><span class="sxs-lookup"><span data-stu-id="52104-178">approverIds</span></span>|<span data-ttu-id="52104-179">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="52104-179">string collection</span></span>|<span data-ttu-id="52104-180">Список ID утверждения, если требуется утверждение для активации.</span><span class="sxs-lookup"><span data-stu-id="52104-180">List of Approval IDs, if approval is required for activation.</span></span>|

## <a name="response"></a><span data-ttu-id="52104-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="52104-181">Response</span></span>

<span data-ttu-id="52104-182">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="52104-182">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="52104-183">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="52104-183">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="52104-184">В противном случае код запретного статуса HTTP 403 будет возвращен.</span><span class="sxs-lookup"><span data-stu-id="52104-184">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="52104-185">Пример</span><span class="sxs-lookup"><span data-stu-id="52104-185">Example</span></span>
##### <a name="request"></a><span data-ttu-id="52104-186">Запрос</span><span class="sxs-lookup"><span data-stu-id="52104-186">Request</span></span>
<span data-ttu-id="52104-187">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="52104-187">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="52104-188">HTTP</span><span class="sxs-lookup"><span data-stu-id="52104-188">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "put_privilegedrolesettings"
}-->
```http
PUT https://graph.microsoft.com/beta/privilegedRoles/{id}/settings
Content-type: application/json

{
    "id": "9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3",
    "elevationDuration": "PT8H",
    "notificationToUserOnElevation": false,
    "ticketingInfoOnElevation": true,
    "mfaOnElevation": false,
    "maxElavationDuration": "PT0S",
    "minElevationDuration": "PT0S",
    "lastGlobalAdmin": false,
    "isMfaOnElevationConfigurable": true,
    "approvalOnElevation": false,
    "approverIds": ["e2b2a2fb-13d7-495c-adc9-941fe966793f", "22770e3f-b9b4-418e-9dea-d0e3d2f275dd"]
}
```
# <a name="c"></a>[<span data-ttu-id="52104-189">C#</span><span class="sxs-lookup"><span data-stu-id="52104-189">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/put-privilegedrolesettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="52104-190">JavaScript</span><span class="sxs-lookup"><span data-stu-id="52104-190">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/put-privilegedrolesettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="52104-191">Objective-C</span><span class="sxs-lookup"><span data-stu-id="52104-191">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/put-privilegedrolesettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="52104-192">Java</span><span class="sxs-lookup"><span data-stu-id="52104-192">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/put-privilegedrolesettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="52104-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="52104-193">Response</span></span>
<span data-ttu-id="52104-194">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="52104-194">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}-->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update privilegedRoleSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


