---
title: Создание temporaryAccessPassAuthenticationMethod
description: Создание нового объекта temporaryAccessPassAuthenticationMethod.
author: inbarckMS
ms.author: inbarc
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 801f82d30baf5a231b0fea78c3613773d4dd8f53
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761095"
---
# <a name="create-temporaryaccesspassauthenticationmethod"></a><span data-ttu-id="9efcb-103">Создание temporaryAccessPassAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="9efcb-103">Create temporaryAccessPassAuthenticationMethod</span></span>
<span data-ttu-id="9efcb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9efcb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9efcb-105">Создайте новый [объект temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) для пользователя.</span><span class="sxs-lookup"><span data-stu-id="9efcb-105">Create a new [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) object on a user.</span></span> <span data-ttu-id="9efcb-106">У пользователя может быть только один временный пропуск доступа.</span><span class="sxs-lookup"><span data-stu-id="9efcb-106">A user can only have one Temporary Access Pass.</span></span> <span data-ttu-id="9efcb-107">Пароль можно использовать между началом и конечным временем временного пропуска доступа.</span><span class="sxs-lookup"><span data-stu-id="9efcb-107">The passcode can be used between the start and end time of the Temporary Access Pass.</span></span> <span data-ttu-id="9efcb-108">Если пользователю требуется новый временный пропуск доступа:</span><span class="sxs-lookup"><span data-stu-id="9efcb-108">If the user requires a new Temporary Access Pass:</span></span>
* <span data-ttu-id="9efcb-109">Хотя текущий пропуск временного доступа действителен, администратору необходимо удалить существующий временный пропуск доступа и создать новый пропуск для пользователя.</span><span class="sxs-lookup"><span data-stu-id="9efcb-109">While the current Temporary Access Pass is valid – the admin needs to delete the existing Temporary Access Pass and create a new pass on the user.</span></span> <span data-ttu-id="9efcb-110">Удаление допустимой временной пропускной записи отзовет сеансы пользователя.</span><span class="sxs-lookup"><span data-stu-id="9efcb-110">Deleting a valid Temporary Access Pass will revoke the user’s sessions.</span></span> 
* <span data-ttu-id="9efcb-111">После истечения срока действия временного пропуска доступа новый временный пропуск переопределит текущий временный пропуск доступа и не отменит сеансы пользователя.</span><span class="sxs-lookup"><span data-stu-id="9efcb-111">After the Temporary Access Pass has expired – a new temporary access pass overrides the current temporary access pass and doesn't revoke the user’s sessions.</span></span>


## <a name="permissions"></a><span data-ttu-id="9efcb-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9efcb-112">Permissions</span></span>

<span data-ttu-id="9efcb-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9efcb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="9efcb-115">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="9efcb-115">Permissions acting on self</span></span>

|<span data-ttu-id="9efcb-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9efcb-116">Permission type</span></span>      | <span data-ttu-id="9efcb-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9efcb-117">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="9efcb-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9efcb-118">Delegated (work or school account)</span></span>     | <span data-ttu-id="9efcb-119">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9efcb-119">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="9efcb-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9efcb-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9efcb-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9efcb-121">Not supported.</span></span> |
| <span data-ttu-id="9efcb-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9efcb-122">Application</span></span>                            | <span data-ttu-id="9efcb-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9efcb-123">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="9efcb-124">Разрешения, действующие на других пользователей</span><span class="sxs-lookup"><span data-stu-id="9efcb-124">Permissions acting on other users</span></span>

