---
title: Удаление Кондитионалакцессполици
description: Удаление объекта Кондитионалакцессполици.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e1064f54368f4bf4be2f655579da3ed133059d53
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384654"
---
# <a name="delete-conditionalaccesspolicy"></a><span data-ttu-id="64908-103">Удаление Кондитионалакцессполици</span><span class="sxs-lookup"><span data-stu-id="64908-103">Delete conditionalAccessPolicy</span></span>

<span data-ttu-id="64908-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64908-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="64908-105">Удаление объекта [кондитионалакцессполици](../resources/conditionalaccesspolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="64908-105">Delete a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="64908-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="64908-106">Permissions</span></span>

<span data-ttu-id="64908-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64908-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64908-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64908-109">Permission type</span></span>                        | <span data-ttu-id="64908-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="64908-110">Permissions (from least to most privileged)</span></span>                    |
|:--------------------------------------|:---------------------------------------------------------------|
| <span data-ttu-id="64908-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64908-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="64908-112">Policy. Read. ALL и Policy. ReadWrite. Кондитионалакцесс</span><span class="sxs-lookup"><span data-stu-id="64908-112">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="64908-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64908-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64908-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64908-114">Not supported.</span></span> |
| <span data-ttu-id="64908-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="64908-115">Application</span></span>                            | <span data-ttu-id="64908-116">Policy. Read. ALL и Policy. ReadWrite. Кондитионалакцесс</span><span class="sxs-lookup"><span data-stu-id="64908-116">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |

## <a name="http-request"></a><span data-ttu-id="64908-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64908-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/conditionalAccess/policies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="64908-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="64908-118">Request headers</span></span>

| <span data-ttu-id="64908-119">Имя</span><span class="sxs-lookup"><span data-stu-id="64908-119">Name</span></span>          | <span data-ttu-id="64908-120">Описание</span><span class="sxs-lookup"><span data-stu-id="64908-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="64908-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="64908-121">Authorization</span></span> | <span data-ttu-id="64908-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64908-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="64908-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="64908-124">Request body</span></span>

<span data-ttu-id="64908-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="64908-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64908-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="64908-126">Response</span></span>

<span data-ttu-id="64908-p103">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="64908-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64908-129">Пример</span><span class="sxs-lookup"><span data-stu-id="64908-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="64908-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="64908-130">Request</span></span>

<span data-ttu-id="64908-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="64908-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="64908-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="64908-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conditionalaccesspolicy"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/identity/conditionalAccess/policies/{id}
```

---

### <a name="response"></a><span data-ttu-id="64908-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="64908-133">Response</span></span>

<span data-ttu-id="64908-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="64908-134">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete conditionalAccessPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
