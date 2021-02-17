---
title: Создание temporaryAccessPassAuthenticationMethod
description: Создание объекта temporaryAccessPassAuthenticationMethod.
author: inbarckMS
ms.author: inbarc
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d048d843c0a93dc779a0966d6a27d337251fc974
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272687"
---
# <a name="create-temporaryaccesspassauthenticationmethod"></a><span data-ttu-id="1aa26-103">Создание temporaryAccessPassAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="1aa26-103">Create temporaryAccessPassAuthenticationMethod</span></span>
<span data-ttu-id="1aa26-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1aa26-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1aa26-105">Создайте новый [временный объектAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) для пользователя.</span><span class="sxs-lookup"><span data-stu-id="1aa26-105">Create a new [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) object on a user.</span></span> <span data-ttu-id="1aa26-106">У пользователя может быть только один временный проход доступа.</span><span class="sxs-lookup"><span data-stu-id="1aa26-106">A user can only have one Temporary Access Pass.</span></span> <span data-ttu-id="1aa26-107">Пароль можно использовать между началом и временем окончания временного прохода доступа.</span><span class="sxs-lookup"><span data-stu-id="1aa26-107">The passcode can be used between the start and end time of the Temporary Access Pass.</span></span> <span data-ttu-id="1aa26-108">Если пользователю требуется новый временный проход доступа:</span><span class="sxs-lookup"><span data-stu-id="1aa26-108">If the user requires a new Temporary Access Pass:</span></span>
* <span data-ttu-id="1aa26-109">Несмотря на то что текущий временный проход доступа действителен, администратору необходимо удалить существующий временный проход доступа и создать новый проход для пользователя.</span><span class="sxs-lookup"><span data-stu-id="1aa26-109">While the current Temporary Access Pass is valid – the admin needs to delete the existing Temporary Access Pass and create a new pass on the user.</span></span> <span data-ttu-id="1aa26-110">При удалении действительного временного прохода сеансы пользователя будут отоскины.</span><span class="sxs-lookup"><span data-stu-id="1aa26-110">Deleting a valid Temporary Access Pass will revoke the user’s sessions.</span></span> 
* <span data-ttu-id="1aa26-111">По истечении срока действия временного доступа новый временный проход доступа переопределяет текущий временный проход доступа и не отменяет сеансы пользователя.</span><span class="sxs-lookup"><span data-stu-id="1aa26-111">After the Temporary Access Pass has expired – a new temporary access pass overrides the current temporary access pass and doesn't revoke the user’s sessions.</span></span>


## <a name="permissions"></a><span data-ttu-id="1aa26-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1aa26-112">Permissions</span></span>

<span data-ttu-id="1aa26-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1aa26-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="1aa26-115">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="1aa26-115">Permissions acting on self</span></span>

|<span data-ttu-id="1aa26-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1aa26-116">Permission type</span></span>      | <span data-ttu-id="1aa26-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1aa26-117">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="1aa26-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1aa26-118">Delegated (work or school account)</span></span>     | <span data-ttu-id="1aa26-119">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1aa26-119">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="1aa26-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1aa26-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1aa26-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1aa26-121">Not supported.</span></span> |
| <span data-ttu-id="1aa26-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1aa26-122">Application</span></span>                            | <span data-ttu-id="1aa26-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1aa26-123">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="1aa26-124">Разрешения, действующие с другими пользователями</span><span class="sxs-lookup"><span data-stu-id="1aa26-124">Permissions acting on other users</span></span>

