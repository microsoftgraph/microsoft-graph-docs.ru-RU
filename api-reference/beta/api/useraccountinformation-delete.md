---
title: Удаление userAccountInformation
description: Удаление объекта userAccountInformation.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 30e9a3e098a26e4e490a5f1c1799eca2124edd73
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/18/2021
ms.locfileid: "50291967"
---
# <a name="delete-useraccountinformation"></a><span data-ttu-id="e43d8-103">Удаление userAccountInformation</span><span class="sxs-lookup"><span data-stu-id="e43d8-103">Delete userAccountInformation</span></span>

<span data-ttu-id="e43d8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e43d8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e43d8-105">Удаление объекта [userAccountInformation](../resources/useraccountinformation.md) из профиля [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="e43d8-105">Delete an [userAccountInformation](../resources/useraccountinformation.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e43d8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e43d8-106">Permissions</span></span>

<span data-ttu-id="e43d8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e43d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e43d8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e43d8-109">Permission type</span></span>                        | <span data-ttu-id="e43d8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e43d8-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e43d8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e43d8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e43d8-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e43d8-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="e43d8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e43d8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e43d8-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e43d8-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="e43d8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e43d8-115">Application</span></span>                            | <span data-ttu-id="e43d8-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e43d8-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="e43d8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e43d8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/account/{id}
DELETE /users/{id | userPrincipalName}/profile/account/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e43d8-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e43d8-118">Request headers</span></span>

| <span data-ttu-id="e43d8-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e43d8-119">Name</span></span>           | <span data-ttu-id="e43d8-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e43d8-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="e43d8-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e43d8-121">Authorization</span></span>  | <span data-ttu-id="e43d8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e43d8-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e43d8-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e43d8-124">Request body</span></span>

<span data-ttu-id="e43d8-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e43d8-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e43d8-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="e43d8-126">Response</span></span>

<span data-ttu-id="e43d8-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e43d8-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e43d8-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="e43d8-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e43d8-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="e43d8-130">Request</span></span>

<span data-ttu-id="e43d8-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e43d8-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_useraccountinformation"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/account/{id}
```

### <a name="response"></a><span data-ttu-id="e43d8-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="e43d8-132">Response</span></span>

<span data-ttu-id="e43d8-133">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e43d8-133">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

