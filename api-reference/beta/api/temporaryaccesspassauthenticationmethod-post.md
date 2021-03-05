---
title: Создание temporaryAccessPassAuthenticationMethod
description: Создание нового объекта temporaryAccessPassAuthenticationMethod.
author: inbarckMS
ms.author: inbarc
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 544911076be077740d77ec45faf76a315e96e805
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475113"
---
# <a name="create-temporaryaccesspassauthenticationmethod"></a><span data-ttu-id="a6afa-103">Создание temporaryAccessPassAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a6afa-103">Create temporaryAccessPassAuthenticationMethod</span></span>
<span data-ttu-id="a6afa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6afa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6afa-105">Создайте новый [объект temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) для пользователя.</span><span class="sxs-lookup"><span data-stu-id="a6afa-105">Create a new [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) object on a user.</span></span> <span data-ttu-id="a6afa-106">У пользователя может быть только один временный пропуск доступа.</span><span class="sxs-lookup"><span data-stu-id="a6afa-106">A user can only have one Temporary Access Pass.</span></span> <span data-ttu-id="a6afa-107">Пароль можно использовать между началом и конечным временем временного пропуска доступа.</span><span class="sxs-lookup"><span data-stu-id="a6afa-107">The passcode can be used between the start and end time of the Temporary Access Pass.</span></span> <span data-ttu-id="a6afa-108">Если пользователю требуется новый временный пропуск доступа:</span><span class="sxs-lookup"><span data-stu-id="a6afa-108">If the user requires a new Temporary Access Pass:</span></span>
* <span data-ttu-id="a6afa-109">Хотя текущий пропуск временного доступа действителен, администратору необходимо удалить существующий временный пропуск доступа и создать новый пропуск для пользователя.</span><span class="sxs-lookup"><span data-stu-id="a6afa-109">While the current Temporary Access Pass is valid – the admin needs to delete the existing Temporary Access Pass and create a new pass on the user.</span></span> <span data-ttu-id="a6afa-110">Удаление допустимой временной пропускной записи отзовет сеансы пользователя.</span><span class="sxs-lookup"><span data-stu-id="a6afa-110">Deleting a valid Temporary Access Pass will revoke the user’s sessions.</span></span> 
* <span data-ttu-id="a6afa-111">После истечения срока действия временного пропуска доступа новый временный пропуск переопределит текущий временный пропуск доступа и не отменит сеансы пользователя.</span><span class="sxs-lookup"><span data-stu-id="a6afa-111">After the Temporary Access Pass has expired – a new temporary access pass overrides the current temporary access pass and doesn't revoke the user’s sessions.</span></span>


## <a name="permissions"></a><span data-ttu-id="a6afa-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a6afa-112">Permissions</span></span>

<span data-ttu-id="a6afa-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6afa-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="a6afa-115">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="a6afa-115">Permissions acting on self</span></span>

|<span data-ttu-id="a6afa-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a6afa-116">Permission type</span></span>      | <span data-ttu-id="a6afa-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a6afa-117">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="a6afa-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a6afa-118">Delegated (work or school account)</span></span>     | <span data-ttu-id="a6afa-119">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a6afa-119">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="a6afa-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a6afa-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6afa-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6afa-121">Not supported.</span></span> |
| <span data-ttu-id="a6afa-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a6afa-122">Application</span></span>                            | <span data-ttu-id="a6afa-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6afa-123">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="a6afa-124">Разрешения, действующие на других пользователей</span><span class="sxs-lookup"><span data-stu-id="a6afa-124">Permissions acting on other users</span></span>

