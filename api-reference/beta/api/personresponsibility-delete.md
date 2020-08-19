---
title: Удаление Персонреспонсибилити
description: Удаляет объект Персонреспонсибилити.
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: bb99620a23370f6763fa6544a3992053f5057183
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46813161"
---
# <a name="delete-personresponsibility"></a><span data-ttu-id="b75be-103">Удаление Персонреспонсибилити</span><span class="sxs-lookup"><span data-stu-id="b75be-103">Delete personResponsibility</span></span>
<span data-ttu-id="b75be-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b75be-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b75be-105">Удаляет объект [персонреспонсибилити](../resources/personresponsibility.md) из [профиля](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="b75be-105">Deletes a [personResponsibility](../resources/personresponsibility.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b75be-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b75be-106">Permissions</span></span>

<span data-ttu-id="b75be-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b75be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b75be-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b75be-109">Permission type</span></span>                        | <span data-ttu-id="b75be-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b75be-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="b75be-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b75be-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b75be-112">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="b75be-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="b75be-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b75be-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b75be-114">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="b75be-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="b75be-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="b75be-115">Application</span></span>                            | <span data-ttu-id="b75be-116">User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="b75be-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="b75be-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b75be-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/profile/responsibilities/{id}
DELETE /users/{id | userPrincipalName}/profile/responsibilities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b75be-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b75be-118">Request headers</span></span>
|<span data-ttu-id="b75be-119">Имя</span><span class="sxs-lookup"><span data-stu-id="b75be-119">Name</span></span>|<span data-ttu-id="b75be-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b75be-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b75be-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b75be-121">Authorization</span></span>|<span data-ttu-id="b75be-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b75be-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b75be-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b75be-124">Request body</span></span>
<span data-ttu-id="b75be-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b75be-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b75be-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="b75be-126">Response</span></span>

<span data-ttu-id="b75be-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b75be-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="b75be-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="b75be-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b75be-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="b75be-129">Request</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f"],
  "name": "delete_personresponsibility"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/me/profile/responsibilities/0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f
```

### <a name="response"></a><span data-ttu-id="b75be-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="b75be-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
