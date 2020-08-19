---
title: Удаление Едукатионалактивити
description: Удаление объекта Едукатионалактивити из профиля пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 96c717171f683d2a32e62b4e79b80639e2cb5242
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810953"
---
# <a name="delete-educationalactivity"></a><span data-ttu-id="ddbdf-103">Удаление Едукатионалактивити</span><span class="sxs-lookup"><span data-stu-id="ddbdf-103">Delete educationalActivity</span></span>

<span data-ttu-id="ddbdf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ddbdf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ddbdf-105">Удаление объекта [едукатионалактивити](../resources/educationalactivity.md) из [профиля](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="ddbdf-105">Delete an [educationalActivity](../resources/educationalactivity.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ddbdf-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ddbdf-106">Permissions</span></span>

<span data-ttu-id="ddbdf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ddbdf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ddbdf-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ddbdf-109">Permission type</span></span>                        | <span data-ttu-id="ddbdf-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ddbdf-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ddbdf-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ddbdf-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ddbdf-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ddbdf-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="ddbdf-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ddbdf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ddbdf-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ddbdf-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="ddbdf-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ddbdf-115">Application</span></span>                            | <span data-ttu-id="ddbdf-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddbdf-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="ddbdf-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ddbdf-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/educationalActivities/{id} 
DELETE /users/{id | userPrincipalName}/profile/educationalActivities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ddbdf-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ddbdf-118">Request headers</span></span>

| <span data-ttu-id="ddbdf-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ddbdf-119">Name</span></span>           |<span data-ttu-id="ddbdf-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ddbdf-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="ddbdf-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ddbdf-121">Authorization</span></span>  | <span data-ttu-id="ddbdf-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ddbdf-p102">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="ddbdf-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ddbdf-124">Request body</span></span>

<span data-ttu-id="ddbdf-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ddbdf-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ddbdf-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="ddbdf-126">Response</span></span>

<span data-ttu-id="ddbdf-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ddbdf-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ddbdf-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="ddbdf-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ddbdf-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="ddbdf-130">Request</span></span>

<span data-ttu-id="ddbdf-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ddbdf-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationalactivity"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/educationalActivities/{id}
```

### <a name="response"></a><span data-ttu-id="ddbdf-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="ddbdf-132">Response</span></span>

<span data-ttu-id="ddbdf-133">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ddbdf-133">The following is an example of the response.</span></span>

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
  "description": "Delete educationalActivity",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
