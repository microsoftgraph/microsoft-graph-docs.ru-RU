---
title: Удаление Активитибаседтимеаутполици
description: Удаление Активитибаседтимеаутполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8124030da30028e9c3ee9cef67541627e5888292
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43227952"
---
# <a name="delete-activitybasedtimeoutpolicy"></a><span data-ttu-id="6a9b4-103">Удаление Активитибаседтимеаутполици</span><span class="sxs-lookup"><span data-stu-id="6a9b4-103">Delete activityBasedTimeoutPolicy</span></span>

<span data-ttu-id="6a9b4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a9b4-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="6a9b4-105">Удаление объекта [активитибаседтимеаутполици](../resources/activitybasedtimeoutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="6a9b4-105">Delete an [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6a9b4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6a9b4-106">Permissions</span></span>

<span data-ttu-id="6a9b4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a9b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6a9b4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6a9b4-109">Permission type</span></span>                        | <span data-ttu-id="6a9b4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6a9b4-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6a9b4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6a9b4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6a9b4-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="6a9b4-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="6a9b4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6a9b4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a9b4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a9b4-114">Not supported.</span></span> |
| <span data-ttu-id="6a9b4-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="6a9b4-115">Application</span></span>                            | <span data-ttu-id="6a9b4-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="6a9b4-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="6a9b4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6a9b4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/activityBasedTimeoutPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6a9b4-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6a9b4-118">Request headers</span></span>

| <span data-ttu-id="6a9b4-119">Имя</span><span class="sxs-lookup"><span data-stu-id="6a9b4-119">Name</span></span>          | <span data-ttu-id="6a9b4-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6a9b4-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="6a9b4-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6a9b4-121">Authorization</span></span> | <span data-ttu-id="6a9b4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6a9b4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6a9b4-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6a9b4-124">Request body</span></span>

<span data-ttu-id="6a9b4-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6a9b4-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a9b4-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="6a9b4-126">Response</span></span>

<span data-ttu-id="6a9b4-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6a9b4-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="6a9b4-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="6a9b4-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6a9b4-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="6a9b4-129">Request</span></span>

<span data-ttu-id="6a9b4-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6a9b4-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_activitybasedtimeoutpolicy"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/policies/activityBasedTimeoutPolicies/{id}
```

### <a name="response"></a><span data-ttu-id="6a9b4-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a9b4-131">Response</span></span>

<span data-ttu-id="6a9b4-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6a9b4-132">The following is an example of the response.</span></span>

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
  "description": "Delete activityBasedTimeoutPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
