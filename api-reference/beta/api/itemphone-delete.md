---
title: Удаление itemPhone
description: Удаление объекта itemPhone из профиля пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 4b947a7674f73a4351cdb6742587812acd66d253
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50577417"
---
# <a name="delete-itemphonenumber"></a><span data-ttu-id="fcf2d-103">Удаление элементаPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="fcf2d-103">Delete itemPhoneNumber</span></span>

<span data-ttu-id="fcf2d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fcf2d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fcf2d-105">Удаление [объекта itemPhone](../resources/itemphone.md) из профиля [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="fcf2d-105">Delete an [itemPhone](../resources/itemphone.md) object from the user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fcf2d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fcf2d-106">Permissions</span></span>

<span data-ttu-id="fcf2d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fcf2d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fcf2d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fcf2d-109">Permission type</span></span>                        | <span data-ttu-id="fcf2d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fcf2d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="fcf2d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fcf2d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="fcf2d-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fcf2d-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="fcf2d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fcf2d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fcf2d-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fcf2d-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="fcf2d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fcf2d-115">Application</span></span>                            | <span data-ttu-id="fcf2d-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fcf2d-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="fcf2d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fcf2d-117">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/profile/phones/{itemPhoneId}
DELETE /users/{userId}/profile/phones/{itemPhoneId}
```

## <a name="request-headers"></a><span data-ttu-id="fcf2d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fcf2d-118">Request headers</span></span>

|<span data-ttu-id="fcf2d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="fcf2d-119">Name</span></span>|<span data-ttu-id="fcf2d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="fcf2d-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fcf2d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fcf2d-121">Authorization</span></span>|<span data-ttu-id="fcf2d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fcf2d-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fcf2d-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fcf2d-124">Request body</span></span>

<span data-ttu-id="fcf2d-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fcf2d-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fcf2d-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="fcf2d-126">Response</span></span>

<span data-ttu-id="fcf2d-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fcf2d-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="fcf2d-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="fcf2d-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fcf2d-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="fcf2d-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_itemphone"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/users/{userId}/profile/phones/{itemPhoneId}
```

### <a name="response"></a><span data-ttu-id="fcf2d-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="fcf2d-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


