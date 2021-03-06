---
title: Создание temporaryAccessPassAuthenticationMethod
description: Создание нового объекта temporaryAccessPassAuthenticationMethod.
author: inbarckMS
ms.author: inbarc
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fcd0c019e90d326d7b76617e1121fc721b2fe196
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515942"
---
# <a name="create-temporaryaccesspassauthenticationmethod"></a><span data-ttu-id="b23e0-103">Создание temporaryAccessPassAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b23e0-103">Create temporaryAccessPassAuthenticationMethod</span></span>
<span data-ttu-id="b23e0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b23e0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b23e0-105">Создайте новый [объект temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) для пользователя.</span><span class="sxs-lookup"><span data-stu-id="b23e0-105">Create a new [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) object on a user.</span></span> <span data-ttu-id="b23e0-106">У пользователя может быть только один временный пропуск доступа.</span><span class="sxs-lookup"><span data-stu-id="b23e0-106">A user can only have one Temporary Access Pass.</span></span> <span data-ttu-id="b23e0-107">Пароль можно использовать между началом и конечным временем временного пропуска доступа.</span><span class="sxs-lookup"><span data-stu-id="b23e0-107">The passcode can be used between the start and end time of the Temporary Access Pass.</span></span> <span data-ttu-id="b23e0-108">Если пользователю требуется новый временный пропуск доступа:</span><span class="sxs-lookup"><span data-stu-id="b23e0-108">If the user requires a new Temporary Access Pass:</span></span>
* <span data-ttu-id="b23e0-109">Хотя текущий пропуск временного доступа действителен, администратору необходимо удалить существующий временный пропуск доступа и создать новый пропуск для пользователя.</span><span class="sxs-lookup"><span data-stu-id="b23e0-109">While the current Temporary Access Pass is valid – the admin needs to delete the existing Temporary Access Pass and create a new pass on the user.</span></span> <span data-ttu-id="b23e0-110">Удаление допустимой временной пропускной записи отзовет сеансы пользователя.</span><span class="sxs-lookup"><span data-stu-id="b23e0-110">Deleting a valid Temporary Access Pass will revoke the user’s sessions.</span></span> 
* <span data-ttu-id="b23e0-111">После истечения срока действия временного пропуска доступа новый временный пропуск переопределит текущий временный пропуск доступа и не отменит сеансы пользователя.</span><span class="sxs-lookup"><span data-stu-id="b23e0-111">After the Temporary Access Pass has expired – a new temporary access pass overrides the current temporary access pass and doesn't revoke the user’s sessions.</span></span>


## <a name="permissions"></a><span data-ttu-id="b23e0-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b23e0-112">Permissions</span></span>

<span data-ttu-id="b23e0-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b23e0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="b23e0-115">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="b23e0-115">Permissions acting on self</span></span>

|<span data-ttu-id="b23e0-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b23e0-116">Permission type</span></span>      | <span data-ttu-id="b23e0-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b23e0-117">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="b23e0-118">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b23e0-118">Delegated (work or school account)</span></span>     | <span data-ttu-id="b23e0-119">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b23e0-119">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="b23e0-120">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b23e0-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b23e0-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b23e0-121">Not supported.</span></span> |
| <span data-ttu-id="b23e0-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b23e0-122">Application</span></span>                            | <span data-ttu-id="b23e0-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b23e0-123">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="b23e0-124">Разрешения, действующие на других пользователей</span><span class="sxs-lookup"><span data-stu-id="b23e0-124">Permissions acting on other users</span></span>

