---
title: Удаление Усераккаунтинформатион
description: Удаление объекта Усераккаунтинформатион.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 583184860730adbd64899bdc5091c40534677529
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43228368"
---
# <a name="delete-useraccountinformation"></a><span data-ttu-id="6c138-103">Удаление Усераккаунтинформатион</span><span class="sxs-lookup"><span data-stu-id="6c138-103">Delete userAccountInformation</span></span>

<span data-ttu-id="6c138-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c138-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c138-105">Удаление объекта [усераккаунтинформатион](../resources/useraccountinformation.md) из [профиля](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="6c138-105">Delete a [userAccountInformation](../resources/useraccountinformation.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6c138-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6c138-106">Permissions</span></span>

<span data-ttu-id="6c138-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c138-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6c138-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6c138-109">Permission type</span></span>                        | <span data-ttu-id="6c138-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6c138-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6c138-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6c138-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6c138-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c138-112">Not supported.</span></span>                              |
| <span data-ttu-id="6c138-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6c138-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c138-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c138-114">Not supported.</span></span>                              |
| <span data-ttu-id="6c138-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6c138-115">Application</span></span>                            | <span data-ttu-id="6c138-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c138-116">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="6c138-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6c138-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /user/profile/account{id}
```

## <a name="request-headers"></a><span data-ttu-id="6c138-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6c138-118">Request headers</span></span>

| <span data-ttu-id="6c138-119">Имя</span><span class="sxs-lookup"><span data-stu-id="6c138-119">Name</span></span>           | <span data-ttu-id="6c138-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6c138-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="6c138-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6c138-121">Authorization</span></span>  | <span data-ttu-id="6c138-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6c138-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6c138-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6c138-124">Request body</span></span>

<span data-ttu-id="6c138-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6c138-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c138-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c138-126">Response</span></span>

<span data-ttu-id="6c138-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6c138-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6c138-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="6c138-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6c138-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="6c138-130">Request</span></span>

<span data-ttu-id="6c138-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6c138-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_useraccountinformation"
}-->

```http
DELETE https://graph.microsoft.com/beta/user/profile/account/{id}
```

### <a name="response"></a><span data-ttu-id="6c138-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c138-132">Response</span></span>

<span data-ttu-id="6c138-133">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6c138-133">The following is an example of the response.</span></span>

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
  "description": "Delete userAccountInformation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
