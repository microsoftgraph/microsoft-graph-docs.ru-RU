---
title: Удаление Усераккаунтинформатион
description: Удаление объекта Усераккаунтинформатион.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: b7df1498260be758fd7c945fe013b09d09e1aed0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050299"
---
# <a name="delete-useraccountinformation"></a><span data-ttu-id="505fc-103">Удаление Усераккаунтинформатион</span><span class="sxs-lookup"><span data-stu-id="505fc-103">Delete userAccountInformation</span></span>

<span data-ttu-id="505fc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="505fc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="505fc-105">Удаление объекта [усераккаунтинформатион](../resources/useraccountinformation.md) из [профиля](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="505fc-105">Delete an [userAccountInformation](../resources/useraccountinformation.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="505fc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="505fc-106">Permissions</span></span>

<span data-ttu-id="505fc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="505fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="505fc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="505fc-109">Permission type</span></span>                        | <span data-ttu-id="505fc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="505fc-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="505fc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="505fc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="505fc-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="505fc-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="505fc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="505fc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="505fc-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="505fc-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="505fc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="505fc-115">Application</span></span>                            | <span data-ttu-id="505fc-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="505fc-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="505fc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="505fc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/accounts/{id}
DELETE /users/{id | userPrincipalName}/profile/accounts/{id}
```

## <a name="request-headers"></a><span data-ttu-id="505fc-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="505fc-118">Request headers</span></span>

| <span data-ttu-id="505fc-119">Имя</span><span class="sxs-lookup"><span data-stu-id="505fc-119">Name</span></span>           | <span data-ttu-id="505fc-120">Описание</span><span class="sxs-lookup"><span data-stu-id="505fc-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="505fc-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="505fc-121">Authorization</span></span>  | <span data-ttu-id="505fc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="505fc-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="505fc-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="505fc-124">Request body</span></span>

<span data-ttu-id="505fc-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="505fc-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="505fc-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="505fc-126">Response</span></span>

<span data-ttu-id="505fc-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="505fc-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="505fc-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="505fc-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="505fc-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="505fc-130">Request</span></span>

<span data-ttu-id="505fc-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="505fc-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_useraccountinformation"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/accounts/{id}
```

### <a name="response"></a><span data-ttu-id="505fc-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="505fc-132">Response</span></span>

<span data-ttu-id="505fc-133">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="505fc-133">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

