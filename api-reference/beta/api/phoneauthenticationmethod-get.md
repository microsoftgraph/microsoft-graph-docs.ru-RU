---
title: Получение Фонеаусентикатионмесод
description: Получение одного объекта Фонеаусентикатионмесод.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0eee3702c31c5237d8b1f322018dcc60bc63762c
ms.sourcegitcommit: 9c16d84eac9c34134864ad63a9bb95c309218a44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/18/2020
ms.locfileid: "43557801"
---
# <a name="get-phoneauthenticationmethod"></a><span data-ttu-id="2b931-103">Получение Фонеаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="2b931-103">Get phoneAuthenticationMethod</span></span>

<span data-ttu-id="2b931-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b931-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b931-105">Получение одного объекта [фонеаусентикатионмесод](../resources/phoneauthenticationmethod.md) .</span><span class="sxs-lookup"><span data-stu-id="2b931-105">Retrieve a single [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2b931-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2b931-106">Permissions</span></span>

<span data-ttu-id="2b931-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b931-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2b931-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b931-109">Permission type</span></span>                        | <span data-ttu-id="2b931-110">Разрешения, действующие на себя (по крайней мере для самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="2b931-110">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="2b931-111">Разрешения, действующие на других (по крайней мере для самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="2b931-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="2b931-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b931-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="2b931-113">Усераусентикатионмесод. Read, Усераусентикатионмесод. Read. ALL, Усераусентикатионмесод. ReadWrite, Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="2b931-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span> | <span data-ttu-id="2b931-114">Усераусентикатионмесод. Read. ALL, Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="2b931-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="2b931-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b931-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b931-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b931-116">Not supported.</span></span> | <span data-ttu-id="2b931-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b931-117">Not supported.</span></span> |
| <span data-ttu-id="2b931-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2b931-118">Application</span></span>                            | <span data-ttu-id="2b931-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b931-119">Not supported.</span></span> | <span data-ttu-id="2b931-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b931-120">Not supported.</span></span> |

<span data-ttu-id="2b931-121">Для делегированных сценариев, в которых администратор работает с другим пользователем, администратору необходима [одна из следующих ролей](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="2b931-121">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="2b931-122">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="2b931-122">Global admin</span></span>
* <span data-ttu-id="2b931-123">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="2b931-123">Global reader</span></span>
* <span data-ttu-id="2b931-124">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="2b931-124">Privileged authentication admin</span></span>
* <span data-ttu-id="2b931-125">Администратор проверки подлинности (видит только скрытые номера телефонов)</span><span class="sxs-lookup"><span data-stu-id="2b931-125">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="2b931-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b931-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/phoneMethods/{id}
GET /users/{id}/authentication/phoneMethods/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2b931-127">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2b931-127">Optional query parameters</span></span>

<span data-ttu-id="2b931-128">Этот метод не поддерживает дополнительные параметры запроса для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="2b931-128">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2b931-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2b931-129">Request headers</span></span>

| <span data-ttu-id="2b931-130">Имя</span><span class="sxs-lookup"><span data-stu-id="2b931-130">Name</span></span>      |<span data-ttu-id="2b931-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2b931-131">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2b931-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2b931-132">Authorization</span></span> | <span data-ttu-id="2b931-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2b931-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2b931-135">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2b931-135">Request body</span></span>

<span data-ttu-id="2b931-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2b931-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b931-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="2b931-137">Response</span></span>

<span data-ttu-id="2b931-138">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [фонеаусентикатионмесод](../resources/phoneauthenticationmethod.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2b931-138">If successful, this method returns a `200 OK` response code and the requested [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2b931-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="2b931-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2b931-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b931-140">Request</span></span>

<span data-ttu-id="2b931-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b931-141">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_phoneauthenticationmethod"
}-->

```http
GET https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7
```

### <a name="response"></a><span data-ttu-id="2b931-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b931-142">Response</span></span>

<span data-ttu-id="2b931-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2b931-143">The following is an example of the response.</span></span>

> <span data-ttu-id="2b931-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2b931-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.phoneAuthenticationMethod"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "phoneNumber": "+1 2065555555",
  "phoneType": "mobile",
  "smsSignInState": "ready",
  "id": "3179e48a-750b-4051-897c-87b9720928f7"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get phoneAuthenticationMethod",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
