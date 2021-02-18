---
title: Удаление personResponsibility
description: Удаляет объект personResponsibility.
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 17ce90f05b52cb05c3030ceff0fb3312f71466ef
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292723"
---
# <a name="delete-personresponsibility"></a><span data-ttu-id="1c21e-103">Удаление personResponsibility</span><span class="sxs-lookup"><span data-stu-id="1c21e-103">Delete personResponsibility</span></span>
<span data-ttu-id="1c21e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c21e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1c21e-105">Удаляет объект [personResponsibility](../resources/personresponsibility.md) из профиля [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="1c21e-105">Deletes a [personResponsibility](../resources/personresponsibility.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1c21e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1c21e-106">Permissions</span></span>

<span data-ttu-id="1c21e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c21e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1c21e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1c21e-109">Permission type</span></span>                        | <span data-ttu-id="1c21e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1c21e-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="1c21e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1c21e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1c21e-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c21e-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="1c21e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1c21e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c21e-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c21e-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="1c21e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1c21e-115">Application</span></span>                            | <span data-ttu-id="1c21e-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c21e-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="1c21e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1c21e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/responsibilities/{id}
DELETE /users/{id | userPrincipalName}/responsibilities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1c21e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1c21e-118">Request headers</span></span>
|<span data-ttu-id="1c21e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="1c21e-119">Name</span></span>|<span data-ttu-id="1c21e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1c21e-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1c21e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1c21e-121">Authorization</span></span>|<span data-ttu-id="1c21e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1c21e-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c21e-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1c21e-124">Request body</span></span>
<span data-ttu-id="1c21e-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1c21e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c21e-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c21e-126">Response</span></span>

<span data-ttu-id="1c21e-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1c21e-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="1c21e-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="1c21e-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1c21e-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c21e-129">Request</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f"],
  "name": "delete_personresponsibility"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/me/responsibilities/0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f
```

### <a name="response"></a><span data-ttu-id="1c21e-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c21e-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


