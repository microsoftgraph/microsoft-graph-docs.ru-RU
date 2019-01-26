---
title: Обновление privilegedRoleSettings
description: Обновление параметров ролей для параметров указанного ролей. Объект privilegedRoleSettings будут возвращены.
localization_priority: Normal
ms.openlocfilehash: 7b49d228372e2fa122f9461706f782c60cfea379
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577272"
---
# <a name="update-privilegedrolesettings"></a><span data-ttu-id="beb19-104">Обновление privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="beb19-104">Update privilegedRoleSettings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="beb19-105">Обновление параметров ролей для параметров указанного ролей.</span><span class="sxs-lookup"><span data-stu-id="beb19-105">Update the role settings for the given role setting.</span></span> <span data-ttu-id="beb19-106">Объект [privilegedRoleSettings](../resources/privilegedrolesettings.md) будут возвращены.</span><span class="sxs-lookup"><span data-stu-id="beb19-106">A [privilegedRoleSettings](../resources/privilegedrolesettings.md) object will be returned.</span></span>
## <a name="permissions"></a><span data-ttu-id="beb19-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="beb19-107">Permissions</span></span>

<span data-ttu-id="beb19-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="beb19-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="beb19-110">**Примечание:** Источник запроса, должны использовать одну из следующих ролей: привилегированной роль администратора, глобального администратора, администратора безопасности или безопасности чтения.</span><span class="sxs-lookup"><span data-stu-id="beb19-110">**Note:** The requester must have one of the following roles: Privileged Role Administrator, Global Administrator, Security Administrator, or Security Reader.</span></span> 

