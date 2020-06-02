---
title: Обновление аусоризатионполици
description: Обновление свойств объекта Аусоризатионполици.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ac605e93603cb39491fd980e78a9b0f0026541eb
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44492224"
---
# <a name="update-authorizationpolicy"></a><span data-ttu-id="7e865-103">Обновление Аусоризатионполици</span><span class="sxs-lookup"><span data-stu-id="7e865-103">Update authorizationPolicy</span></span>

<span data-ttu-id="7e865-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e865-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e865-105">Обновление свойств объекта [аусоризатионполици](../resources/authorizationpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="7e865-105">Update the properties of a [authorizationPolicy](../resources/authorizationpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7e865-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7e865-106">Permissions</span></span>

<span data-ttu-id="7e865-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e865-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7e865-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7e865-109">Permission type</span></span>                        | <span data-ttu-id="7e865-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7e865-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7e865-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7e865-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7e865-112">Policy. ReadWrite. Authorization</span><span class="sxs-lookup"><span data-stu-id="7e865-112">Policy.ReadWrite.Authorization</span></span>|
| <span data-ttu-id="7e865-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7e865-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e865-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e865-114">Not supported.</span></span> |
| <span data-ttu-id="7e865-115">Сервер приложений</span><span class="sxs-lookup"><span data-stu-id="7e865-115">Application</span></span>                            | <span data-ttu-id="7e865-116">Policy. ReadWrite. Authorization</span><span class="sxs-lookup"><span data-stu-id="7e865-116">Policy.ReadWrite.Authorization</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e865-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7e865-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/authorizationPolicy/authorizationPolicy
```

## <a name="request-headers"></a><span data-ttu-id="7e865-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7e865-118">Request headers</span></span>

| <span data-ttu-id="7e865-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7e865-119">Name</span></span>       | <span data-ttu-id="7e865-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7e865-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="7e865-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e865-121">Authorization</span></span> | <span data-ttu-id="7e865-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="7e865-122">Bearer {token}</span></span> |
| <span data-ttu-id="7e865-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7e865-123">Content-type</span></span> | <span data-ttu-id="7e865-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7e865-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="7e865-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7e865-125">Request body</span></span>

<span data-ttu-id="7e865-126">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="7e865-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="7e865-127">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="7e865-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="7e865-128">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="7e865-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7e865-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="7e865-129">Property</span></span>     | <span data-ttu-id="7e865-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7e865-130">Type</span></span>        | <span data-ttu-id="7e865-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7e865-131">Description</span></span> |
|:-------------|:------------|:------------|  
|<span data-ttu-id="7e865-132">displayName</span><span class="sxs-lookup"><span data-stu-id="7e865-132">displayName</span></span>|<span data-ttu-id="7e865-133">Строка</span><span class="sxs-lookup"><span data-stu-id="7e865-133">String</span></span>| <span data-ttu-id="7e865-134">Отображаемое имя для этой политики.</span><span class="sxs-lookup"><span data-stu-id="7e865-134">Display name for this policy.</span></span> |  
|<span data-ttu-id="7e865-135">description</span><span class="sxs-lookup"><span data-stu-id="7e865-135">description</span></span>|<span data-ttu-id="7e865-136">String</span><span class="sxs-lookup"><span data-stu-id="7e865-136">String</span></span>| <span data-ttu-id="7e865-137">Описание этой политики.</span><span class="sxs-lookup"><span data-stu-id="7e865-137">Description of this policy.</span></span> |  
|<span data-ttu-id="7e865-138">гуестусерролеид</span><span class="sxs-lookup"><span data-stu-id="7e865-138">guestUserRoleId</span></span>|<span data-ttu-id="7e865-139">Guid</span><span class="sxs-lookup"><span data-stu-id="7e865-139">Guid</span></span>| <span data-ttu-id="7e865-140">Представляет templateId роли для роли, которая должна быть выделена пользователю "гость".</span><span class="sxs-lookup"><span data-stu-id="7e865-140">Represents role templateId for the role that should be granted to guest user.</span></span> <span data-ttu-id="7e865-141">Обратитесь к [списку унифиедроледефинитионс](https://docs.microsoft.com/graph/api/rbacapplication-list-roledefinitions?view=graph-rest-beta&tabs=http) , чтобы найти список доступных шаблонов ролей.</span><span class="sxs-lookup"><span data-stu-id="7e865-141">Refer to [List unifiedRoleDefinitions](https://docs.microsoft.com/graph/api/rbacapplication-list-roledefinitions?view=graph-rest-beta&tabs=http) to find the list of available role templates.</span></span> <span data-ttu-id="7e865-142">Только поддерживаемые роли: User (a0b1b346-4d3e-4e8b-98f8-753987be4970), гость (10dae51f-b6af-4016-8d66-8c2a99b929b3) и пользователь с ограниченным гостями (2af84b1e-32c8-42b7-82bc-daa82404023b).</span><span class="sxs-lookup"><span data-stu-id="7e865-142">Only supported roles today are User (a0b1b346-4d3e-4e8b-98f8-753987be4970), Guest User (10dae51f-b6af-4016-8d66-8c2a99b929b3), and Restricted Guest User (2af84b1e-32c8-42b7-82bc-daa82404023b).</span></span> | 
|<span data-ttu-id="7e865-143">енабледпревиевфеатурес</span><span class="sxs-lookup"><span data-stu-id="7e865-143">enabledPreviewFeatures</span></span>|<span data-ttu-id="7e865-144">Коллекция (String)</span><span class="sxs-lookup"><span data-stu-id="7e865-144">Collection(string)</span></span>| <span data-ttu-id="7e865-145">Список компонентов, включенных для закрытой предварительной версии в клиенте.</span><span class="sxs-lookup"><span data-stu-id="7e865-145">List of features enabled for private preview on the tenant.</span></span> | 
|<span data-ttu-id="7e865-146">блоккмсолповершелл</span><span class="sxs-lookup"><span data-stu-id="7e865-146">blockMsolPowerShell</span></span>|<span data-ttu-id="7e865-147">Логический</span><span class="sxs-lookup"><span data-stu-id="7e865-147">Boolean</span></span>| <span data-ttu-id="7e865-148">Чтобы отключить использование MSOL PowerShell, задайте для этого свойства значение `true` .</span><span class="sxs-lookup"><span data-stu-id="7e865-148">To disable the use of MSOL PowerShell, set this property to `true`.</span></span> <span data-ttu-id="7e865-149">Параметр `true` также отключит доступ пользователей к устаревшей конечной точке службы, используемой MSOL PowerShell.</span><span class="sxs-lookup"><span data-stu-id="7e865-149">Setting to `true` will also disable user-based access to the legacy service endpoint used by MSOL PowerShell.</span></span> <span data-ttu-id="7e865-150">Это не повлияет на Azure AD Connect или Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7e865-150">This does not affect Azure AD Connect or Microsoft Graph.</span></span> | 

## <a name="response"></a><span data-ttu-id="7e865-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e865-151">Response</span></span>

<span data-ttu-id="7e865-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7e865-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7e865-154">Примеры</span><span class="sxs-lookup"><span data-stu-id="7e865-154">Examples</span></span>

### <a name="example-1-update-or-set-guest-user-access-level-for-the-tenant"></a><span data-ttu-id="7e865-155">Пример 1: обновление или Настройка уровня доступа гостей для клиента</span><span class="sxs-lookup"><span data-stu-id="7e865-155">Example 1: Update or set Guest user access level for the tenant</span></span>

#### <a name="request"></a><span data-ttu-id="7e865-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="7e865-156">Request</span></span>

<span data-ttu-id="7e865-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7e865-157">The following is an example of the request.</span></span> <span data-ttu-id="7e865-158">В этом примере уровень гостевого доступа изменяется на "ограниченный гостевой пользователь".</span><span class="sxs-lookup"><span data-stu-id="7e865-158">In this example, guest access level is modified to Restricted Guest User.</span></span>

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy
{
  "guestUserRole": "2af84b1e-32c8-42b7-82bc-daa82404023b"
}

```
#### <a name="response"></a><span data-ttu-id="7e865-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="7e865-159">Response</span></span>

<span data-ttu-id="7e865-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7e865-160">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicyPolicy"
} -->

```http
HTTP/1.1 204 No Content

```

### <a name="example-2-enable-new-feature-for-preview-on-tenant"></a><span data-ttu-id="7e865-161">Пример 2: включение новой функции для предварительного просмотра в клиенте</span><span class="sxs-lookup"><span data-stu-id="7e865-161">Example 2: Enable new feature for preview on tenant</span></span>

#### <a name="request"></a><span data-ttu-id="7e865-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="7e865-162">Request</span></span>

<span data-ttu-id="7e865-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7e865-163">The following is an example of the request.</span></span>

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy
{
  "enabledPreviewFeatures": ["assignGroupsToRoles"]
}

```
#### <a name="response"></a><span data-ttu-id="7e865-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e865-164">Response</span></span>

<span data-ttu-id="7e865-165">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7e865-165">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicyPolicy"
} -->

```http
HTTP/1.1 204 No Content
```


### <a name="example-3-block-msol-powershell-in-tenant"></a><span data-ttu-id="7e865-166">Пример 3: Блокировка MSOL PowerShell в клиенте</span><span class="sxs-lookup"><span data-stu-id="7e865-166">Example 3: Block MSOL PowerShell in tenant</span></span>

#### <a name="request"></a><span data-ttu-id="7e865-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="7e865-167">Request</span></span>

<span data-ttu-id="7e865-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7e865-168">The following is an example of the request.</span></span>

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy
{
  "blockMsolPowerShell": true
}

```
#### <a name="response"></a><span data-ttu-id="7e865-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e865-169">Response</span></span>

<span data-ttu-id="7e865-170">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7e865-170">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicyPolicy"
} -->

```http
HTTP/1.1 204 No Content
```