|<span data-ttu-id="9efcb-125">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9efcb-125">Permission type</span></span>      | <span data-ttu-id="9efcb-126">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9efcb-126">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="9efcb-127">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9efcb-127">Delegated (work or school account)</span></span>     | <span data-ttu-id="9efcb-128">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9efcb-128">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="9efcb-129">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9efcb-129">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9efcb-130">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9efcb-130">Not supported.</span></span> |
| <span data-ttu-id="9efcb-131">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9efcb-131">Application</span></span>                            | <span data-ttu-id="9efcb-132">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9efcb-132">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="9efcb-133">Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="9efcb-133">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="9efcb-134">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="9efcb-134">Global admin</span></span>
* <span data-ttu-id="9efcb-135">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="9efcb-135">Privileged authentication admin</span></span>
* <span data-ttu-id="9efcb-136">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="9efcb-136">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="9efcb-137">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9efcb-137">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{id | userPrincipalName}/authentication/temporaryAccessPassMethods
```

## <a name="request-headers"></a><span data-ttu-id="9efcb-138">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9efcb-138">Request headers</span></span>
|<span data-ttu-id="9efcb-139">Имя</span><span class="sxs-lookup"><span data-stu-id="9efcb-139">Name</span></span>|<span data-ttu-id="9efcb-140">Описание</span><span class="sxs-lookup"><span data-stu-id="9efcb-140">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9efcb-141">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9efcb-141">Authorization</span></span>|<span data-ttu-id="9efcb-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9efcb-p104">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="9efcb-144">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9efcb-144">Content-Type</span></span>|<span data-ttu-id="9efcb-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9efcb-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9efcb-147">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9efcb-147">Request body</span></span>
<span data-ttu-id="9efcb-148">В теле запроса поставляем представление JSON объекта [temporaryAccessPassAuthenticationMethod.](../resources/temporaryaccesspassauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="9efcb-148">In the request body, supply a JSON representation of the [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) object.</span></span>

<span data-ttu-id="9efcb-149">В следующей таблице описываются необязательные свойства, которые можно использовать при создании [временногоAccessPassAuthenticationMethod.](../resources/temporaryaccesspassauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="9efcb-149">The following table describes optional properties that can be used when creating the [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md).</span></span>

|<span data-ttu-id="9efcb-150">Свойство</span><span class="sxs-lookup"><span data-stu-id="9efcb-150">Property</span></span>|<span data-ttu-id="9efcb-151">Тип</span><span class="sxs-lookup"><span data-stu-id="9efcb-151">Type</span></span>|<span data-ttu-id="9efcb-152">Описание</span><span class="sxs-lookup"><span data-stu-id="9efcb-152">Description</span></span>|<span data-ttu-id="9efcb-153">Обязательная</span><span class="sxs-lookup"><span data-stu-id="9efcb-153">Required</span></span>| 
|:---|:---|:---|:---|
|<span data-ttu-id="9efcb-154">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9efcb-154">startDateTime</span></span>|<span data-ttu-id="9efcb-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9efcb-155">DateTimeOffset</span></span>|<span data-ttu-id="9efcb-156">Дата и время, когда временныйAccessPass станет доступным для использования, если не задать временный пропуск доступа, можно использовать во время создания.</span><span class="sxs-lookup"><span data-stu-id="9efcb-156">The date and time when the temporaryAccessPass becomes available to use, if not set the Temporary Access Pass is available to use at creation time.</span></span>| <span data-ttu-id="9efcb-157">Нет</span><span class="sxs-lookup"><span data-stu-id="9efcb-157">No</span></span>|
|<span data-ttu-id="9efcb-158">lifetimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="9efcb-158">lifetimeInMinutes</span></span>|<span data-ttu-id="9efcb-159">Int32</span><span class="sxs-lookup"><span data-stu-id="9efcb-159">Int32</span></span>|<span data-ttu-id="9efcb-160">Срок службы temporaryAccessPass в минутах, начиная с момента создания или при наборе startDateTime.</span><span class="sxs-lookup"><span data-stu-id="9efcb-160">The lifetime of the temporaryAccessPass in minutes starting at creation time or at startDateTime, if set.</span></span> <span data-ttu-id="9efcb-161">Минимум 10, максимум 43200 (эквивалент 30 дней).</span><span class="sxs-lookup"><span data-stu-id="9efcb-161">Minimum 10, Maximum 43200 (equivalent to 30 days).</span></span>| <span data-ttu-id="9efcb-162">Нет</span><span class="sxs-lookup"><span data-stu-id="9efcb-162">No</span></span>|
|<span data-ttu-id="9efcb-163">isUsableOnce</span><span class="sxs-lookup"><span data-stu-id="9efcb-163">isUsableOnce</span></span>|<span data-ttu-id="9efcb-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="9efcb-164">Boolean</span></span>|<span data-ttu-id="9efcb-165">Определяет, ограничен ли пропуск одно время использования.</span><span class="sxs-lookup"><span data-stu-id="9efcb-165">Determines if the pass is limited to a one time use.</span></span> <span data-ttu-id="9efcb-166">Если true — пропуск можно использовать один раз, если false — пропуск можно использовать несколько раз в течение временного времени службыAccessPass.</span><span class="sxs-lookup"><span data-stu-id="9efcb-166">If True – the pass can be used once, if False – the pass can be used multiple times within the temporaryAccessPass life time.</span></span> <span data-ttu-id="9efcb-167">Многоцелевой временный пропуск доступа (isUsableOnce = false) может быть создан и использован для регистрации, если это разрешено политикой метода проверки подлинности временного доступа.</span><span class="sxs-lookup"><span data-stu-id="9efcb-167">A multi-use Temporary Access Pass (isUsableOnce = false), can only be created and used for sign-in if it is allowed by the Temporary Access Pass Authentication method policy.</span></span>|  <span data-ttu-id="9efcb-168">Нет</span><span class="sxs-lookup"><span data-stu-id="9efcb-168">No</span></span>|



## <a name="response"></a><span data-ttu-id="9efcb-169">Ответ</span><span class="sxs-lookup"><span data-stu-id="9efcb-169">Response</span></span>

<span data-ttu-id="9efcb-170">В случае успешной работы этот метод возвращает код ответа и временный `201 Created` [объектAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9efcb-170">If successful, this method returns a `201 Created` response code and a [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9efcb-171">Примеры</span><span class="sxs-lookup"><span data-stu-id="9efcb-171">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9efcb-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="9efcb-172">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="9efcb-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="9efcb-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_temporaryaccesspassauthenticationmethod_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/temporaryAccessPassMethods
Content-Type: application/json
Content-length: 209

{
  "@odata.type": "#microsoft.graph.temporaryAccessPassAuthenticationMethod",
  "startDateTime": "2021-01-26T00:00:00.000Z",
  "lifetimeInMinutes": 60,
  "isUsableOnce": false
}
```
# <a name="c"></a>[<span data-ttu-id="9efcb-174">C#</span><span class="sxs-lookup"><span data-stu-id="9efcb-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-temporaryaccesspassauthenticationmethod-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9efcb-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9efcb-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-temporaryaccesspassauthenticationmethod-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9efcb-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9efcb-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-temporaryaccesspassauthenticationmethod-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9efcb-177">Java</span><span class="sxs-lookup"><span data-stu-id="9efcb-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-temporaryaccesspassauthenticationmethod-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9efcb-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="9efcb-178">Response</span></span>
<span data-ttu-id="9efcb-179">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9efcb-179">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.temporaryAccessPassAuthenticationMethod"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.temporaryAccessPassAuthenticationMethod",
    "id": "81757535-e21e-4330-a338-33b8038ff12b",
    "temporaryAccessPass": "nc+&G=xwDKCz",
    "createdDateTime": "2021-01-25T23:53:35.5026721Z",
    "startDateTime": "2021-01-26T00:00:00Z",
    "lifetimeInMinutes": 60,
    "isUsableOnce": false,
    "isUsable": false,
    "methodUsabilityReason": "NotYetValid"

}
```
