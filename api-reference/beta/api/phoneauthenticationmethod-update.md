---
title: Обновление Фонеаусентикатионмесод
description: Обновление номера телефона, связанного с объектом Фонеаусентикатионмесод.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 994fd1173f1b2622d1aa67d046ebb6102c6e3a1a
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48402648"
---
# <a name="update-phoneauthenticationmethod"></a><span data-ttu-id="2945f-103">Обновление Фонеаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="2945f-103">Update phoneAuthenticationMethod</span></span>

<span data-ttu-id="2945f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2945f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2945f-105">Обновление номера телефона, связанного с [методом проверки подлинности по телефону](../resources/phoneauthenticationmethod.md).</span><span class="sxs-lookup"><span data-stu-id="2945f-105">Update the phone number associated with a [phone authentication method](../resources/phoneauthenticationmethod.md).</span></span>

<span data-ttu-id="2945f-106">Тип телефона изменить нельзя.</span><span class="sxs-lookup"><span data-stu-id="2945f-106">You can't change a phone's type.</span></span> <span data-ttu-id="2945f-107">Чтобы изменить тип телефона, добавьте новый номер нужного типа, а затем удалите объект с исходным типом.</span><span class="sxs-lookup"><span data-stu-id="2945f-107">To change a phone's type, add a new number of the desired type and then delete the object with the original type.</span></span>

<span data-ttu-id="2945f-108">Если для входа в систему пользователь включен с помощью политики SMS и `mobile` изменился номер, система попытается зарегистрировать номер для использования в этой системе.</span><span class="sxs-lookup"><span data-stu-id="2945f-108">If a user is enabled by policy to use SMS to sign in and the `mobile` number is changed, the system will attempt to register the number for use in that system.</span></span>

## <a name="permissions"></a><span data-ttu-id="2945f-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2945f-109">Permissions</span></span>

<span data-ttu-id="2945f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2945f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2945f-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2945f-112">Permission type</span></span>                        | <span data-ttu-id="2945f-113">Разрешения, действующие на себя (по крайней мере для самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="2945f-113">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="2945f-114">Разрешения, действующие на других (по крайней мере для самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="2945f-114">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="2945f-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2945f-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="2945f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2945f-116">Not supported.</span></span> | <span data-ttu-id="2945f-117">Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="2945f-117">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="2945f-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2945f-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2945f-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2945f-119">Not supported.</span></span> | <span data-ttu-id="2945f-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2945f-120">Not supported.</span></span> |
| <span data-ttu-id="2945f-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2945f-121">Application</span></span>                            | <span data-ttu-id="2945f-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2945f-122">Not supported.</span></span> | <span data-ttu-id="2945f-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2945f-123">Not supported.</span></span> |

<span data-ttu-id="2945f-124">Для делегированных сценариев, в которых администратор работает с другим пользователем, администратору необходима [одна из следующих ролей](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="2945f-124">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="2945f-125">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="2945f-125">Global admin</span></span>
* <span data-ttu-id="2945f-126">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="2945f-126">Privileged authentication admin</span></span>
* <span data-ttu-id="2945f-127">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="2945f-127">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="2945f-128">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2945f-128">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /me/authentication/phoneMethods/{id}
PUT /users/{id}/authentication/phoneMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2945f-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2945f-129">Request headers</span></span>

| <span data-ttu-id="2945f-130">Имя</span><span class="sxs-lookup"><span data-stu-id="2945f-130">Name</span></span>       | <span data-ttu-id="2945f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2945f-131">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="2945f-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2945f-132">Authorization</span></span> | <span data-ttu-id="2945f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2945f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2945f-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2945f-135">Content-type</span></span>  | <span data-ttu-id="2945f-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2945f-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2945f-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2945f-138">Request body</span></span>

<span data-ttu-id="2945f-139">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="2945f-139">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="2945f-140">Существующие свойства, не включенные в текст запроса, будут пересчитаны на основе изменений, внесенных в другие значения свойств.</span><span class="sxs-lookup"><span data-stu-id="2945f-140">Existing properties that are not included in the request body will be recalculated based on changes to other property values.</span></span>

| <span data-ttu-id="2945f-141">Свойство</span><span class="sxs-lookup"><span data-stu-id="2945f-141">Property</span></span>     | <span data-ttu-id="2945f-142">Тип</span><span class="sxs-lookup"><span data-stu-id="2945f-142">Type</span></span>        | <span data-ttu-id="2945f-143">Описание</span><span class="sxs-lookup"><span data-stu-id="2945f-143">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2945f-144">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="2945f-144">phoneNumber</span></span>|<span data-ttu-id="2945f-145">String</span><span class="sxs-lookup"><span data-stu-id="2945f-145">String</span></span>|<span data-ttu-id="2945f-146">Номер телефона для текста или вызов для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="2945f-146">The phone number to text or call for authentication.</span></span> <span data-ttu-id="2945f-147">Номера телефонов используют формат "+ \<country code\> \<number\> x \<extension\> " с необязательным расширением.</span><span class="sxs-lookup"><span data-stu-id="2945f-147">Phone numbers use the format "+\<country code\> \<number\>x\<extension\>", with extension optional.</span></span> <span data-ttu-id="2945f-148">Например, допустимые + 1 5555551234 или + 1 5555551234x123.</span><span class="sxs-lookup"><span data-stu-id="2945f-148">For example, +1 5555551234 or +1 5555551234x123 are valid.</span></span> <span data-ttu-id="2945f-149">При создании или обновлении числа отклоняются, если они не совпадают с требуемым форматом.</span><span class="sxs-lookup"><span data-stu-id="2945f-149">Numbers are rejected when creating/updating if they do not match the required format.</span></span>|
|<span data-ttu-id="2945f-150">фонетипе</span><span class="sxs-lookup"><span data-stu-id="2945f-150">phoneType</span></span>|<span data-ttu-id="2945f-151">string</span><span class="sxs-lookup"><span data-stu-id="2945f-151">string</span></span>| <span data-ttu-id="2945f-152">Возможные значения: `mobile` , `alternateMobile` , или `office` .</span><span class="sxs-lookup"><span data-stu-id="2945f-152">Possible values are: `mobile`, `alternateMobile`, or `office`.</span></span>|

## <a name="response"></a><span data-ttu-id="2945f-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="2945f-153">Response</span></span>

<span data-ttu-id="2945f-154">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [фонеаусентикатионмесод](../resources/phoneauthenticationmethod.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2945f-154">If successful, this method returns a `200 OK` response code and an updated [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2945f-155">Примеры</span><span class="sxs-lookup"><span data-stu-id="2945f-155">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2945f-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="2945f-156">Request</span></span>

<span data-ttu-id="2945f-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2945f-157">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2945f-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="2945f-158">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="2945f-159">C#</span><span class="sxs-lookup"><span data-stu-id="2945f-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-phoneauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2945f-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2945f-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-phoneauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2945f-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2945f-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-phoneauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2945f-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="2945f-162">Response</span></span>

<span data-ttu-id="2945f-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2945f-163">The following is an example of the response.</span></span>

> <span data-ttu-id="2945f-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2945f-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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