---
title: Обновление Привилежедролесеттингс
description: Обновление параметров роли для данного параметра роли. Будет возвращен объект Привилежедролесеттингс.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: c7457fe35aef8f58d615678f0cbe1a8f77fda766
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48976156"
---
# <a name="update-privilegedrolesettings"></a><span data-ttu-id="43250-104">Обновление Привилежедролесеттингс</span><span class="sxs-lookup"><span data-stu-id="43250-104">Update privilegedRoleSettings</span></span>

<span data-ttu-id="43250-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43250-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="43250-106">Обновление параметров роли для данного параметра роли.</span><span class="sxs-lookup"><span data-stu-id="43250-106">Update the role settings for the given role setting.</span></span> <span data-ttu-id="43250-107">Будет возвращен объект [привилежедролесеттингс](../resources/privilegedrolesettings.md) .</span><span class="sxs-lookup"><span data-stu-id="43250-107">A [privilegedRoleSettings](../resources/privilegedrolesettings.md) object will be returned.</span></span>
## <a name="permissions"></a><span data-ttu-id="43250-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="43250-108">Permissions</span></span>

<span data-ttu-id="43250-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43250-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="43250-111">**Примечание:** Для обновления параметров роли запрашивающая сторона должна иметь роль администратора привилегированной роли.</span><span class="sxs-lookup"><span data-stu-id="43250-111">**Note:** The requester must have the Privileged Role Administrator role to update role settings.</span></span> 