|<span data-ttu-id="beb19-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="beb19-111">Permission type</span></span>      | <span data-ttu-id="beb19-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="beb19-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="beb19-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="beb19-113">Delegated (work or school account)</span></span> | <span data-ttu-id="beb19-114">PrivilegedAccess.ReadWrite.AzureAD Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="beb19-114">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="beb19-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="beb19-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="beb19-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="beb19-116">Not supported.</span></span>    |
|<span data-ttu-id="beb19-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="beb19-117">Application</span></span> | <span data-ttu-id="beb19-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="beb19-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="beb19-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="beb19-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /privilegedRoles/{id}/settings
```

## <a name="request-headers"></a><span data-ttu-id="beb19-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="beb19-120">Request headers</span></span>
| <span data-ttu-id="beb19-121">Имя</span><span class="sxs-lookup"><span data-stu-id="beb19-121">Name</span></span>      |<span data-ttu-id="beb19-122">Описание</span><span class="sxs-lookup"><span data-stu-id="beb19-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="beb19-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="beb19-123">Authorization</span></span>  | <span data-ttu-id="beb19-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="beb19-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="beb19-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="beb19-126">Request body</span></span>
<span data-ttu-id="beb19-127">В тексте запроса укажите представление JSON объекта [privilegedRoleSettings](../resources/privilegedrolesettings.md) .</span><span class="sxs-lookup"><span data-stu-id="beb19-127">In the request body, supply a JSON representation of a [privilegedRoleSettings](../resources/privilegedrolesettings.md) object.</span></span>

<span data-ttu-id="beb19-128">В следующей таблице приведены свойства, которые можно указать при обновлении параметров ролей.</span><span class="sxs-lookup"><span data-stu-id="beb19-128">The following table lists the properties that you can supply when you update a role setting.</span></span>

|<span data-ttu-id="beb19-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="beb19-129">Property</span></span>|<span data-ttu-id="beb19-130">Тип</span><span class="sxs-lookup"><span data-stu-id="beb19-130">Type</span></span>|<span data-ttu-id="beb19-131">Описание</span><span class="sxs-lookup"><span data-stu-id="beb19-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="beb19-132">elevationDuration</span><span class="sxs-lookup"><span data-stu-id="beb19-132">elevationDuration</span></span> |<span data-ttu-id="beb19-133">String (метка времени)</span><span class="sxs-lookup"><span data-stu-id="beb19-133">String (timestamp)</span></span> |<span data-ttu-id="beb19-134">Длительность, при активации роли.</span><span class="sxs-lookup"><span data-stu-id="beb19-134">The duration when the role is activated.</span></span> <span data-ttu-id="beb19-135">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="beb19-135">Required.</span></span>|
|<span data-ttu-id="beb19-136">id</span><span class="sxs-lookup"><span data-stu-id="beb19-136">id</span></span>| <span data-ttu-id="beb19-137">String (идентификатор)</span><span class="sxs-lookup"><span data-stu-id="beb19-137">string (identifier)</span></span> |<span data-ttu-id="beb19-138">Уникальный идентификатор для параметров роли.</span><span class="sxs-lookup"><span data-stu-id="beb19-138">The unique identifier for the role settings.</span></span> <span data-ttu-id="beb19-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="beb19-139">Read-only.</span></span> <span data-ttu-id="beb19-140">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="beb19-140">Required.</span></span>|
|<span data-ttu-id="beb19-141">isMfaOnElevationConfigurable</span><span class="sxs-lookup"><span data-stu-id="beb19-141">isMfaOnElevationConfigurable</span></span>|<span data-ttu-id="beb19-142">boolean</span><span class="sxs-lookup"><span data-stu-id="beb19-142">boolean</span></span>|<span data-ttu-id="beb19-143">**значение true,** Если mfaOnElevation может быть настроен.</span><span class="sxs-lookup"><span data-stu-id="beb19-143">**true** if mfaOnElevation is configurable.</span></span> <span data-ttu-id="beb19-144">**значение false,** Если mfaOnElevation не настраивается.</span><span class="sxs-lookup"><span data-stu-id="beb19-144">**false** if mfaOnElevation is not configurable.</span></span> <span data-ttu-id="beb19-145">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="beb19-145">Required.</span></span>|
|<span data-ttu-id="beb19-146">lastGlobalAdmin</span><span class="sxs-lookup"><span data-stu-id="beb19-146">lastGlobalAdmin</span></span>| <span data-ttu-id="beb19-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="beb19-147">Boolean</span></span> |<span data-ttu-id="beb19-148">Только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="beb19-148">For internal use only.</span></span>|
|<span data-ttu-id="beb19-149">maxElavationDuration</span><span class="sxs-lookup"><span data-stu-id="beb19-149">maxElavationDuration</span></span>| <span data-ttu-id="beb19-150">String (метка времени)</span><span class="sxs-lookup"><span data-stu-id="beb19-150">String (timestamp)</span></span>|<span data-ttu-id="beb19-151">Максимальная длительность для активации роли.</span><span class="sxs-lookup"><span data-stu-id="beb19-151">Maximum duration for the activated role.</span></span> <span data-ttu-id="beb19-152">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="beb19-152">Required.</span></span>|
|<span data-ttu-id="beb19-153">mfaOnElevation</span><span class="sxs-lookup"><span data-stu-id="beb19-153">mfaOnElevation</span></span>| <span data-ttu-id="beb19-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="beb19-154">Boolean</span></span> |<span data-ttu-id="beb19-155">**значение true,** Если необходимо активировать роль многофакторной проверкой Подлинности.</span><span class="sxs-lookup"><span data-stu-id="beb19-155">**true** if MFA is required to activate the role.</span></span> <span data-ttu-id="beb19-156">**значение false,** Если многофакторной проверкой Подлинности не требуется для включения роли.</span><span class="sxs-lookup"><span data-stu-id="beb19-156">**false** if MFA is not required to activate the role.</span></span> <span data-ttu-id="beb19-157">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="beb19-157">Required.</span></span>|
|<span data-ttu-id="beb19-158">minElevationDuration</span><span class="sxs-lookup"><span data-stu-id="beb19-158">minElevationDuration</span></span>| <span data-ttu-id="beb19-159">String (метка времени)</span><span class="sxs-lookup"><span data-stu-id="beb19-159">String (timestamp)</span></span> |<span data-ttu-id="beb19-160">Минимальная продолжительность активированные роли.</span><span class="sxs-lookup"><span data-stu-id="beb19-160">Minimum duration for the activated role.</span></span> <span data-ttu-id="beb19-161">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="beb19-161">Required.</span></span>|
|<span data-ttu-id="beb19-162">notificationToUserOnElevation</span><span class="sxs-lookup"><span data-stu-id="beb19-162">notificationToUserOnElevation</span></span>|<span data-ttu-id="beb19-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="beb19-163">Boolean</span></span>|<span data-ttu-id="beb19-164">**значение true,** Если отправить уведомление конечному пользователю при активации роли.</span><span class="sxs-lookup"><span data-stu-id="beb19-164">**true** if send notification to the end user when the role is activated.</span></span> <span data-ttu-id="beb19-165">**значение false,** Если не отправлять уведомления при активации роли.</span><span class="sxs-lookup"><span data-stu-id="beb19-165">**false** if do not send notification when the role is activated.</span></span> <span data-ttu-id="beb19-166">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="beb19-166">Required.</span></span>|
|<span data-ttu-id="beb19-167">ticketingInfoOnElevation</span><span class="sxs-lookup"><span data-stu-id="beb19-167">ticketingInfoOnElevation</span></span>|<span data-ttu-id="beb19-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="beb19-168">Boolean</span></span>|<span data-ttu-id="beb19-169">**значение true,** Если отдела сведения требуется при активации роли.</span><span class="sxs-lookup"><span data-stu-id="beb19-169">**true** if the ticketing information is required when activate the role.</span></span> <span data-ttu-id="beb19-170">**значение false,** Если отдела сведения не является обязательным, когда активировать роль.</span><span class="sxs-lookup"><span data-stu-id="beb19-170">**false** if the ticketing information is not required when activate the role.</span></span> <span data-ttu-id="beb19-171">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="beb19-171">Required.</span></span>|
|<span data-ttu-id="beb19-172">approvalOnElevation</span><span class="sxs-lookup"><span data-stu-id="beb19-172">approvalOnElevation</span></span>|<span data-ttu-id="beb19-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="beb19-173">Boolean</span></span>|<span data-ttu-id="beb19-174">**значение true,** Если требуется утверждение при активации роли.</span><span class="sxs-lookup"><span data-stu-id="beb19-174">**true** if the approval is required when activate the role.</span></span> <span data-ttu-id="beb19-175">**значение false,** Если утверждение не является обязательным, когда активировать роль.</span><span class="sxs-lookup"><span data-stu-id="beb19-175">**false** if the approval is not required when activate the role.</span></span> <span data-ttu-id="beb19-176">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="beb19-176">Required.</span></span>|
|<span data-ttu-id="beb19-177">approverIds</span><span class="sxs-lookup"><span data-stu-id="beb19-177">approverIds</span></span>| <span data-ttu-id="beb19-178">Коллекция строк (идентификатор)</span><span class="sxs-lookup"><span data-stu-id="beb19-178">String (identifier) collection</span></span>|<span data-ttu-id="beb19-179">Список идентификаторов утверждения, если требуется для активации утверждение.</span><span class="sxs-lookup"><span data-stu-id="beb19-179">List of Approval IDs, if approval is required for activation.</span></span>|

## <a name="response"></a><span data-ttu-id="beb19-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="beb19-180">Response</span></span>

<span data-ttu-id="beb19-181">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="beb19-181">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="beb19-182">Обратите внимание, что необходимо зарегистрировать для PIM клиента.</span><span class="sxs-lookup"><span data-stu-id="beb19-182">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="beb19-183">В противном случае будут возвращены код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="beb19-183">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="beb19-184">Пример</span><span class="sxs-lookup"><span data-stu-id="beb19-184">Example</span></span>
##### <a name="request"></a><span data-ttu-id="beb19-185">Запрос</span><span class="sxs-lookup"><span data-stu-id="beb19-185">Request</span></span>
<span data-ttu-id="beb19-186">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="beb19-186">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="beb19-187">Отклик</span><span class="sxs-lookup"><span data-stu-id="beb19-187">Response</span></span>
<span data-ttu-id="beb19-188">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="beb19-188">Here is an example of the response.</span></span>

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
    "Error: /api-reference/beta/api/privilegedrolesettings-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
