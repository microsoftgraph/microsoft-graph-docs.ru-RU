---
title: Удаление Екстерналконнектион
description: Удаление Екстерналконнектион.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 0bf79319c13d627c68d233a9ccd83c016e62b9fb
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938676"
---
# <a name="delete-externalconnection"></a><span data-ttu-id="5b283-103">Удаление Екстерналконнектион</span><span class="sxs-lookup"><span data-stu-id="5b283-103">Delete externalConnection</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b283-104">Удаление [екстерналконнектион](../resources/externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="5b283-104">Delete an [externalConnection](../resources/externalconnection.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5b283-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5b283-105">Permissions</span></span>

<span data-ttu-id="5b283-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b283-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5b283-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5b283-108">Permission type</span></span>                        | <span data-ttu-id="5b283-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5b283-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5b283-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b283-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="5b283-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b283-111">Not supported.</span></span> |
| <span data-ttu-id="5b283-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b283-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b283-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b283-113">Not supported.</span></span> |
| <span data-ttu-id="5b283-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5b283-114">Application</span></span>                            | <span data-ttu-id="5b283-115">Екстерналитем. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5b283-115">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5b283-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b283-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /external/connections/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5b283-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5b283-117">Request headers</span></span>

| <span data-ttu-id="5b283-118">Имя</span><span class="sxs-lookup"><span data-stu-id="5b283-118">Name</span></span>          | <span data-ttu-id="5b283-119">Описание</span><span class="sxs-lookup"><span data-stu-id="5b283-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="5b283-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5b283-120">Authorization</span></span> | <span data-ttu-id="5b283-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b283-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5b283-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5b283-123">Request body</span></span>

<span data-ttu-id="5b283-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5b283-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b283-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="5b283-125">Response</span></span>

<span data-ttu-id="5b283-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="5b283-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5b283-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="5b283-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5b283-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b283-129">Request</span></span>

<span data-ttu-id="5b283-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5b283-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_connection"
}-->

```http
DELETE https://graph.microsoft.com/beta/connections/contosohr
```

<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="5b283-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b283-131">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="5b283-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5b283-132">The following is an example of the response.</span></span>

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
  "description": "Delete externalConnection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
