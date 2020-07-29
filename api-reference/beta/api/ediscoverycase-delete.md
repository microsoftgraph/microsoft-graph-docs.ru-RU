---
title: Удаление Едисковерикасе
description: Удаление объекта Едисковерикасе.
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: c1ef35c31bb349c2e4ea8622d2f18f90ed6e0b83
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/29/2020
ms.locfileid: "46510213"
---
# <a name="delete-ediscoverycase"></a><span data-ttu-id="b4a07-103">Удаление Едисковерикасе</span><span class="sxs-lookup"><span data-stu-id="b4a07-103">Delete ediscoveryCase</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4a07-104">Удаление объекта [едисковерикасе](../resources/ediscoverycase.md) .</span><span class="sxs-lookup"><span data-stu-id="b4a07-104">Delete an [ediscoveryCase](../resources/ediscoverycase.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4a07-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b4a07-105">Permissions</span></span>

<span data-ttu-id="b4a07-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4a07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b4a07-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b4a07-108">Permission type</span></span>                        | <span data-ttu-id="b4a07-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b4a07-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b4a07-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4a07-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b4a07-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="b4a07-111">User.Read</span></span>      |
| <span data-ttu-id="b4a07-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4a07-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4a07-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4a07-113">Not supported.</span></span> |
| <span data-ttu-id="b4a07-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b4a07-114">Application</span></span>                            | <span data-ttu-id="b4a07-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4a07-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b4a07-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b4a07-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /compliance/ediscovery/cases/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b4a07-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b4a07-117">Request headers</span></span>

| <span data-ttu-id="b4a07-118">Имя</span><span class="sxs-lookup"><span data-stu-id="b4a07-118">Name</span></span>          | <span data-ttu-id="b4a07-119">Описание</span><span class="sxs-lookup"><span data-stu-id="b4a07-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b4a07-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b4a07-120">Authorization</span></span> | <span data-ttu-id="b4a07-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4a07-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b4a07-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b4a07-123">Request body</span></span>

<span data-ttu-id="b4a07-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b4a07-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4a07-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4a07-125">Response</span></span>

<span data-ttu-id="b4a07-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b4a07-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b4a07-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="b4a07-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b4a07-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4a07-129">Request</span></span>

<span data-ttu-id="b4a07-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b4a07-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_ediscoverycase"
}-->

```http
DELETE https://graph.microsoft.com/beta/compliance/ediscovery/cases/061b9a92-8926-4bd9-b41d-abf35edc7583
```

### <a name="response"></a><span data-ttu-id="b4a07-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4a07-131">Response</span></span>

<span data-ttu-id="b4a07-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b4a07-132">The following is an example of the response.</span></span>

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
  "description": "Delete ediscoveryCase",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
