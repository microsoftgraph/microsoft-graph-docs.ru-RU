---
title: Обновление Привилежедролесеттингс
description: Обновление параметров роли для данного параметра роли. Будет возвращен объект Привилежедролесеттингс.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: b097b0831ed33e826ae62a413a1b3d9f2227b45e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35978665"
---
# <a name="update-privilegedrolesettings"></a><span data-ttu-id="9be6d-104">Обновление Привилежедролесеттингс</span><span class="sxs-lookup"><span data-stu-id="9be6d-104">Update privilegedRoleSettings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9be6d-105">Обновление параметров роли для данного параметра роли.</span><span class="sxs-lookup"><span data-stu-id="9be6d-105">Update the role settings for the given role setting.</span></span> <span data-ttu-id="9be6d-106">Будет возвращен объект [привилежедролесеттингс](../resources/privilegedrolesettings.md) .</span><span class="sxs-lookup"><span data-stu-id="9be6d-106">A [privilegedRoleSettings](../resources/privilegedrolesettings.md) object will be returned.</span></span>
## <a name="permissions"></a><span data-ttu-id="9be6d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9be6d-107">Permissions</span></span>

<span data-ttu-id="9be6d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9be6d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="9be6d-110">**Примечание:** Запрашивающая сторона должна иметь одну из следующих ролей: привилегированный администратор ролей, глобальный администратор, администратор безопасности или средство чтения безопасности.</span><span class="sxs-lookup"><span data-stu-id="9be6d-110">**Note:** The requester must have one of the following roles: Privileged Role Administrator, Global Administrator, Security Administrator, or Security Reader.</span></span> 