|<span data-ttu-id="1aa26-125">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1aa26-125">Permission type</span></span>      | <span data-ttu-id="1aa26-126">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1aa26-126">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="1aa26-127">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1aa26-127">Delegated (work or school account)</span></span>     | <span data-ttu-id="1aa26-128">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1aa26-128">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="1aa26-129">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1aa26-129">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1aa26-130">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1aa26-130">Not supported.</span></span> |
| <span data-ttu-id="1aa26-131">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1aa26-131">Application</span></span>                            | <span data-ttu-id="1aa26-132">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1aa26-132">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="1aa26-133">Для делегирования сценариев, в которых администратор действует над другим пользователем, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="1aa26-133">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="1aa26-134">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="1aa26-134">Global admin</span></span>
* <span data-ttu-id="1aa26-135">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="1aa26-135">Privileged authentication admin</span></span>
* <span data-ttu-id="1aa26-136">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="1aa26-136">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="1aa26-137">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1aa26-137">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{id | userPrincipalName}/authentication/temporaryAccessPassMethods
```

## <a name="request-headers"></a><span data-ttu-id="1aa26-138">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1aa26-138">Request headers</span></span>
|<span data-ttu-id="1aa26-139">Имя</span><span class="sxs-lookup"><span data-stu-id="1aa26-139">Name</span></span>|<span data-ttu-id="1aa26-140">Описание</span><span class="sxs-lookup"><span data-stu-id="1aa26-140">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1aa26-141">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1aa26-141">Authorization</span></span>|<span data-ttu-id="1aa26-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1aa26-p104">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="1aa26-144">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1aa26-144">Content-Type</span></span>|<span data-ttu-id="1aa26-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1aa26-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1aa26-147">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1aa26-147">Request body</span></span>
<span data-ttu-id="1aa26-148">В теле запроса укажу представление объекта [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="1aa26-148">In the request body, supply a JSON representation of the [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) object.</span></span>

<span data-ttu-id="1aa26-149">В следующей таблице описываются необязательные свойства, которые можно использовать при создании [временного объектаAccessPassAuthenticationMethod.](../resources/temporaryaccesspassauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="1aa26-149">The following table describes optional properties that can be used when creating the [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md).</span></span>

|<span data-ttu-id="1aa26-150">Свойство</span><span class="sxs-lookup"><span data-stu-id="1aa26-150">Property</span></span>|<span data-ttu-id="1aa26-151">Тип</span><span class="sxs-lookup"><span data-stu-id="1aa26-151">Type</span></span>|<span data-ttu-id="1aa26-152">Описание</span><span class="sxs-lookup"><span data-stu-id="1aa26-152">Description</span></span>|<span data-ttu-id="1aa26-153">Обязательный</span><span class="sxs-lookup"><span data-stu-id="1aa26-153">Required</span></span>| 
|:---|:---|:---|:---|
|<span data-ttu-id="1aa26-154">startDateTime</span><span class="sxs-lookup"><span data-stu-id="1aa26-154">startDateTime</span></span>|<span data-ttu-id="1aa26-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1aa26-155">DateTimeOffset</span></span>|<span data-ttu-id="1aa26-156">Дата и время, когда временныйaccessPass становится доступным для использования, если не задав временный проход доступа, доступен для использования во время создания.</span><span class="sxs-lookup"><span data-stu-id="1aa26-156">The date and time when the temporaryAccessPass becomes available to use, if not set the Temporary Access Pass is available to use at creation time.</span></span>| <span data-ttu-id="1aa26-157">Нет</span><span class="sxs-lookup"><span data-stu-id="1aa26-157">No</span></span>|
|<span data-ttu-id="1aa26-158">lifetimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="1aa26-158">lifetimeInMinutes</span></span>|<span data-ttu-id="1aa26-159">Int32</span><span class="sxs-lookup"><span data-stu-id="1aa26-159">Int32</span></span>|<span data-ttu-id="1aa26-160">Время существования temporaryAccessPass в минутах, начиная с момента создания или в startDateTime, если установлено.</span><span class="sxs-lookup"><span data-stu-id="1aa26-160">The lifetime of the temporaryAccessPass in minutes starting at creation time or at startDateTime, if set.</span></span> <span data-ttu-id="1aa26-161">Минимум 10, максимум 43200 (эквивалентно 30 дням).</span><span class="sxs-lookup"><span data-stu-id="1aa26-161">Minimum 10, Maximum 43200 (equivalent to 30 days).</span></span>| <span data-ttu-id="1aa26-162">Нет</span><span class="sxs-lookup"><span data-stu-id="1aa26-162">No</span></span>|
|<span data-ttu-id="1aa26-163">isUsableOnce</span><span class="sxs-lookup"><span data-stu-id="1aa26-163">isUsableOnce</span></span>|<span data-ttu-id="1aa26-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="1aa26-164">Boolean</span></span>|<span data-ttu-id="1aa26-165">Определяет, ограничен ли проход одновейным использованием.</span><span class="sxs-lookup"><span data-stu-id="1aa26-165">Determines if the pass is limited to a one time use.</span></span> <span data-ttu-id="1aa26-166">Если имеет значение True, то проход можно использовать один раз, если задав значение False, этот проход можно использовать несколько раз в течение жизненного времени temporaryAccessPass.</span><span class="sxs-lookup"><span data-stu-id="1aa26-166">If True – the pass can be used once, if False – the pass can be used multiple times within the temporaryAccessPass life time.</span></span> <span data-ttu-id="1aa26-167">A multi-use Temporary Access Pass (isUsableOnce = false), can only be created and used for sign-in if it is allowed by the Temporary Access Pass Authentication method policy.</span><span class="sxs-lookup"><span data-stu-id="1aa26-167">A multi-use Temporary Access Pass (isUsableOnce = false), can only be created and used for sign-in if it is allowed by the Temporary Access Pass Authentication method policy.</span></span>|  <span data-ttu-id="1aa26-168">Нет</span><span class="sxs-lookup"><span data-stu-id="1aa26-168">No</span></span>|



## <a name="response"></a><span data-ttu-id="1aa26-169">Ответ</span><span class="sxs-lookup"><span data-stu-id="1aa26-169">Response</span></span>

<span data-ttu-id="1aa26-170">В случае успеха этот метод возвращает код отклика и временный `201 Created` [объектAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1aa26-170">If successful, this method returns a `201 Created` response code and a [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1aa26-171">Примеры</span><span class="sxs-lookup"><span data-stu-id="1aa26-171">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1aa26-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="1aa26-172">Request</span></span>
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

### <a name="response"></a><span data-ttu-id="1aa26-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="1aa26-173">Response</span></span>
<span data-ttu-id="1aa26-174">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1aa26-174">**Note:** The response object shown here might be shortened for readability.</span></span>
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