---
title: Удаление Фонеаусентикатионмесод
description: Удаление метода проверки подлинности телефона пользователя.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 05e6b50b04b0b527ad7b37bcadb5405c0e896fe0
ms.sourcegitcommit: 9c16d84eac9c34134864ad63a9bb95c309218a44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/18/2020
ms.locfileid: "43557817"
---
# <a name="delete-phoneauthenticationmethod"></a><span data-ttu-id="490af-103">Удаление Фонеаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="490af-103">Delete phoneAuthenticationMethod</span></span>

<span data-ttu-id="490af-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="490af-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="490af-105">Удаление [метода проверки подлинности телефона](../resources/phoneauthenticationmethod.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="490af-105">Delete a user's [phone authentication method](../resources/phoneauthenticationmethod.md).</span></span> 

><span data-ttu-id="490af-106">**Примечание:** При этом номер телефона будет удален от пользователя, и он больше не сможет использовать проверку подлинности с помощью SMS или голосовых вызовов.</span><span class="sxs-lookup"><span data-stu-id="490af-106">**Note:** This removes the phone number from the user and they will no longer be able to use the number for authentication, whether via SMS or voice calls.</span></span>

<span data-ttu-id="490af-107">Помните, что у пользователя не может `alternateMobile` быть номера без `mobile` номера.</span><span class="sxs-lookup"><span data-stu-id="490af-107">Remember that a user cannot have an `alternateMobile` number without a `mobile` number.</span></span> <span data-ttu-id="490af-108">`mobile` Если вы хотите удалить номер из пользователя, который также имеет `alternateMobile` номер, сначала [Обновите](phoneauthenticationmethod-update.md) его `mobile` до нового номера, а затем удалите `alternateMobile` номер.</span><span class="sxs-lookup"><span data-stu-id="490af-108">If you want to remove a `mobile` number from a user that also has an `alternateMobile` number, first [update](phoneauthenticationmethod-update.md) the `mobile` number to the new number, then delete the `alternateMobile` number.</span></span>

<span data-ttu-id="490af-109">Если номер телефона является методом проверки подлинности с многофакторной проверкой подлинности (MFA) Azure по умолчанию, он не может быть удален.</span><span class="sxs-lookup"><span data-stu-id="490af-109">If the phone number is the user's default Azure multi-factor authentication (MFA) authentication method, it cannot be deleted.</span></span> <span data-ttu-id="490af-110">Попросите пользователя изменить метод проверки подлинности по умолчанию, а затем удалить этот номер.</span><span class="sxs-lookup"><span data-stu-id="490af-110">Have the user change their default authentication method, and then delete the number.</span></span>

## <a name="permissions"></a><span data-ttu-id="490af-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="490af-111">Permissions</span></span>

<span data-ttu-id="490af-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="490af-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="490af-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="490af-114">Permission type</span></span>                        | <span data-ttu-id="490af-115">Разрешения, действующие на себя (по крайней мере для самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="490af-115">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="490af-116">Разрешения, действующие на других (по крайней мере для самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="490af-116">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="490af-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="490af-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="490af-118">Усераусентикатионмесод. ReadWrite, Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="490af-118">UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span> | <span data-ttu-id="490af-119">Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="490af-119">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="490af-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="490af-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="490af-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="490af-121">Not supported.</span></span> | <span data-ttu-id="490af-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="490af-122">Not supported.</span></span> |
| <span data-ttu-id="490af-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="490af-123">Application</span></span>                            | <span data-ttu-id="490af-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="490af-124">Not supported.</span></span> | <span data-ttu-id="490af-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="490af-125">Not supported.</span></span> |

<span data-ttu-id="490af-126">Для делегированных сценариев, в которых администратор работает с другим пользователем, администратору необходима [одна из следующих ролей](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="490af-126">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="490af-127">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="490af-127">Global admin</span></span>
* <span data-ttu-id="490af-128">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="490af-128">Privileged authentication admin</span></span>
* <span data-ttu-id="490af-129">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="490af-129">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="490af-130">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="490af-130">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/authentication/phoneMethods/{id}
DELETE /users/{id}/authentication/phoneMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="490af-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="490af-131">Request headers</span></span>

| <span data-ttu-id="490af-132">Имя</span><span class="sxs-lookup"><span data-stu-id="490af-132">Name</span></span>          | <span data-ttu-id="490af-133">Описание</span><span class="sxs-lookup"><span data-stu-id="490af-133">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="490af-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="490af-134">Authorization</span></span> | <span data-ttu-id="490af-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="490af-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="490af-137">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="490af-137">Request body</span></span>

<span data-ttu-id="490af-138">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="490af-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="490af-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="490af-139">Response</span></span>

<span data-ttu-id="490af-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="490af-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="490af-142">Примеры</span><span class="sxs-lookup"><span data-stu-id="490af-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="490af-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="490af-143">Request</span></span>

<span data-ttu-id="490af-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="490af-144">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_phoneauthenticationmethod"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7
```

### <a name="response"></a><span data-ttu-id="490af-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="490af-145">Response</span></span>

<span data-ttu-id="490af-146">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="490af-146">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete phoneAuthenticationMethod",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
