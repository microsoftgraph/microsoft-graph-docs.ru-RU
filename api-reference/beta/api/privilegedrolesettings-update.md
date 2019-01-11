---
title: Обновление privilegedRoleSettings
description: Обновление параметров ролей для параметров указанного ролей. Объект privilegedRoleSettings будут возвращены.
localization_priority: Normal
ms.openlocfilehash: 7c117abfe774eae60e42dcbc5f748c10cacf5cd6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819322"
---
# <a name="update-privilegedrolesettings"></a><span data-ttu-id="b6a44-104">Обновление privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="b6a44-104">Update privilegedRoleSettings</span></span>

> <span data-ttu-id="b6a44-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b6a44-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b6a44-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6a44-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b6a44-107">Обновление параметров ролей для параметров указанного ролей.</span><span class="sxs-lookup"><span data-stu-id="b6a44-107">Update the role settings for the given role setting.</span></span> <span data-ttu-id="b6a44-108">Объект [privilegedRoleSettings](../resources/privilegedrolesettings.md) будут возвращены.</span><span class="sxs-lookup"><span data-stu-id="b6a44-108">A [privilegedRoleSettings](../resources/privilegedrolesettings.md) object will be returned.</span></span>
## <a name="permissions"></a><span data-ttu-id="b6a44-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b6a44-109">Permissions</span></span>

<span data-ttu-id="b6a44-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6a44-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="b6a44-112">**Примечание:** Источник запроса, должны использовать одну из следующих ролей: привилегированной роль администратора, глобального администратора, администратора безопасности или безопасности чтения.</span><span class="sxs-lookup"><span data-stu-id="b6a44-112">**Note:** The requester must have one of the following roles: Privileged Role Administrator, Global Administrator, Security Administrator, or Security Reader.</span></span> 

