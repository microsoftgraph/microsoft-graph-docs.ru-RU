---
title: Обновление privilegedRoleSettings
description: Обновление параметров ролей для параметров указанного ролей. Объект privilegedRoleSettings будут возвращены.
ms.openlocfilehash: 0e0f6b7253a1c1d8570c0b91fac4b08bbd39dfff
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082044"
---
# <a name="update-privilegedrolesettings"></a><span data-ttu-id="033c6-104">Обновление privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="033c6-104">Update privilegedRoleSettings</span></span>

> <span data-ttu-id="033c6-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="033c6-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="033c6-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="033c6-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="033c6-107">Обновление параметров ролей для параметров указанного ролей.</span><span class="sxs-lookup"><span data-stu-id="033c6-107">Update the role settings for the given role setting.</span></span> <span data-ttu-id="033c6-108">Объект [privilegedRoleSettings](../resources/privilegedrolesettings.md) будут возвращены.</span><span class="sxs-lookup"><span data-stu-id="033c6-108">A [privilegedRoleSettings](../resources/privilegedrolesettings.md) object will be returned.</span></span>
## <a name="permissions"></a><span data-ttu-id="033c6-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="033c6-109">Permissions</span></span>

<span data-ttu-id="033c6-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="033c6-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="033c6-112">**Примечание:** Источник запроса, должны использовать одну из следующих ролей: привилегированной роль администратора, глобального администратора, администратора безопасности или безопасности чтения.</span><span class="sxs-lookup"><span data-stu-id="033c6-112">**Note:** The requester must have one of the following roles: Privileged Role Administrator, Global Administrator, Security Administrator, or Security Reader.</span></span> 