|<span data-ttu-id="b23e0-125">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b23e0-125">Permission type</span></span>      | <span data-ttu-id="b23e0-126">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b23e0-126">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="b23e0-127">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b23e0-127">Delegated (work or school account)</span></span>     | <span data-ttu-id="b23e0-128">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b23e0-128">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="b23e0-129">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b23e0-129">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b23e0-130">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b23e0-130">Not supported.</span></span> |
| <span data-ttu-id="b23e0-131">Приложение</span><span class="sxs-lookup"><span data-stu-id="b23e0-131">Application</span></span>                            | <span data-ttu-id="b23e0-132">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b23e0-132">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="b23e0-133">Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="b23e0-133">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="b23e0-134">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="b23e0-134">Global admin</span></span>
* <span data-ttu-id="b23e0-135">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="b23e0-135">Privileged authentication admin</span></span>
* <span data-ttu-id="b23e0-136">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="b23e0-136">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="b23e0-137">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b23e0-137">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{id | userPrincipalName}/authentication/temporaryAccessPassMethods
```

## <a name="request-headers"></a><span data-ttu-id="b23e0-138">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b23e0-138">Request headers</span></span>
|<span data-ttu-id="b23e0-139">Имя</span><span class="sxs-lookup"><span data-stu-id="b23e0-139">Name</span></span>|<span data-ttu-id="b23e0-140">Описание</span><span class="sxs-lookup"><span data-stu-id="b23e0-140">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b23e0-141">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b23e0-141">Authorization</span></span>|<span data-ttu-id="b23e0-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b23e0-p104">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b23e0-144">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b23e0-144">Content-Type</span></span>|<span data-ttu-id="b23e0-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b23e0-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b23e0-147">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b23e0-147">Request body</span></span>
<span data-ttu-id="b23e0-148">В теле запроса поставляем представление JSON объекта [temporaryAccessPassAuthenticationMethod.](../resources/temporaryaccesspassauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="b23e0-148">In the request body, supply a JSON representation of the [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) object.</span></span>

<span data-ttu-id="b23e0-149">В следующей таблице описываются необязательные свойства, которые можно использовать при создании [временногоAccessPassAuthenticationMethod.](../resources/temporaryaccesspassauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="b23e0-149">The following table describes optional properties that can be used when creating the [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md).</span></span>

|<span data-ttu-id="b23e0-150">Свойство</span><span class="sxs-lookup"><span data-stu-id="b23e0-150">Property</span></span>|<span data-ttu-id="b23e0-151">Тип</span><span class="sxs-lookup"><span data-stu-id="b23e0-151">Type</span></span>|<span data-ttu-id="b23e0-152">Описание</span><span class="sxs-lookup"><span data-stu-id="b23e0-152">Description</span></span>|<span data-ttu-id="b23e0-153">Обязательный</span><span class="sxs-lookup"><span data-stu-id="b23e0-153">Required</span></span>| 
|:---|:---|:---|:---|
|<span data-ttu-id="b23e0-154">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b23e0-154">startDateTime</span></span>|<span data-ttu-id="b23e0-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b23e0-155">DateTimeOffset</span></span>|<span data-ttu-id="b23e0-156">Дата и время, когда временныйAccessPass станет доступным для использования, если не задать временный пропуск доступа, можно использовать во время создания.</span><span class="sxs-lookup"><span data-stu-id="b23e0-156">The date and time when the temporaryAccessPass becomes available to use, if not set the Temporary Access Pass is available to use at creation time.</span></span>| <span data-ttu-id="b23e0-157">Нет</span><span class="sxs-lookup"><span data-stu-id="b23e0-157">No</span></span>|
|<span data-ttu-id="b23e0-158">lifetimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="b23e0-158">lifetimeInMinutes</span></span>|<span data-ttu-id="b23e0-159">Int32</span><span class="sxs-lookup"><span data-stu-id="b23e0-159">Int32</span></span>|<span data-ttu-id="b23e0-160">Срок службы temporaryAccessPass в минутах, начиная с момента создания или при наборе startDateTime.</span><span class="sxs-lookup"><span data-stu-id="b23e0-160">The lifetime of the temporaryAccessPass in minutes starting at creation time or at startDateTime, if set.</span></span> <span data-ttu-id="b23e0-161">Минимум 10, максимум 43200 (эквивалент 30 дней).</span><span class="sxs-lookup"><span data-stu-id="b23e0-161">Minimum 10, Maximum 43200 (equivalent to 30 days).</span></span>| <span data-ttu-id="b23e0-162">Нет</span><span class="sxs-lookup"><span data-stu-id="b23e0-162">No</span></span>|
|<span data-ttu-id="b23e0-163">isUsableOnce</span><span class="sxs-lookup"><span data-stu-id="b23e0-163">isUsableOnce</span></span>|<span data-ttu-id="b23e0-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="b23e0-164">Boolean</span></span>|<span data-ttu-id="b23e0-165">Определяет, ограничен ли пропуск одно время использования.</span><span class="sxs-lookup"><span data-stu-id="b23e0-165">Determines if the pass is limited to a one time use.</span></span> <span data-ttu-id="b23e0-166">Если true — пропуск можно использовать один раз, если false — пропуск можно использовать несколько раз в течение временного времени службыAccessPass.</span><span class="sxs-lookup"><span data-stu-id="b23e0-166">If True – the pass can be used once, if False – the pass can be used multiple times within the temporaryAccessPass life time.</span></span> <span data-ttu-id="b23e0-167">Многоцелевой временный пропуск доступа (isUsableOnce = false) может быть создан и использован для регистрации, если это разрешено политикой метода проверки подлинности временного доступа.</span><span class="sxs-lookup"><span data-stu-id="b23e0-167">A multi-use Temporary Access Pass (isUsableOnce = false), can only be created and used for sign-in if it is allowed by the Temporary Access Pass Authentication method policy.</span></span>|  <span data-ttu-id="b23e0-168">Нет</span><span class="sxs-lookup"><span data-stu-id="b23e0-168">No</span></span>|



## <a name="response"></a><span data-ttu-id="b23e0-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="b23e0-169">Response</span></span>

<span data-ttu-id="b23e0-170">В случае успешной работы этот метод возвращает код ответа и временный `201 Created` [объектAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b23e0-170">If successful, this method returns a `201 Created` response code and a [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b23e0-171">Примеры</span><span class="sxs-lookup"><span data-stu-id="b23e0-171">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b23e0-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="b23e0-172">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b23e0-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="b23e0-173">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b23e0-174">C#</span><span class="sxs-lookup"><span data-stu-id="b23e0-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-temporaryaccesspassauthenticationmethod-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b23e0-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b23e0-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-temporaryaccesspassauthenticationmethod-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b23e0-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b23e0-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-temporaryaccesspassauthenticationmethod-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b23e0-177">Java</span><span class="sxs-lookup"><span data-stu-id="b23e0-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-temporaryaccesspassauthenticationmethod-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b23e0-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="b23e0-178">Response</span></span>
<span data-ttu-id="b23e0-179">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b23e0-179">**Note:** The response object shown here might be shortened for readability.</span></span>
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