|<span data-ttu-id="b6a44-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b6a44-113">Permission type</span></span>      | <span data-ttu-id="b6a44-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b6a44-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b6a44-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b6a44-115">Delegated (work or school account)</span></span> | <span data-ttu-id="b6a44-116">PrivilegedAccess.ReadWrite.AzureAD Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b6a44-116">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b6a44-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b6a44-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6a44-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6a44-118">Not supported.</span></span>    |
|<span data-ttu-id="b6a44-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b6a44-119">Application</span></span> | <span data-ttu-id="b6a44-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6a44-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b6a44-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b6a44-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /privilegedRoles/{id}/settings
```

## <a name="request-headers"></a><span data-ttu-id="b6a44-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b6a44-122">Request headers</span></span>
| <span data-ttu-id="b6a44-123">Имя</span><span class="sxs-lookup"><span data-stu-id="b6a44-123">Name</span></span>      |<span data-ttu-id="b6a44-124">Описание</span><span class="sxs-lookup"><span data-stu-id="b6a44-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b6a44-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b6a44-125">Authorization</span></span>  | <span data-ttu-id="b6a44-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b6a44-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b6a44-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b6a44-128">Request body</span></span>
<span data-ttu-id="b6a44-129">В тексте запроса укажите представление JSON объекта [privilegedRoleSettings](../resources/privilegedrolesettings.md) .</span><span class="sxs-lookup"><span data-stu-id="b6a44-129">In the request body, supply a JSON representation of a [privilegedRoleSettings](../resources/privilegedrolesettings.md) object.</span></span>

<span data-ttu-id="b6a44-130">В следующей таблице приведены свойства, которые можно указать при обновлении параметров ролей.</span><span class="sxs-lookup"><span data-stu-id="b6a44-130">The following table lists the properties that you can supply when you update a role setting.</span></span>

|<span data-ttu-id="b6a44-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="b6a44-131">Property</span></span>|<span data-ttu-id="b6a44-132">Тип</span><span class="sxs-lookup"><span data-stu-id="b6a44-132">Type</span></span>|<span data-ttu-id="b6a44-133">Описание</span><span class="sxs-lookup"><span data-stu-id="b6a44-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b6a44-134">elevationDuration</span><span class="sxs-lookup"><span data-stu-id="b6a44-134">elevationDuration</span></span>|<span data-ttu-id="b6a44-135">duration</span><span class="sxs-lookup"><span data-stu-id="b6a44-135">duration</span></span>|<span data-ttu-id="b6a44-136">Длительность, при активации роли.</span><span class="sxs-lookup"><span data-stu-id="b6a44-136">The duration when the role is activated.</span></span> <span data-ttu-id="b6a44-137">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b6a44-137">Required.</span></span>|
|<span data-ttu-id="b6a44-138">id</span><span class="sxs-lookup"><span data-stu-id="b6a44-138">id</span></span>|<span data-ttu-id="b6a44-139">строка</span><span class="sxs-lookup"><span data-stu-id="b6a44-139">string</span></span>|<span data-ttu-id="b6a44-140">Уникальный идентификатор для параметров роли.</span><span class="sxs-lookup"><span data-stu-id="b6a44-140">The unique identifier for the role settings.</span></span> <span data-ttu-id="b6a44-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b6a44-141">Read-only.</span></span> <span data-ttu-id="b6a44-142">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b6a44-142">Required.</span></span>|
|<span data-ttu-id="b6a44-143">isMfaOnElevationConfigurable</span><span class="sxs-lookup"><span data-stu-id="b6a44-143">isMfaOnElevationConfigurable</span></span>|<span data-ttu-id="b6a44-144">boolean</span><span class="sxs-lookup"><span data-stu-id="b6a44-144">boolean</span></span>|<span data-ttu-id="b6a44-145">**значение true,** Если mfaOnElevation может быть настроен.</span><span class="sxs-lookup"><span data-stu-id="b6a44-145">**true** if mfaOnElevation is configurable.</span></span> <span data-ttu-id="b6a44-146">**значение false,** Если mfaOnElevation не настраивается.</span><span class="sxs-lookup"><span data-stu-id="b6a44-146">**false** if mfaOnElevation is not configurable.</span></span> <span data-ttu-id="b6a44-147">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b6a44-147">Required.</span></span>|
|<span data-ttu-id="b6a44-148">lastGlobalAdmin</span><span class="sxs-lookup"><span data-stu-id="b6a44-148">lastGlobalAdmin</span></span>|<span data-ttu-id="b6a44-149">Логический</span><span class="sxs-lookup"><span data-stu-id="b6a44-149">Boolean</span></span>|<span data-ttu-id="b6a44-150">Только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="b6a44-150">For internal use only.</span></span>|
|<span data-ttu-id="b6a44-151">maxElavationDuration</span><span class="sxs-lookup"><span data-stu-id="b6a44-151">maxElavationDuration</span></span>|<span data-ttu-id="b6a44-152">duration</span><span class="sxs-lookup"><span data-stu-id="b6a44-152">duration</span></span>|<span data-ttu-id="b6a44-153">Максимальная длительность для активации роли.</span><span class="sxs-lookup"><span data-stu-id="b6a44-153">Maximum duration for the activated role.</span></span> <span data-ttu-id="b6a44-154">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b6a44-154">Required.</span></span>|
|<span data-ttu-id="b6a44-155">mfaOnElevation</span><span class="sxs-lookup"><span data-stu-id="b6a44-155">mfaOnElevation</span></span>|<span data-ttu-id="b6a44-156">Логический</span><span class="sxs-lookup"><span data-stu-id="b6a44-156">Boolean</span></span>|<span data-ttu-id="b6a44-157">**значение true,** Если необходимо активировать роль многофакторной проверкой Подлинности.</span><span class="sxs-lookup"><span data-stu-id="b6a44-157">**true** if MFA is required to activate the role.</span></span> <span data-ttu-id="b6a44-158">**значение false,** Если многофакторной проверкой Подлинности не требуется для включения роли.</span><span class="sxs-lookup"><span data-stu-id="b6a44-158">**false** if MFA is not required to activate the role.</span></span> <span data-ttu-id="b6a44-159">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b6a44-159">Required.</span></span>|
|<span data-ttu-id="b6a44-160">minElevationDuration</span><span class="sxs-lookup"><span data-stu-id="b6a44-160">minElevationDuration</span></span>|<span data-ttu-id="b6a44-161">duration</span><span class="sxs-lookup"><span data-stu-id="b6a44-161">duration</span></span>|<span data-ttu-id="b6a44-162">Минимальная продолжительность активированные роли.</span><span class="sxs-lookup"><span data-stu-id="b6a44-162">Minimum duration for the activated role.</span></span> <span data-ttu-id="b6a44-163">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b6a44-163">Required.</span></span>|
|<span data-ttu-id="b6a44-164">notificationToUserOnElevation</span><span class="sxs-lookup"><span data-stu-id="b6a44-164">notificationToUserOnElevation</span></span>|<span data-ttu-id="b6a44-165">Логический</span><span class="sxs-lookup"><span data-stu-id="b6a44-165">Boolean</span></span>|<span data-ttu-id="b6a44-166">**значение true,** Если отправить уведомление конечному пользователю при активации роли.</span><span class="sxs-lookup"><span data-stu-id="b6a44-166">**true** if send notification to the end user when the role is activated.</span></span> <span data-ttu-id="b6a44-167">**значение false,** Если не отправлять уведомления при активации роли.</span><span class="sxs-lookup"><span data-stu-id="b6a44-167">**false** if do not send notification when the role is activated.</span></span> <span data-ttu-id="b6a44-168">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b6a44-168">Required.</span></span>|
|<span data-ttu-id="b6a44-169">ticketingInfoOnElevation</span><span class="sxs-lookup"><span data-stu-id="b6a44-169">ticketingInfoOnElevation</span></span>|<span data-ttu-id="b6a44-170">Логический</span><span class="sxs-lookup"><span data-stu-id="b6a44-170">Boolean</span></span>|<span data-ttu-id="b6a44-171">**значение true,** Если отдела сведения требуется при активации роли.</span><span class="sxs-lookup"><span data-stu-id="b6a44-171">**true** if the ticketing information is required when activate the role.</span></span> <span data-ttu-id="b6a44-172">**значение false,** Если отдела сведения не является обязательным, когда активировать роль.</span><span class="sxs-lookup"><span data-stu-id="b6a44-172">**false** if the ticketing information is not required when activate the role.</span></span> <span data-ttu-id="b6a44-173">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b6a44-173">Required.</span></span>|
|<span data-ttu-id="b6a44-174">approvalOnElevation</span><span class="sxs-lookup"><span data-stu-id="b6a44-174">approvalOnElevation</span></span>|<span data-ttu-id="b6a44-175">Логический</span><span class="sxs-lookup"><span data-stu-id="b6a44-175">Boolean</span></span>|<span data-ttu-id="b6a44-176">**значение true,** Если требуется утверждение при активации роли.</span><span class="sxs-lookup"><span data-stu-id="b6a44-176">**true** if the approval is required when activate the role.</span></span> <span data-ttu-id="b6a44-177">**значение false,** Если утверждение не является обязательным, когда активировать роль.</span><span class="sxs-lookup"><span data-stu-id="b6a44-177">**false** if the approval is not required when activate the role.</span></span> <span data-ttu-id="b6a44-178">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b6a44-178">Required.</span></span>|
|<span data-ttu-id="b6a44-179">approverIds</span><span class="sxs-lookup"><span data-stu-id="b6a44-179">approverIds</span></span>|<span data-ttu-id="b6a44-180">array</span><span class="sxs-lookup"><span data-stu-id="b6a44-180">array</span></span>|<span data-ttu-id="b6a44-181">Список идентификаторов утверждения, если требуется для активации утверждение.</span><span class="sxs-lookup"><span data-stu-id="b6a44-181">List of Approval IDs, if approval is required for activation.</span></span>|

## <a name="response"></a><span data-ttu-id="b6a44-182">Ответ</span><span class="sxs-lookup"><span data-stu-id="b6a44-182">Response</span></span>

<span data-ttu-id="b6a44-183">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b6a44-183">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="b6a44-184">Обратите внимание, что необходимо зарегистрировать для PIM клиента.</span><span class="sxs-lookup"><span data-stu-id="b6a44-184">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="b6a44-185">В противном случае будут возвращены код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="b6a44-185">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="b6a44-186">Пример</span><span class="sxs-lookup"><span data-stu-id="b6a44-186">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b6a44-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="b6a44-187">Request</span></span>
<span data-ttu-id="b6a44-188">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b6a44-188">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="b6a44-189">Ответ</span><span class="sxs-lookup"><span data-stu-id="b6a44-189">Response</span></span>
<span data-ttu-id="b6a44-190">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b6a44-190">Here is an example of the response.</span></span>

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