|<span data-ttu-id="9be6d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9be6d-111">Permission type</span></span>      | <span data-ttu-id="9be6d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9be6d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9be6d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9be6d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="9be6d-114">Привилежедакцесс. ReadWrite. AzureAD, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="9be6d-114">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9be6d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9be6d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9be6d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9be6d-116">Not supported.</span></span>    |
|<span data-ttu-id="9be6d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9be6d-117">Application</span></span> | <span data-ttu-id="9be6d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9be6d-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9be6d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9be6d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /privilegedRoles/{id}/settings
```

## <a name="request-headers"></a><span data-ttu-id="9be6d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9be6d-120">Request headers</span></span>
| <span data-ttu-id="9be6d-121">Имя</span><span class="sxs-lookup"><span data-stu-id="9be6d-121">Name</span></span>      |<span data-ttu-id="9be6d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="9be6d-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9be6d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9be6d-123">Authorization</span></span>  | <span data-ttu-id="9be6d-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9be6d-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9be6d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9be6d-126">Request body</span></span>
<span data-ttu-id="9be6d-127">В тексте запроса добавьте представление объекта [привилежедролесеттингс](../resources/privilegedrolesettings.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9be6d-127">In the request body, supply a JSON representation of a [privilegedRoleSettings](../resources/privilegedrolesettings.md) object.</span></span>

<span data-ttu-id="9be6d-128">В следующей таблице перечислены свойства, которые можно предоставить при обновлении параметров роли.</span><span class="sxs-lookup"><span data-stu-id="9be6d-128">The following table lists the properties that you can supply when you update a role setting.</span></span>

|<span data-ttu-id="9be6d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="9be6d-129">Property</span></span>|<span data-ttu-id="9be6d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="9be6d-130">Type</span></span>|<span data-ttu-id="9be6d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="9be6d-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9be6d-132">Елеватиондуратион</span><span class="sxs-lookup"><span data-stu-id="9be6d-132">elevationDuration</span></span>|<span data-ttu-id="9be6d-133">duration</span><span class="sxs-lookup"><span data-stu-id="9be6d-133">duration</span></span>|<span data-ttu-id="9be6d-134">Продолжительность активации роли.</span><span class="sxs-lookup"><span data-stu-id="9be6d-134">The duration when the role is activated.</span></span> <span data-ttu-id="9be6d-135">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9be6d-135">Required.</span></span>|
|<span data-ttu-id="9be6d-136">id</span><span class="sxs-lookup"><span data-stu-id="9be6d-136">id</span></span>|<span data-ttu-id="9be6d-137">string</span><span class="sxs-lookup"><span data-stu-id="9be6d-137">string</span></span>|<span data-ttu-id="9be6d-138">Уникальный идентификатор для параметров роли.</span><span class="sxs-lookup"><span data-stu-id="9be6d-138">The unique identifier for the role settings.</span></span> <span data-ttu-id="9be6d-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9be6d-139">Read-only.</span></span> <span data-ttu-id="9be6d-140">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="9be6d-140">Required.</span></span>|
|<span data-ttu-id="9be6d-141">Исмфаонелеватионконфигурабле</span><span class="sxs-lookup"><span data-stu-id="9be6d-141">isMfaOnElevationConfigurable</span></span>|<span data-ttu-id="9be6d-142">boolean</span><span class="sxs-lookup"><span data-stu-id="9be6d-142">boolean</span></span>|<span data-ttu-id="9be6d-143">**значение true** , если мфаонелеватион является настраиваемым.</span><span class="sxs-lookup"><span data-stu-id="9be6d-143">**true** if mfaOnElevation is configurable.</span></span> <span data-ttu-id="9be6d-144">**false** , если мфаонелеватион не является настраиваемым.</span><span class="sxs-lookup"><span data-stu-id="9be6d-144">**false** if mfaOnElevation is not configurable.</span></span> <span data-ttu-id="9be6d-145">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="9be6d-145">Required.</span></span>|
|<span data-ttu-id="9be6d-146">Ластглобаладмин</span><span class="sxs-lookup"><span data-stu-id="9be6d-146">lastGlobalAdmin</span></span>|<span data-ttu-id="9be6d-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="9be6d-147">Boolean</span></span>|<span data-ttu-id="9be6d-148">Только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="9be6d-148">For internal use only.</span></span>|
|<span data-ttu-id="9be6d-149">Макселаватиондуратион</span><span class="sxs-lookup"><span data-stu-id="9be6d-149">maxElavationDuration</span></span>|<span data-ttu-id="9be6d-150">duration</span><span class="sxs-lookup"><span data-stu-id="9be6d-150">duration</span></span>|<span data-ttu-id="9be6d-151">Максимальная длительность активированной роли.</span><span class="sxs-lookup"><span data-stu-id="9be6d-151">Maximum duration for the activated role.</span></span> <span data-ttu-id="9be6d-152">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="9be6d-152">Required.</span></span>|
|<span data-ttu-id="9be6d-153">Мфаонелеватион</span><span class="sxs-lookup"><span data-stu-id="9be6d-153">mfaOnElevation</span></span>|<span data-ttu-id="9be6d-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="9be6d-154">Boolean</span></span>|<span data-ttu-id="9be6d-155">**значение true** , если для активации роли требуется mfa.</span><span class="sxs-lookup"><span data-stu-id="9be6d-155">**true** if MFA is required to activate the role.</span></span> <span data-ttu-id="9be6d-156">**false** , если MFA не требуется для активации роли.</span><span class="sxs-lookup"><span data-stu-id="9be6d-156">**false** if MFA is not required to activate the role.</span></span> <span data-ttu-id="9be6d-157">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="9be6d-157">Required.</span></span>|
|<span data-ttu-id="9be6d-158">Минелеватиондуратион</span><span class="sxs-lookup"><span data-stu-id="9be6d-158">minElevationDuration</span></span>|<span data-ttu-id="9be6d-159">duration</span><span class="sxs-lookup"><span data-stu-id="9be6d-159">duration</span></span>|<span data-ttu-id="9be6d-160">Минимальная длительность активированной роли.</span><span class="sxs-lookup"><span data-stu-id="9be6d-160">Minimum duration for the activated role.</span></span> <span data-ttu-id="9be6d-161">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="9be6d-161">Required.</span></span>|
|<span data-ttu-id="9be6d-162">Нотификатионтаусеронелеватион</span><span class="sxs-lookup"><span data-stu-id="9be6d-162">notificationToUserOnElevation</span></span>|<span data-ttu-id="9be6d-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="9be6d-163">Boolean</span></span>|<span data-ttu-id="9be6d-164">**имеет значение true** , если вы отправляете уведомление конечному пользователю при активации роли.</span><span class="sxs-lookup"><span data-stu-id="9be6d-164">**true** if send notification to the end user when the role is activated.</span></span> <span data-ttu-id="9be6d-165">**значение false** , если уведомление не отправляется при активации роли.</span><span class="sxs-lookup"><span data-stu-id="9be6d-165">**false** if do not send notification when the role is activated.</span></span> <span data-ttu-id="9be6d-166">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="9be6d-166">Required.</span></span>|
|<span data-ttu-id="9be6d-167">Тиккетингинфунелеватион</span><span class="sxs-lookup"><span data-stu-id="9be6d-167">ticketingInfoOnElevation</span></span>|<span data-ttu-id="9be6d-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="9be6d-168">Boolean</span></span>|<span data-ttu-id="9be6d-169">**имеет значение true** , если при активации роли требуются сведения о билетах.</span><span class="sxs-lookup"><span data-stu-id="9be6d-169">**true** if the ticketing information is required when activate the role.</span></span> <span data-ttu-id="9be6d-170">**false** , если при активации роли не требуются сведения о билетах.</span><span class="sxs-lookup"><span data-stu-id="9be6d-170">**false** if the ticketing information is not required when activate the role.</span></span> <span data-ttu-id="9be6d-171">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="9be6d-171">Required.</span></span>|
|<span data-ttu-id="9be6d-172">Аппровалонелеватион</span><span class="sxs-lookup"><span data-stu-id="9be6d-172">approvalOnElevation</span></span>|<span data-ttu-id="9be6d-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="9be6d-173">Boolean</span></span>|<span data-ttu-id="9be6d-174">**имеет значение true** , если при активации роли необходимо выполнить утверждение.</span><span class="sxs-lookup"><span data-stu-id="9be6d-174">**true** if the approval is required when activate the role.</span></span> <span data-ttu-id="9be6d-175">**false** , если при активации роли не нужно утверждать.</span><span class="sxs-lookup"><span data-stu-id="9be6d-175">**false** if the approval is not required when activate the role.</span></span> <span data-ttu-id="9be6d-176">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="9be6d-176">Required.</span></span>|
|<span data-ttu-id="9be6d-177">Аппроверидс</span><span class="sxs-lookup"><span data-stu-id="9be6d-177">approverIds</span></span>|<span data-ttu-id="9be6d-178">string collection</span><span class="sxs-lookup"><span data-stu-id="9be6d-178">string collection</span></span>|<span data-ttu-id="9be6d-179">Список идентификаторов утверждения, если для активации необходимо утверждение.</span><span class="sxs-lookup"><span data-stu-id="9be6d-179">List of Approval IDs, if approval is required for activation.</span></span>|

## <a name="response"></a><span data-ttu-id="9be6d-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="9be6d-180">Response</span></span>

<span data-ttu-id="9be6d-181">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9be6d-181">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="9be6d-182">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="9be6d-182">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="9be6d-183">В противном случае будет возвращен код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="9be6d-183">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="9be6d-184">Пример</span><span class="sxs-lookup"><span data-stu-id="9be6d-184">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9be6d-185">Запрос</span><span class="sxs-lookup"><span data-stu-id="9be6d-185">Request</span></span>
<span data-ttu-id="9be6d-186">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9be6d-186">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9be6d-187">HTTP</span><span class="sxs-lookup"><span data-stu-id="9be6d-187">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="9be6d-188">C#</span><span class="sxs-lookup"><span data-stu-id="9be6d-188">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/put-privilegedrolesettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9be6d-189">Javascript</span><span class="sxs-lookup"><span data-stu-id="9be6d-189">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/put-privilegedrolesettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9be6d-190">Цель — C</span><span class="sxs-lookup"><span data-stu-id="9be6d-190">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/put-privilegedrolesettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9be6d-191">Java</span><span class="sxs-lookup"><span data-stu-id="9be6d-191">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/put-privilegedrolesettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9be6d-192">Ответ</span><span class="sxs-lookup"><span data-stu-id="9be6d-192">Response</span></span>
<span data-ttu-id="9be6d-193">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9be6d-193">Here is an example of the response.</span></span>
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