|<span data-ttu-id="033c6-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="033c6-113">Permission type</span></span>      | <span data-ttu-id="033c6-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="033c6-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="033c6-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="033c6-115">Delegated (work or school account)</span></span> | <span data-ttu-id="033c6-116">PrivilegedAccess.ReadWrite.AzureAD Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="033c6-116">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="033c6-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="033c6-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="033c6-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="033c6-118">Not supported.</span></span>    |
|<span data-ttu-id="033c6-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="033c6-119">Application</span></span> | <span data-ttu-id="033c6-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="033c6-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="033c6-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="033c6-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /privilegedRoles/{id}/settings
```

## <a name="request-headers"></a><span data-ttu-id="033c6-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="033c6-122">Request headers</span></span>
| <span data-ttu-id="033c6-123">Имя</span><span class="sxs-lookup"><span data-stu-id="033c6-123">Name</span></span>      |<span data-ttu-id="033c6-124">Описание</span><span class="sxs-lookup"><span data-stu-id="033c6-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="033c6-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="033c6-125">Authorization</span></span>  | <span data-ttu-id="033c6-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="033c6-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="033c6-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="033c6-128">Request body</span></span>
<span data-ttu-id="033c6-129">В тексте запроса укажите представление JSON объекта [privilegedRoleSettings](../resources/privilegedrolesettings.md) .</span><span class="sxs-lookup"><span data-stu-id="033c6-129">In the request body, supply a JSON representation of a [privilegedRoleSettings](../resources/privilegedrolesettings.md) object.</span></span>

<span data-ttu-id="033c6-130">В следующей таблице приведены свойства, которые можно указать при обновлении параметров ролей.</span><span class="sxs-lookup"><span data-stu-id="033c6-130">The following table lists the properties that you can supply when you update a role setting.</span></span>

|<span data-ttu-id="033c6-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="033c6-131">Property</span></span>|<span data-ttu-id="033c6-132">Тип</span><span class="sxs-lookup"><span data-stu-id="033c6-132">Type</span></span>|<span data-ttu-id="033c6-133">Description</span><span class="sxs-lookup"><span data-stu-id="033c6-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="033c6-134">elevationDuration</span><span class="sxs-lookup"><span data-stu-id="033c6-134">elevationDuration</span></span>|<span data-ttu-id="033c6-135">duration</span><span class="sxs-lookup"><span data-stu-id="033c6-135">duration</span></span>|<span data-ttu-id="033c6-136">Длительность, при активации роли.</span><span class="sxs-lookup"><span data-stu-id="033c6-136">The duration when the role is activated.</span></span> <span data-ttu-id="033c6-137">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="033c6-137">Required.</span></span>|
|<span data-ttu-id="033c6-138">id</span><span class="sxs-lookup"><span data-stu-id="033c6-138">id</span></span>|<span data-ttu-id="033c6-139">строка</span><span class="sxs-lookup"><span data-stu-id="033c6-139">string</span></span>|<span data-ttu-id="033c6-140">Уникальный идентификатор для параметров роли.</span><span class="sxs-lookup"><span data-stu-id="033c6-140">The unique identifier for the role settings.</span></span> <span data-ttu-id="033c6-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="033c6-141">Read-only.</span></span> <span data-ttu-id="033c6-142">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="033c6-142">Required.</span></span>|
|<span data-ttu-id="033c6-143">isMfaOnElevationConfigurable</span><span class="sxs-lookup"><span data-stu-id="033c6-143">isMfaOnElevationConfigurable</span></span>|<span data-ttu-id="033c6-144">boolean</span><span class="sxs-lookup"><span data-stu-id="033c6-144">boolean</span></span>|<span data-ttu-id="033c6-145">**значение true,** Если mfaOnElevation может быть настроен.</span><span class="sxs-lookup"><span data-stu-id="033c6-145">**true** if mfaOnElevation is configurable.</span></span> <span data-ttu-id="033c6-146">**значение false,** Если mfaOnElevation не настраивается.</span><span class="sxs-lookup"><span data-stu-id="033c6-146">**false** if mfaOnElevation is not configurable.</span></span> <span data-ttu-id="033c6-147">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="033c6-147">Required.</span></span>|
|<span data-ttu-id="033c6-148">lastGlobalAdmin</span><span class="sxs-lookup"><span data-stu-id="033c6-148">lastGlobalAdmin</span></span>|<span data-ttu-id="033c6-149">Логический</span><span class="sxs-lookup"><span data-stu-id="033c6-149">Boolean</span></span>|<span data-ttu-id="033c6-150">Только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="033c6-150">For internal use only.</span></span>|
|<span data-ttu-id="033c6-151">maxElavationDuration</span><span class="sxs-lookup"><span data-stu-id="033c6-151">maxElavationDuration</span></span>|<span data-ttu-id="033c6-152">duration</span><span class="sxs-lookup"><span data-stu-id="033c6-152">duration</span></span>|<span data-ttu-id="033c6-153">Максимальная длительность для активации роли.</span><span class="sxs-lookup"><span data-stu-id="033c6-153">Maximum duration for the activated role.</span></span> <span data-ttu-id="033c6-154">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="033c6-154">Required.</span></span>|
|<span data-ttu-id="033c6-155">mfaOnElevation</span><span class="sxs-lookup"><span data-stu-id="033c6-155">mfaOnElevation</span></span>|<span data-ttu-id="033c6-156">Логический</span><span class="sxs-lookup"><span data-stu-id="033c6-156">Boolean</span></span>|<span data-ttu-id="033c6-157">**значение true,** Если необходимо активировать роль многофакторной проверкой Подлинности.</span><span class="sxs-lookup"><span data-stu-id="033c6-157">**true** if MFA is required to activate the role.</span></span> <span data-ttu-id="033c6-158">**значение false,** Если многофакторной проверкой Подлинности не требуется для включения роли.</span><span class="sxs-lookup"><span data-stu-id="033c6-158">**false** if MFA is not required to activate the role.</span></span> <span data-ttu-id="033c6-159">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="033c6-159">Required.</span></span>|
|<span data-ttu-id="033c6-160">minElevationDuration</span><span class="sxs-lookup"><span data-stu-id="033c6-160">minElevationDuration</span></span>|<span data-ttu-id="033c6-161">duration</span><span class="sxs-lookup"><span data-stu-id="033c6-161">duration</span></span>|<span data-ttu-id="033c6-162">Минимальная продолжительность активированные роли.</span><span class="sxs-lookup"><span data-stu-id="033c6-162">Minimum duration for the activated role.</span></span> <span data-ttu-id="033c6-163">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="033c6-163">Required.</span></span>|
|<span data-ttu-id="033c6-164">notificationToUserOnElevation</span><span class="sxs-lookup"><span data-stu-id="033c6-164">notificationToUserOnElevation</span></span>|<span data-ttu-id="033c6-165">Логический</span><span class="sxs-lookup"><span data-stu-id="033c6-165">Boolean</span></span>|<span data-ttu-id="033c6-166">**значение true,** Если отправить уведомление конечному пользователю при активации роли.</span><span class="sxs-lookup"><span data-stu-id="033c6-166">**true** if send notification to the end user when the role is activated.</span></span> <span data-ttu-id="033c6-167">**значение false,** Если не отправлять уведомления при активации роли.</span><span class="sxs-lookup"><span data-stu-id="033c6-167">**false** if do not send notification when the role is activated.</span></span> <span data-ttu-id="033c6-168">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="033c6-168">Required.</span></span>|
|<span data-ttu-id="033c6-169">ticketingInfoOnElevation</span><span class="sxs-lookup"><span data-stu-id="033c6-169">ticketingInfoOnElevation</span></span>|<span data-ttu-id="033c6-170">Логический</span><span class="sxs-lookup"><span data-stu-id="033c6-170">Boolean</span></span>|<span data-ttu-id="033c6-171">**значение true,** Если отдела сведения требуется при активации роли.</span><span class="sxs-lookup"><span data-stu-id="033c6-171">**true** if the ticketing information is required when activate the role.</span></span> <span data-ttu-id="033c6-172">**значение false,** Если отдела сведения не является обязательным, когда активировать роль.</span><span class="sxs-lookup"><span data-stu-id="033c6-172">**false** if the ticketing information is not required when activate the role.</span></span> <span data-ttu-id="033c6-173">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="033c6-173">Required.</span></span>|
|<span data-ttu-id="033c6-174">approvalOnElevation</span><span class="sxs-lookup"><span data-stu-id="033c6-174">approvalOnElevation</span></span>|<span data-ttu-id="033c6-175">Логический</span><span class="sxs-lookup"><span data-stu-id="033c6-175">Boolean</span></span>|<span data-ttu-id="033c6-176">**значение true,** Если требуется утверждение при активации роли.</span><span class="sxs-lookup"><span data-stu-id="033c6-176">**true** if the approval is required when activate the role.</span></span> <span data-ttu-id="033c6-177">**значение false,** Если утверждение не является обязательным, когда активировать роль.</span><span class="sxs-lookup"><span data-stu-id="033c6-177">**false** if the approval is not required when activate the role.</span></span> <span data-ttu-id="033c6-178">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="033c6-178">Required.</span></span>|
|<span data-ttu-id="033c6-179">approverIds</span><span class="sxs-lookup"><span data-stu-id="033c6-179">approverIds</span></span>|<span data-ttu-id="033c6-180">array</span><span class="sxs-lookup"><span data-stu-id="033c6-180">array</span></span>|<span data-ttu-id="033c6-181">Список идентификаторов утверждения, если требуется для активации утверждение.</span><span class="sxs-lookup"><span data-stu-id="033c6-181">List of Approval IDs, if approval is required for activation.</span></span>|

## <a name="response"></a><span data-ttu-id="033c6-182">Ответ</span><span class="sxs-lookup"><span data-stu-id="033c6-182">Response</span></span>

<span data-ttu-id="033c6-183">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="033c6-183">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="033c6-184">Обратите внимание, что необходимо зарегистрировать для PIM клиента.</span><span class="sxs-lookup"><span data-stu-id="033c6-184">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="033c6-185">В противном случае будут возвращены код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="033c6-185">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="033c6-186">Пример</span><span class="sxs-lookup"><span data-stu-id="033c6-186">Example</span></span>
##### <a name="request"></a><span data-ttu-id="033c6-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="033c6-187">Request</span></span>
<span data-ttu-id="033c6-188">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="033c6-188">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="033c6-189">Ответ</span><span class="sxs-lookup"><span data-stu-id="033c6-189">Response</span></span>
<span data-ttu-id="033c6-190">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="033c6-190">Here is an example of the response.</span></span>

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update privilegedRoleSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
