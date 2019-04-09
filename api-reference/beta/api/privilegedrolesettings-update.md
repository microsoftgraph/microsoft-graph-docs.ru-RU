---
title: Обновление Привилежедролесеттингс
description: Обновление параметров роли для данного параметра роли. Будет возвращен объект Привилежедролесеттингс.
localization_priority: Normal
ms.openlocfilehash: 779b0d4cd61672c90c103ebb2545cb75324273fd
ms.sourcegitcommit: 9fd437a77da99d8436d6c852edd99a9ba873f8cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/09/2019
ms.locfileid: "31560117"
---
# <a name="update-privilegedrolesettings"></a><span data-ttu-id="c2ecf-104">Обновление Привилежедролесеттингс</span><span class="sxs-lookup"><span data-stu-id="c2ecf-104">Update privilegedRoleSettings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2ecf-105">Обновление параметров роли для данного параметра роли.</span><span class="sxs-lookup"><span data-stu-id="c2ecf-105">Update the role settings for the given role setting.</span></span> <span data-ttu-id="c2ecf-106">Будет возвращен объект [привилежедролесеттингс](../resources/privilegedrolesettings.md) .</span><span class="sxs-lookup"><span data-stu-id="c2ecf-106">A [privilegedRoleSettings](../resources/privilegedrolesettings.md) object will be returned.</span></span>
## <a name="permissions"></a><span data-ttu-id="c2ecf-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c2ecf-107">Permissions</span></span>

<span data-ttu-id="c2ecf-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2ecf-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="c2ecf-110">**Примечание:** Запрашивающая сторона должна иметь одну из следующих ролей: привилегированный администратор ролей, глобальный администратор, администратор безопасности или средство чтения безопасности.</span><span class="sxs-lookup"><span data-stu-id="c2ecf-110">**Note:** The requester must have one of the following roles: Privileged Role Administrator, Global Administrator, Security Administrator, or Security Reader.</span></span> 