|<span data-ttu-id="43250-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="43250-112">Permission type</span></span>      | <span data-ttu-id="43250-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="43250-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="43250-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="43250-114">Delegated (work or school account)</span></span> | <span data-ttu-id="43250-115">Привилежедакцесс. ReadWrite. AzureAD, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="43250-115">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="43250-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="43250-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="43250-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43250-117">Not supported.</span></span>    |
|<span data-ttu-id="43250-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="43250-118">Application</span></span> | <span data-ttu-id="43250-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43250-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="43250-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="43250-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /privilegedRoles/{id}/settings
```

## <a name="request-headers"></a><span data-ttu-id="43250-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="43250-121">Request headers</span></span>
| <span data-ttu-id="43250-122">Имя</span><span class="sxs-lookup"><span data-stu-id="43250-122">Name</span></span>      |<span data-ttu-id="43250-123">Описание</span><span class="sxs-lookup"><span data-stu-id="43250-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="43250-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="43250-124">Authorization</span></span>  | <span data-ttu-id="43250-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="43250-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="43250-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="43250-127">Request body</span></span>
<span data-ttu-id="43250-128">В тексте запроса добавьте представление объекта [привилежедролесеттингс](../resources/privilegedrolesettings.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="43250-128">In the request body, supply a JSON representation of a [privilegedRoleSettings](../resources/privilegedrolesettings.md) object.</span></span>

<span data-ttu-id="43250-129">В следующей таблице перечислены свойства, которые можно предоставить при обновлении параметров роли.</span><span class="sxs-lookup"><span data-stu-id="43250-129">The following table lists the properties that you can supply when you update a role setting.</span></span>

|<span data-ttu-id="43250-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="43250-130">Property</span></span>|<span data-ttu-id="43250-131">Тип</span><span class="sxs-lookup"><span data-stu-id="43250-131">Type</span></span>|<span data-ttu-id="43250-132">Описание</span><span class="sxs-lookup"><span data-stu-id="43250-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="43250-133">елеватиондуратион</span><span class="sxs-lookup"><span data-stu-id="43250-133">elevationDuration</span></span>|<span data-ttu-id="43250-134">duration</span><span class="sxs-lookup"><span data-stu-id="43250-134">duration</span></span>|<span data-ttu-id="43250-135">Продолжительность активации роли.</span><span class="sxs-lookup"><span data-stu-id="43250-135">The duration when the role is activated.</span></span> <span data-ttu-id="43250-136">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="43250-136">Required.</span></span>|
|<span data-ttu-id="43250-137">id</span><span class="sxs-lookup"><span data-stu-id="43250-137">id</span></span>|<span data-ttu-id="43250-138">string</span><span class="sxs-lookup"><span data-stu-id="43250-138">string</span></span>|<span data-ttu-id="43250-139">Уникальный идентификатор для параметров роли.</span><span class="sxs-lookup"><span data-stu-id="43250-139">The unique identifier for the role settings.</span></span> <span data-ttu-id="43250-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="43250-140">Read-only.</span></span> <span data-ttu-id="43250-141">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="43250-141">Required.</span></span>|
|<span data-ttu-id="43250-142">исмфаонелеватионконфигурабле</span><span class="sxs-lookup"><span data-stu-id="43250-142">isMfaOnElevationConfigurable</span></span>|<span data-ttu-id="43250-143">boolean</span><span class="sxs-lookup"><span data-stu-id="43250-143">boolean</span></span>|<span data-ttu-id="43250-144">**значение true** , если мфаонелеватион является настраиваемым.</span><span class="sxs-lookup"><span data-stu-id="43250-144">**true** if mfaOnElevation is configurable.</span></span> <span data-ttu-id="43250-145">**false** , если мфаонелеватион не является настраиваемым.</span><span class="sxs-lookup"><span data-stu-id="43250-145">**false** if mfaOnElevation is not configurable.</span></span> <span data-ttu-id="43250-146">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="43250-146">Required.</span></span>|
|<span data-ttu-id="43250-147">ластглобаладмин</span><span class="sxs-lookup"><span data-stu-id="43250-147">lastGlobalAdmin</span></span>|<span data-ttu-id="43250-148">Логический</span><span class="sxs-lookup"><span data-stu-id="43250-148">Boolean</span></span>|<span data-ttu-id="43250-149">Только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="43250-149">For internal use only.</span></span>|
|<span data-ttu-id="43250-150">макселаватиондуратион</span><span class="sxs-lookup"><span data-stu-id="43250-150">maxElavationDuration</span></span>|<span data-ttu-id="43250-151">duration</span><span class="sxs-lookup"><span data-stu-id="43250-151">duration</span></span>|<span data-ttu-id="43250-152">Максимальная длительность активированной роли.</span><span class="sxs-lookup"><span data-stu-id="43250-152">Maximum duration for the activated role.</span></span> <span data-ttu-id="43250-153">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="43250-153">Required.</span></span>|
|<span data-ttu-id="43250-154">мфаонелеватион</span><span class="sxs-lookup"><span data-stu-id="43250-154">mfaOnElevation</span></span>|<span data-ttu-id="43250-155">Логический</span><span class="sxs-lookup"><span data-stu-id="43250-155">Boolean</span></span>|<span data-ttu-id="43250-156">**значение true** , если для активации роли требуется mfa.</span><span class="sxs-lookup"><span data-stu-id="43250-156">**true** if MFA is required to activate the role.</span></span> <span data-ttu-id="43250-157">**false** , если MFA не требуется для активации роли.</span><span class="sxs-lookup"><span data-stu-id="43250-157">**false** if MFA is not required to activate the role.</span></span> <span data-ttu-id="43250-158">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="43250-158">Required.</span></span>|
|<span data-ttu-id="43250-159">минелеватиондуратион</span><span class="sxs-lookup"><span data-stu-id="43250-159">minElevationDuration</span></span>|<span data-ttu-id="43250-160">duration</span><span class="sxs-lookup"><span data-stu-id="43250-160">duration</span></span>|<span data-ttu-id="43250-161">Минимальная длительность активированной роли.</span><span class="sxs-lookup"><span data-stu-id="43250-161">Minimum duration for the activated role.</span></span> <span data-ttu-id="43250-162">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="43250-162">Required.</span></span>|
|<span data-ttu-id="43250-163">нотификатионтаусеронелеватион</span><span class="sxs-lookup"><span data-stu-id="43250-163">notificationToUserOnElevation</span></span>|<span data-ttu-id="43250-164">Логический</span><span class="sxs-lookup"><span data-stu-id="43250-164">Boolean</span></span>|<span data-ttu-id="43250-165">**имеет значение true** , если вы отправляете уведомление конечному пользователю при активации роли.</span><span class="sxs-lookup"><span data-stu-id="43250-165">**true** if send notification to the end user when the role is activated.</span></span> <span data-ttu-id="43250-166">**значение false** , если уведомление не отправляется при активации роли.</span><span class="sxs-lookup"><span data-stu-id="43250-166">**false** if do not send notification when the role is activated.</span></span> <span data-ttu-id="43250-167">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="43250-167">Required.</span></span>|
|<span data-ttu-id="43250-168">тиккетингинфунелеватион</span><span class="sxs-lookup"><span data-stu-id="43250-168">ticketingInfoOnElevation</span></span>|<span data-ttu-id="43250-169">Логический</span><span class="sxs-lookup"><span data-stu-id="43250-169">Boolean</span></span>|<span data-ttu-id="43250-170">**имеет значение true** , если при активации роли требуются сведения о билетах.</span><span class="sxs-lookup"><span data-stu-id="43250-170">**true** if the ticketing information is required when activate the role.</span></span> <span data-ttu-id="43250-171">**false** , если при активации роли не требуются сведения о билетах.</span><span class="sxs-lookup"><span data-stu-id="43250-171">**false** if the ticketing information is not required when activate the role.</span></span> <span data-ttu-id="43250-172">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="43250-172">Required.</span></span>|
|<span data-ttu-id="43250-173">аппровалонелеватион</span><span class="sxs-lookup"><span data-stu-id="43250-173">approvalOnElevation</span></span>|<span data-ttu-id="43250-174">Логический</span><span class="sxs-lookup"><span data-stu-id="43250-174">Boolean</span></span>|<span data-ttu-id="43250-175">**имеет значение true** , если при активации роли необходимо выполнить утверждение.</span><span class="sxs-lookup"><span data-stu-id="43250-175">**true** if the approval is required when activate the role.</span></span> <span data-ttu-id="43250-176">**false** , если при активации роли не нужно утверждать.</span><span class="sxs-lookup"><span data-stu-id="43250-176">**false** if the approval is not required when activate the role.</span></span> <span data-ttu-id="43250-177">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="43250-177">Required.</span></span>|
|<span data-ttu-id="43250-178">аппроверидс</span><span class="sxs-lookup"><span data-stu-id="43250-178">approverIds</span></span>|<span data-ttu-id="43250-179">string collection</span><span class="sxs-lookup"><span data-stu-id="43250-179">string collection</span></span>|<span data-ttu-id="43250-180">Список идентификаторов утверждения, если для активации необходимо утверждение.</span><span class="sxs-lookup"><span data-stu-id="43250-180">List of Approval IDs, if approval is required for activation.</span></span>|

## <a name="response"></a><span data-ttu-id="43250-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="43250-181">Response</span></span>

<span data-ttu-id="43250-182">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="43250-182">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="43250-183">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="43250-183">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="43250-184">В противном случае будет возвращен код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="43250-184">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="43250-185">Пример</span><span class="sxs-lookup"><span data-stu-id="43250-185">Example</span></span>
##### <a name="request"></a><span data-ttu-id="43250-186">Запрос</span><span class="sxs-lookup"><span data-stu-id="43250-186">Request</span></span>
<span data-ttu-id="43250-187">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="43250-187">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="43250-188">HTTP</span><span class="sxs-lookup"><span data-stu-id="43250-188">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="43250-189">C#</span><span class="sxs-lookup"><span data-stu-id="43250-189">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/put-privilegedrolesettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="43250-190">JavaScript</span><span class="sxs-lookup"><span data-stu-id="43250-190">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/put-privilegedrolesettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="43250-191">Objective-C</span><span class="sxs-lookup"><span data-stu-id="43250-191">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/put-privilegedrolesettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="43250-192">Java</span><span class="sxs-lookup"><span data-stu-id="43250-192">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/put-privilegedrolesettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="43250-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="43250-193">Response</span></span>
<span data-ttu-id="43250-194">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="43250-194">Here is an example of the response.</span></span>
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


