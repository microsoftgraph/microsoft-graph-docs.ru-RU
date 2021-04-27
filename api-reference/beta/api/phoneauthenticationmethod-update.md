---
title: Обновление phoneAuthenticationMethod
description: Обновление номера телефона, связанного с объектом phoneAuthenticationMethod.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 5230ca00a63f3543b95ef4f2a1dc7242c5460a1b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055409"
---
# <a name="update-phoneauthenticationmethod"></a><span data-ttu-id="f5ac7-103">Обновление phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f5ac7-103">Update phoneAuthenticationMethod</span></span>

<span data-ttu-id="f5ac7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5ac7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5ac7-105">Обновление номера телефона, связанного с [методом проверки подлинности телефона.](../resources/phoneauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="f5ac7-105">Update the phone number associated with a [phone authentication method](../resources/phoneauthenticationmethod.md).</span></span>

<span data-ttu-id="f5ac7-106">Вы не можете изменить тип телефона.</span><span class="sxs-lookup"><span data-stu-id="f5ac7-106">You can't change a phone's type.</span></span> <span data-ttu-id="f5ac7-107">Чтобы изменить тип телефона, добавьте новый номер нужного типа и удалите объект с помощью исходного типа.</span><span class="sxs-lookup"><span data-stu-id="f5ac7-107">To change a phone's type, add a new number of the desired type and then delete the object with the original type.</span></span>

<span data-ttu-id="f5ac7-108">Если политика позволяет пользователю использовать SMS для входа и изменить номер, система попытается зарегистрировать номер для использования `mobile` в этой системе.</span><span class="sxs-lookup"><span data-stu-id="f5ac7-108">If a user is enabled by policy to use SMS to sign in and the `mobile` number is changed, the system will attempt to register the number for use in that system.</span></span>

## <a name="permissions"></a><span data-ttu-id="f5ac7-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f5ac7-109">Permissions</span></span>

<span data-ttu-id="f5ac7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5ac7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="f5ac7-112">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="f5ac7-112">Permissions acting on self</span></span>

|<span data-ttu-id="f5ac7-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f5ac7-113">Permission type</span></span>      | <span data-ttu-id="f5ac7-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f5ac7-114">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="f5ac7-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f5ac7-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="f5ac7-116">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f5ac7-116">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="f5ac7-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f5ac7-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5ac7-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5ac7-118">Not supported.</span></span> |
| <span data-ttu-id="f5ac7-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f5ac7-119">Application</span></span>                            | <span data-ttu-id="f5ac7-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5ac7-120">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="f5ac7-121">Разрешения, действующие на других пользователей</span><span class="sxs-lookup"><span data-stu-id="f5ac7-121">Permissions acting on other users</span></span>

|<span data-ttu-id="f5ac7-122">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f5ac7-122">Permission type</span></span>      | <span data-ttu-id="f5ac7-123">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f5ac7-123">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="f5ac7-124">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f5ac7-124">Delegated (work or school account)</span></span>     | <span data-ttu-id="f5ac7-125">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5ac7-125">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="f5ac7-126">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f5ac7-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5ac7-127">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5ac7-127">Not supported.</span></span> |
| <span data-ttu-id="f5ac7-128">Приложение</span><span class="sxs-lookup"><span data-stu-id="f5ac7-128">Application</span></span>                            | <span data-ttu-id="f5ac7-129">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5ac7-129">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="f5ac7-130">Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="f5ac7-130">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="f5ac7-131">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="f5ac7-131">Global admin</span></span>
* <span data-ttu-id="f5ac7-132">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="f5ac7-132">Privileged authentication admin</span></span>
* <span data-ttu-id="f5ac7-133">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="f5ac7-133">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="f5ac7-134">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f5ac7-134">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /me/authentication/phoneMethods/{id}
PUT /users/{id | userPrincipalName}/authentication/phoneMethods/{id}
```
<span data-ttu-id="f5ac7-135">Значение, `id` соответствующее обновлению phoneType, является одним из следующих:</span><span class="sxs-lookup"><span data-stu-id="f5ac7-135">The value of `id` corresponding to the phoneType to update is one of the following:</span></span>
+ <span data-ttu-id="f5ac7-136">`b6332ec1-7057-4abe-9331-3d72feddfe41` обновление `alternateMobile` **phoneType**.</span><span class="sxs-lookup"><span data-stu-id="f5ac7-136">`b6332ec1-7057-4abe-9331-3d72feddfe41` to update the `alternateMobile` **phoneType**.</span></span>
+ <span data-ttu-id="f5ac7-137">`e37fc753-ff3b-4958-9484-eaa9425c82bc` обновление `office` **phoneType**.</span><span class="sxs-lookup"><span data-stu-id="f5ac7-137">`e37fc753-ff3b-4958-9484-eaa9425c82bc` to update the `office` **phoneType**.</span></span>
+ <span data-ttu-id="f5ac7-138">`3179e48a-750b-4051-897c-87b9720928f7` обновление `mobile` **phoneType**.</span><span class="sxs-lookup"><span data-stu-id="f5ac7-138">`3179e48a-750b-4051-897c-87b9720928f7` to update the `mobile` **phoneType**.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f5ac7-139">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f5ac7-139">Request headers</span></span>

| <span data-ttu-id="f5ac7-140">Имя</span><span class="sxs-lookup"><span data-stu-id="f5ac7-140">Name</span></span>       | <span data-ttu-id="f5ac7-141">Описание</span><span class="sxs-lookup"><span data-stu-id="f5ac7-141">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f5ac7-142">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f5ac7-142">Authorization</span></span> | <span data-ttu-id="f5ac7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f5ac7-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f5ac7-145">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f5ac7-145">Content-type</span></span>  | <span data-ttu-id="f5ac7-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f5ac7-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f5ac7-148">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f5ac7-148">Request body</span></span>

<span data-ttu-id="f5ac7-149">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="f5ac7-149">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="f5ac7-150">Существующие свойства, не включенные в тело запроса, будут пересчитаны в зависимости от изменений в других значениях свойств.</span><span class="sxs-lookup"><span data-stu-id="f5ac7-150">Existing properties that are not included in the request body will be recalculated based on changes to other property values.</span></span>

| <span data-ttu-id="f5ac7-151">Свойство</span><span class="sxs-lookup"><span data-stu-id="f5ac7-151">Property</span></span>     | <span data-ttu-id="f5ac7-152">Тип</span><span class="sxs-lookup"><span data-stu-id="f5ac7-152">Type</span></span>        | <span data-ttu-id="f5ac7-153">Описание</span><span class="sxs-lookup"><span data-stu-id="f5ac7-153">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f5ac7-154">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="f5ac7-154">phoneNumber</span></span>|<span data-ttu-id="f5ac7-155">String</span><span class="sxs-lookup"><span data-stu-id="f5ac7-155">String</span></span>|<span data-ttu-id="f5ac7-156">Номер телефона для текста или вызова для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="f5ac7-156">The phone number to text or call for authentication.</span></span> <span data-ttu-id="f5ac7-157">Телефон номера используют формат "+ \<country code\> \<number\> \<extension\> x", с необязательным расширением.</span><span class="sxs-lookup"><span data-stu-id="f5ac7-157">Phone numbers use the format "+\<country code\> \<number\>x\<extension\>", with extension optional.</span></span> <span data-ttu-id="f5ac7-158">Например, допустимы +1 5555551234 или +1 5555551234x1233.</span><span class="sxs-lookup"><span data-stu-id="f5ac7-158">For example, +1 5555551234 or +1 5555551234x123 are valid.</span></span> <span data-ttu-id="f5ac7-159">При создании и обновлении номера отклоняется, если они не соответствуют требуемой форме.</span><span class="sxs-lookup"><span data-stu-id="f5ac7-159">Numbers are rejected when creating/updating if they do not match the required format.</span></span>|
|<span data-ttu-id="f5ac7-160">phoneType</span><span class="sxs-lookup"><span data-stu-id="f5ac7-160">phoneType</span></span>|<span data-ttu-id="f5ac7-161">String</span><span class="sxs-lookup"><span data-stu-id="f5ac7-161">string</span></span>| <span data-ttu-id="f5ac7-162">Возможные значения: `mobile`, `alternateMobile` или `office`.</span><span class="sxs-lookup"><span data-stu-id="f5ac7-162">Possible values are: `mobile`, `alternateMobile`, or `office`.</span></span>|

## <a name="response"></a><span data-ttu-id="f5ac7-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5ac7-163">Response</span></span>

<span data-ttu-id="f5ac7-164">В случае успешной работы этот метод возвращает код ответа и обновленный `200 OK` [объект phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f5ac7-164">If successful, this method returns a `200 OK` response code and an updated [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f5ac7-165">Примеры</span><span class="sxs-lookup"><span data-stu-id="f5ac7-165">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f5ac7-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="f5ac7-166">Request</span></span>

<span data-ttu-id="f5ac7-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f5ac7-167">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f5ac7-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="f5ac7-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_phoneauthenticationmethod"
}-->

```http
PUT https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7
Content-type: application/json

{
  "phoneNumber": "+1 2065555554",
  "phoneType": "mobile",
}
```
# <a name="c"></a>[<span data-ttu-id="f5ac7-169">C#</span><span class="sxs-lookup"><span data-stu-id="f5ac7-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-phoneauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f5ac7-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f5ac7-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-phoneauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f5ac7-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f5ac7-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-phoneauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f5ac7-172">Java</span><span class="sxs-lookup"><span data-stu-id="f5ac7-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-phoneauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f5ac7-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5ac7-173">Response</span></span>

<span data-ttu-id="f5ac7-174">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f5ac7-174">The following is an example of the response.</span></span>

> <span data-ttu-id="f5ac7-175">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f5ac7-175">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.phoneAuthenticationMethod"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "phoneNumber": "+1 2065555554",
  "phoneType": "mobile",
  "smsSignInState": "ready",
  "id": "3179e48a-750b-4051-897c-87b9720928f7"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update phoneauthenticationmethod",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
