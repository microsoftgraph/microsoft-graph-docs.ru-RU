---
title: Обновление phoneAuthenticationMethod
description: Обновление номера телефона, связанного с объектом phoneAuthenticationMethod.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ae9f5bc036fd75e72bc7d698aa715447f1be552f
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796628"
---
# <a name="update-phoneauthenticationmethod"></a><span data-ttu-id="03995-103">Обновление phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="03995-103">Update phoneAuthenticationMethod</span></span>

<span data-ttu-id="03995-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03995-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03995-105">Обновление номера телефона, связанного с [методом проверки подлинности телефона.](../resources/phoneauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="03995-105">Update the phone number associated with a [phone authentication method](../resources/phoneauthenticationmethod.md).</span></span>

<span data-ttu-id="03995-106">Тип телефона изменить нельзя.</span><span class="sxs-lookup"><span data-stu-id="03995-106">You can't change a phone's type.</span></span> <span data-ttu-id="03995-107">Чтобы изменить тип телефона, добавьте новый номер нужного типа, а затем удалите объект с исходным типом.</span><span class="sxs-lookup"><span data-stu-id="03995-107">To change a phone's type, add a new number of the desired type and then delete the object with the original type.</span></span>

<span data-ttu-id="03995-108">Если пользователю по политике включено использование SMS для входа и номер изменен, система попытается зарегистрировать номер для использования `mobile` в этой системе.</span><span class="sxs-lookup"><span data-stu-id="03995-108">If a user is enabled by policy to use SMS to sign in and the `mobile` number is changed, the system will attempt to register the number for use in that system.</span></span>

## <a name="permissions"></a><span data-ttu-id="03995-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="03995-109">Permissions</span></span>

<span data-ttu-id="03995-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03995-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="03995-112">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="03995-112">Permissions acting on self</span></span>

|<span data-ttu-id="03995-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03995-113">Permission type</span></span>      | <span data-ttu-id="03995-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="03995-114">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="03995-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03995-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="03995-116">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03995-116">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="03995-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03995-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03995-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03995-118">Not supported.</span></span> |
| <span data-ttu-id="03995-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="03995-119">Application</span></span>                            | <span data-ttu-id="03995-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03995-120">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="03995-121">Разрешения, действующие с другими пользователями</span><span class="sxs-lookup"><span data-stu-id="03995-121">Permissions acting on other users</span></span>

|<span data-ttu-id="03995-122">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03995-122">Permission type</span></span>      | <span data-ttu-id="03995-123">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="03995-123">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="03995-124">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03995-124">Delegated (work or school account)</span></span>     | <span data-ttu-id="03995-125">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03995-125">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="03995-126">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03995-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03995-127">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03995-127">Not supported.</span></span> |
| <span data-ttu-id="03995-128">Приложение</span><span class="sxs-lookup"><span data-stu-id="03995-128">Application</span></span>                            | <span data-ttu-id="03995-129">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03995-129">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="03995-130">Для делегирования сценариев, в которых администратор действует над другим пользователем, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="03995-130">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="03995-131">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="03995-131">Global admin</span></span>
* <span data-ttu-id="03995-132">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="03995-132">Privileged authentication admin</span></span>
* <span data-ttu-id="03995-133">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="03995-133">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="03995-134">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03995-134">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /me/authentication/phoneMethods/{id}
PUT /users/{id | userPrincipalName}/authentication/phoneMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="03995-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="03995-135">Request headers</span></span>

| <span data-ttu-id="03995-136">Имя</span><span class="sxs-lookup"><span data-stu-id="03995-136">Name</span></span>       | <span data-ttu-id="03995-137">Описание</span><span class="sxs-lookup"><span data-stu-id="03995-137">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="03995-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="03995-138">Authorization</span></span> | <span data-ttu-id="03995-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03995-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="03995-141">Content-Type</span><span class="sxs-lookup"><span data-stu-id="03995-141">Content-type</span></span>  | <span data-ttu-id="03995-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03995-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="03995-144">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="03995-144">Request body</span></span>

<span data-ttu-id="03995-145">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="03995-145">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="03995-146">Существующие свойства, не включенные в тело запроса, будут пересчитаны на основе изменений других значений свойств.</span><span class="sxs-lookup"><span data-stu-id="03995-146">Existing properties that are not included in the request body will be recalculated based on changes to other property values.</span></span>

| <span data-ttu-id="03995-147">Свойство</span><span class="sxs-lookup"><span data-stu-id="03995-147">Property</span></span>     | <span data-ttu-id="03995-148">Тип</span><span class="sxs-lookup"><span data-stu-id="03995-148">Type</span></span>        | <span data-ttu-id="03995-149">Описание</span><span class="sxs-lookup"><span data-stu-id="03995-149">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="03995-150">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="03995-150">phoneNumber</span></span>|<span data-ttu-id="03995-151">String</span><span class="sxs-lookup"><span data-stu-id="03995-151">String</span></span>|<span data-ttu-id="03995-152">Номер телефона для текста или вызов для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="03995-152">The phone number to text or call for authentication.</span></span> <span data-ttu-id="03995-153">Номера телефонов используют формат "+ \<country code\> \<number\> \<extension\> x", с необязательным расширением.</span><span class="sxs-lookup"><span data-stu-id="03995-153">Phone numbers use the format "+\<country code\> \<number\>x\<extension\>", with extension optional.</span></span> <span data-ttu-id="03995-154">Например, допустимы +1 5555551234 или +1 5555551234x123.</span><span class="sxs-lookup"><span data-stu-id="03995-154">For example, +1 5555551234 or +1 5555551234x123 are valid.</span></span> <span data-ttu-id="03995-155">Числа отклоняется при создании или обновлении, если они не соответствуют требуемму формату.</span><span class="sxs-lookup"><span data-stu-id="03995-155">Numbers are rejected when creating/updating if they do not match the required format.</span></span>|
|<span data-ttu-id="03995-156">phoneType</span><span class="sxs-lookup"><span data-stu-id="03995-156">phoneType</span></span>|<span data-ttu-id="03995-157">string</span><span class="sxs-lookup"><span data-stu-id="03995-157">string</span></span>| <span data-ttu-id="03995-158">Возможные значения: `mobile` , , или `alternateMobile` `office` .</span><span class="sxs-lookup"><span data-stu-id="03995-158">Possible values are: `mobile`, `alternateMobile`, or `office`.</span></span>|

## <a name="response"></a><span data-ttu-id="03995-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="03995-159">Response</span></span>

<span data-ttu-id="03995-160">В случае успеха этот метод возвращает код отклика и обновленный объект `200 OK` [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="03995-160">If successful, this method returns a `200 OK` response code and an updated [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="03995-161">Примеры</span><span class="sxs-lookup"><span data-stu-id="03995-161">Examples</span></span>

### <a name="request"></a><span data-ttu-id="03995-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="03995-162">Request</span></span>

<span data-ttu-id="03995-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="03995-163">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="03995-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="03995-164">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="03995-165">C#</span><span class="sxs-lookup"><span data-stu-id="03995-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-phoneauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="03995-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="03995-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-phoneauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="03995-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="03995-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-phoneauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="03995-168">Java</span><span class="sxs-lookup"><span data-stu-id="03995-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-phoneauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="03995-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="03995-169">Response</span></span>

<span data-ttu-id="03995-170">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="03995-170">The following is an example of the response.</span></span>

> <span data-ttu-id="03995-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="03995-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