|<span data-ttu-id="c2ecf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2ecf-111">Permission type</span></span>      | <span data-ttu-id="c2ecf-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2ecf-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2ecf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2ecf-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c2ecf-114">Привилежедакцесс. ReadWrite. AzureAD, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="c2ecf-114">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c2ecf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2ecf-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2ecf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2ecf-116">Not supported.</span></span>    |
|<span data-ttu-id="c2ecf-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c2ecf-117">Application</span></span> | <span data-ttu-id="c2ecf-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2ecf-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c2ecf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2ecf-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /privilegedRoles/{id}/settings
```

## <a name="request-headers"></a><span data-ttu-id="c2ecf-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c2ecf-120">Request headers</span></span>
| <span data-ttu-id="c2ecf-121">Имя</span><span class="sxs-lookup"><span data-stu-id="c2ecf-121">Name</span></span>      |<span data-ttu-id="c2ecf-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c2ecf-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c2ecf-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c2ecf-123">Authorization</span></span>  | <span data-ttu-id="c2ecf-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c2ecf-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c2ecf-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c2ecf-126">Request body</span></span>
<span data-ttu-id="c2ecf-127">В тексте запроса добавьте представление объекта [Привилежедролесеттингс](../resources/privilegedrolesettings.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2ecf-127">In the request body, supply a JSON representation of a [privilegedRoleSettings](../resources/privilegedrolesettings.md) object.</span></span>

<span data-ttu-id="c2ecf-128">В следующей таблице перечислены свойства, которые можно предоставить при обновлении параметров роли.</span><span class="sxs-lookup"><span data-stu-id="c2ecf-128">The following table lists the properties that you can supply when you update a role setting.</span></span>

|<span data-ttu-id="c2ecf-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2ecf-129">Property</span></span>|<span data-ttu-id="c2ecf-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c2ecf-130">Type</span></span>|<span data-ttu-id="c2ecf-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c2ecf-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c2ecf-132">Елеватиондуратион</span><span class="sxs-lookup"><span data-stu-id="c2ecf-132">elevationDuration</span></span>|<span data-ttu-id="c2ecf-133">duration</span><span class="sxs-lookup"><span data-stu-id="c2ecf-133">duration</span></span>|<span data-ttu-id="c2ecf-134">Продолжительность активации роли.</span><span class="sxs-lookup"><span data-stu-id="c2ecf-134">The duration when the role is activated.</span></span> <span data-ttu-id="c2ecf-135">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c2ecf-135">Required.</span></span>|
|<span data-ttu-id="c2ecf-136">id</span><span class="sxs-lookup"><span data-stu-id="c2ecf-136">id</span></span>|<span data-ttu-id="c2ecf-137">string</span><span class="sxs-lookup"><span data-stu-id="c2ecf-137">string</span></span>|<span data-ttu-id="c2ecf-138">Уникальный идентификатор для параметров роли.</span><span class="sxs-lookup"><span data-stu-id="c2ecf-138">The unique identifier for the role settings.</span></span> <span data-ttu-id="c2ecf-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c2ecf-139">Read-only.</span></span> <span data-ttu-id="c2ecf-140">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="c2ecf-140">Required.</span></span>|
|<span data-ttu-id="c2ecf-141">Исмфаонелеватионконфигурабле</span><span class="sxs-lookup"><span data-stu-id="c2ecf-141">isMfaOnElevationConfigurable</span></span>|<span data-ttu-id="c2ecf-142">логический</span><span class="sxs-lookup"><span data-stu-id="c2ecf-142">boolean</span></span>|<span data-ttu-id="c2ecf-143">**значение true** , если мфаонелеватион является настраиваемым.</span><span class="sxs-lookup"><span data-stu-id="c2ecf-143">**true** if mfaOnElevation is configurable.</span></span> <span data-ttu-id="c2ecf-144">**false** , если мфаонелеватион не является настраиваемым.</span><span class="sxs-lookup"><span data-stu-id="c2ecf-144">**false** if mfaOnElevation is not configurable.</span></span> <span data-ttu-id="c2ecf-145">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="c2ecf-145">Required.</span></span>|
|<span data-ttu-id="c2ecf-146">Ластглобаладмин</span><span class="sxs-lookup"><span data-stu-id="c2ecf-146">lastGlobalAdmin</span></span>|<span data-ttu-id="c2ecf-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2ecf-147">Boolean</span></span>|<span data-ttu-id="c2ecf-148">Только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="c2ecf-148">For internal use only.</span></span>|
|<span data-ttu-id="c2ecf-149">Макселаватиондуратион</span><span class="sxs-lookup"><span data-stu-id="c2ecf-149">maxElavationDuration</span></span>|<span data-ttu-id="c2ecf-150">duration</span><span class="sxs-lookup"><span data-stu-id="c2ecf-150">duration</span></span>|<span data-ttu-id="c2ecf-151">Максимальная длительность активированной роли.</span><span class="sxs-lookup"><span data-stu-id="c2ecf-151">Maximum duration for the activated role.</span></span> <span data-ttu-id="c2ecf-152">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="c2ecf-152">Required.</span></span>|
|<span data-ttu-id="c2ecf-153">Мфаонелеватион</span><span class="sxs-lookup"><span data-stu-id="c2ecf-153">mfaOnElevation</span></span>|<span data-ttu-id="c2ecf-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2ecf-154">Boolean</span></span>|<span data-ttu-id="c2ecf-155">**значение true** , если для активации роли требуется mfa.</span><span class="sxs-lookup"><span data-stu-id="c2ecf-155">**true** if MFA is required to activate the role.</span></span> <span data-ttu-id="c2ecf-156">**false** , если MFA не требуется для активации роли.</span><span class="sxs-lookup"><span data-stu-id="c2ecf-156">**false** if MFA is not required to activate the role.</span></span> <span data-ttu-id="c2ecf-157">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="c2ecf-157">Required.</span></span>|
|<span data-ttu-id="c2ecf-158">Минелеватиондуратион</span><span class="sxs-lookup"><span data-stu-id="c2ecf-158">minElevationDuration</span></span>|<span data-ttu-id="c2ecf-159">duration</span><span class="sxs-lookup"><span data-stu-id="c2ecf-159">duration</span></span>|<span data-ttu-id="c2ecf-160">Минимальная длительность активированной роли.</span><span class="sxs-lookup"><span data-stu-id="c2ecf-160">Minimum duration for the activated role.</span></span> <span data-ttu-id="c2ecf-161">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="c2ecf-161">Required.</span></span>|
|<span data-ttu-id="c2ecf-162">Нотификатионтаусеронелеватион</span><span class="sxs-lookup"><span data-stu-id="c2ecf-162">notificationToUserOnElevation</span></span>|<span data-ttu-id="c2ecf-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2ecf-163">Boolean</span></span>|<span data-ttu-id="c2ecf-164">**имеет значение true** , если вы отправляете уведомление конечному пользователю при активации роли.</span><span class="sxs-lookup"><span data-stu-id="c2ecf-164">**true** if send notification to the end user when the role is activated.</span></span> <span data-ttu-id="c2ecf-165">**значение false** , если уведомление не отправляется при активации роли.</span><span class="sxs-lookup"><span data-stu-id="c2ecf-165">**false** if do not send notification when the role is activated.</span></span> <span data-ttu-id="c2ecf-166">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="c2ecf-166">Required.</span></span>|
|<span data-ttu-id="c2ecf-167">Тиккетингинфунелеватион</span><span class="sxs-lookup"><span data-stu-id="c2ecf-167">ticketingInfoOnElevation</span></span>|<span data-ttu-id="c2ecf-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2ecf-168">Boolean</span></span>|<span data-ttu-id="c2ecf-169">**имеет значение true** , если при активации роли требуются сведения о билетах.</span><span class="sxs-lookup"><span data-stu-id="c2ecf-169">**true** if the ticketing information is required when activate the role.</span></span> <span data-ttu-id="c2ecf-170">**false** , если при активации роли не требуются сведения о билетах.</span><span class="sxs-lookup"><span data-stu-id="c2ecf-170">**false** if the ticketing information is not required when activate the role.</span></span> <span data-ttu-id="c2ecf-171">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="c2ecf-171">Required.</span></span>|
|<span data-ttu-id="c2ecf-172">Аппровалонелеватион</span><span class="sxs-lookup"><span data-stu-id="c2ecf-172">approvalOnElevation</span></span>|<span data-ttu-id="c2ecf-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2ecf-173">Boolean</span></span>|<span data-ttu-id="c2ecf-174">**имеет значение true** , если при активации роли необходимо выполнить утверждение.</span><span class="sxs-lookup"><span data-stu-id="c2ecf-174">**true** if the approval is required when activate the role.</span></span> <span data-ttu-id="c2ecf-175">**false** , если при активации роли не нужно утверждать.</span><span class="sxs-lookup"><span data-stu-id="c2ecf-175">**false** if the approval is not required when activate the role.</span></span> <span data-ttu-id="c2ecf-176">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="c2ecf-176">Required.</span></span>|
|<span data-ttu-id="c2ecf-177">Аппроверидс</span><span class="sxs-lookup"><span data-stu-id="c2ecf-177">approverIds</span></span>|<span data-ttu-id="c2ecf-178">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c2ecf-178">String collection</span></span>|<span data-ttu-id="c2ecf-179">Список идентификаторов утверждения, если для активации необходимо утверждение.</span><span class="sxs-lookup"><span data-stu-id="c2ecf-179">List of Approval IDs, if approval is required for activation.</span></span>|

## <a name="response"></a><span data-ttu-id="c2ecf-180">Ответ</span><span class="sxs-lookup"><span data-stu-id="c2ecf-180">Response</span></span>

<span data-ttu-id="c2ecf-181">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c2ecf-181">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="c2ecf-182">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="c2ecf-182">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="c2ecf-183">В противном случае будет возвращен код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="c2ecf-183">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="c2ecf-184">Пример</span><span class="sxs-lookup"><span data-stu-id="c2ecf-184">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c2ecf-185">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2ecf-185">Request</span></span>
<span data-ttu-id="c2ecf-186">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2ecf-186">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="c2ecf-187">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2ecf-187">Response</span></span>
<span data-ttu-id="c2ecf-188">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c2ecf-188">Here is an example of the response.</span></span>
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
    "Error: /api-reference/beta/api/privilegedrolesettings-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