|<span data-ttu-id="a6afa-125">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a6afa-125">Permission type</span></span>      | <span data-ttu-id="a6afa-126">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a6afa-126">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="a6afa-127">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a6afa-127">Delegated (work or school account)</span></span>     | <span data-ttu-id="a6afa-128">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6afa-128">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="a6afa-129">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a6afa-129">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6afa-130">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6afa-130">Not supported.</span></span> |
| <span data-ttu-id="a6afa-131">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a6afa-131">Application</span></span>                            | <span data-ttu-id="a6afa-132">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6afa-132">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="a6afa-133">Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="a6afa-133">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="a6afa-134">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="a6afa-134">Global admin</span></span>
* <span data-ttu-id="a6afa-135">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="a6afa-135">Privileged authentication admin</span></span>
* <span data-ttu-id="a6afa-136">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="a6afa-136">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="a6afa-137">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a6afa-137">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{id | userPrincipalName}/authentication/temporaryAccessPassMethods
```

## <a name="request-headers"></a><span data-ttu-id="a6afa-138">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a6afa-138">Request headers</span></span>
|<span data-ttu-id="a6afa-139">Имя</span><span class="sxs-lookup"><span data-stu-id="a6afa-139">Name</span></span>|<span data-ttu-id="a6afa-140">Описание</span><span class="sxs-lookup"><span data-stu-id="a6afa-140">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a6afa-141">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a6afa-141">Authorization</span></span>|<span data-ttu-id="a6afa-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a6afa-p104">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a6afa-144">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a6afa-144">Content-Type</span></span>|<span data-ttu-id="a6afa-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a6afa-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6afa-147">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a6afa-147">Request body</span></span>
<span data-ttu-id="a6afa-148">В теле запроса поставляем представление JSON объекта [temporaryAccessPassAuthenticationMethod.](../resources/temporaryaccesspassauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="a6afa-148">In the request body, supply a JSON representation of the [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) object.</span></span>

<span data-ttu-id="a6afa-149">В следующей таблице описываются необязательные свойства, которые можно использовать при создании [временногоAccessPassAuthenticationMethod.](../resources/temporaryaccesspassauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="a6afa-149">The following table describes optional properties that can be used when creating the [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md).</span></span>

|<span data-ttu-id="a6afa-150">Свойство</span><span class="sxs-lookup"><span data-stu-id="a6afa-150">Property</span></span>|<span data-ttu-id="a6afa-151">Тип</span><span class="sxs-lookup"><span data-stu-id="a6afa-151">Type</span></span>|<span data-ttu-id="a6afa-152">Описание</span><span class="sxs-lookup"><span data-stu-id="a6afa-152">Description</span></span>|<span data-ttu-id="a6afa-153">Обязательный</span><span class="sxs-lookup"><span data-stu-id="a6afa-153">Required</span></span>| 
|:---|:---|:---|:---|
|<span data-ttu-id="a6afa-154">startDateTime</span><span class="sxs-lookup"><span data-stu-id="a6afa-154">startDateTime</span></span>|<span data-ttu-id="a6afa-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6afa-155">DateTimeOffset</span></span>|<span data-ttu-id="a6afa-156">Дата и время, когда временныйAccessPass станет доступным для использования, если не задать временный пропуск доступа, можно использовать во время создания.</span><span class="sxs-lookup"><span data-stu-id="a6afa-156">The date and time when the temporaryAccessPass becomes available to use, if not set the Temporary Access Pass is available to use at creation time.</span></span>| <span data-ttu-id="a6afa-157">Нет</span><span class="sxs-lookup"><span data-stu-id="a6afa-157">No</span></span>|
|<span data-ttu-id="a6afa-158">lifetimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="a6afa-158">lifetimeInMinutes</span></span>|<span data-ttu-id="a6afa-159">Int32</span><span class="sxs-lookup"><span data-stu-id="a6afa-159">Int32</span></span>|<span data-ttu-id="a6afa-160">Срок службы temporaryAccessPass в минутах, начиная с момента создания или при наборе startDateTime.</span><span class="sxs-lookup"><span data-stu-id="a6afa-160">The lifetime of the temporaryAccessPass in minutes starting at creation time or at startDateTime, if set.</span></span> <span data-ttu-id="a6afa-161">Минимум 10, максимум 43200 (эквивалент 30 дней).</span><span class="sxs-lookup"><span data-stu-id="a6afa-161">Minimum 10, Maximum 43200 (equivalent to 30 days).</span></span>| <span data-ttu-id="a6afa-162">Нет</span><span class="sxs-lookup"><span data-stu-id="a6afa-162">No</span></span>|
|<span data-ttu-id="a6afa-163">isUsableOnce</span><span class="sxs-lookup"><span data-stu-id="a6afa-163">isUsableOnce</span></span>|<span data-ttu-id="a6afa-164">Логический</span><span class="sxs-lookup"><span data-stu-id="a6afa-164">Boolean</span></span>|<span data-ttu-id="a6afa-165">Определяет, ограничен ли пропуск одно время использования.</span><span class="sxs-lookup"><span data-stu-id="a6afa-165">Determines if the pass is limited to a one time use.</span></span> <span data-ttu-id="a6afa-166">Если true — пропуск можно использовать один раз, если false — пропуск можно использовать несколько раз в течение временного времени службыAccessPass.</span><span class="sxs-lookup"><span data-stu-id="a6afa-166">If True – the pass can be used once, if False – the pass can be used multiple times within the temporaryAccessPass life time.</span></span> <span data-ttu-id="a6afa-167">Многоцелевой временный пропуск доступа (isUsableOnce = false) может быть создан и использован для регистрации, если это разрешено политикой метода проверки подлинности временного доступа.</span><span class="sxs-lookup"><span data-stu-id="a6afa-167">A multi-use Temporary Access Pass (isUsableOnce = false), can only be created and used for sign-in if it is allowed by the Temporary Access Pass Authentication method policy.</span></span>|  <span data-ttu-id="a6afa-168">Нет</span><span class="sxs-lookup"><span data-stu-id="a6afa-168">No</span></span>|



## <a name="response"></a><span data-ttu-id="a6afa-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6afa-169">Response</span></span>

<span data-ttu-id="a6afa-170">В случае успешной работы этот метод возвращает код ответа и временный `201 Created` [объектAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a6afa-170">If successful, this method returns a `201 Created` response code and a [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a6afa-171">Примеры</span><span class="sxs-lookup"><span data-stu-id="a6afa-171">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a6afa-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="a6afa-172">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a6afa-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="a6afa-173">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a6afa-174">C#</span><span class="sxs-lookup"><span data-stu-id="a6afa-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-temporaryaccesspassauthenticationmethod-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a6afa-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a6afa-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-temporaryaccesspassauthenticationmethod-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a6afa-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a6afa-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-temporaryaccesspassauthenticationmethod-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a6afa-177">Java</span><span class="sxs-lookup"><span data-stu-id="a6afa-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-temporaryaccesspassauthenticationmethod-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a6afa-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6afa-178">Response</span></span>
<span data-ttu-id="a6afa-179">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a6afa-179">**Note:** The response object shown here might be shortened for readability.</span></span>
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
