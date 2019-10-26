---
title: Удаление Трустфрамеворккэйсет
description: Удаление объекта **трустфрамеворккэйсет** .
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ad73363f568c97be720cdcab3711e762b8dcde1a
ms.sourcegitcommit: 8bef2bc8b9e56d1a787ea2f0cda4ed94f05109ad
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/26/2019
ms.locfileid: "37734685"
---
# <a name="delete-trustframeworkkeyset"></a><span data-ttu-id="0f1ff-103">Удаление Трустфрамеворккэйсет</span><span class="sxs-lookup"><span data-stu-id="0f1ff-103">Delete trustFrameworkKeySet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f1ff-104">Удаление объекта [трустфрамеворккэйсет](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="0f1ff-104">Delete a [trustFrameworkKeySet](../resources/trustframeworkkeyset.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0f1ff-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0f1ff-105">Permissions</span></span>

<span data-ttu-id="0f1ff-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f1ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0f1ff-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0f1ff-108">Permission type</span></span>                        | <span data-ttu-id="0f1ff-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0f1ff-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0f1ff-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0f1ff-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0f1ff-111">Трустфрамеворккэйсет. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0f1ff-111">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="0f1ff-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0f1ff-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f1ff-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f1ff-113">Not supported.</span></span> |
| <span data-ttu-id="0f1ff-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0f1ff-114">Application</span></span>                            | <span data-ttu-id="0f1ff-115">Трустфрамеворккэйсет. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0f1ff-115">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0f1ff-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0f1ff-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /trustFramework/keySets/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0f1ff-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0f1ff-117">Request headers</span></span>

| <span data-ttu-id="0f1ff-118">Имя</span><span class="sxs-lookup"><span data-stu-id="0f1ff-118">Name</span></span>          | <span data-ttu-id="0f1ff-119">Описание</span><span class="sxs-lookup"><span data-stu-id="0f1ff-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0f1ff-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0f1ff-120">Authorization</span></span> | <span data-ttu-id="0f1ff-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0f1ff-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0f1ff-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0f1ff-123">Request body</span></span>

<span data-ttu-id="0f1ff-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0f1ff-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0f1ff-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f1ff-125">Response</span></span>

<span data-ttu-id="0f1ff-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0f1ff-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0f1ff-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="0f1ff-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0f1ff-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="0f1ff-129">Request</span></span>

<span data-ttu-id="0f1ff-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0f1ff-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_trustframeworkkeyset"
}-->

```http
DELETE https://graph.microsoft.com/beta/trustFramework/keySets/{id}
```

### <a name="response"></a><span data-ttu-id="0f1ff-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f1ff-131">Response</span></span>

<span data-ttu-id="0f1ff-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0f1ff-132">The following is an example of the response.</span></span>

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
  "description": "Delete trustFrameworkKeySet",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
