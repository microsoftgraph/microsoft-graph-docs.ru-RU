---
title: Получение Коннектионоператион
description: Получение свойств объекта Коннектионоператион.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 76936584883549fb2fd2fedbeed42cbe78702e55
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936596"
---
# <a name="get-connectionoperation"></a><span data-ttu-id="6eea4-103">Получение Коннектионоператион</span><span class="sxs-lookup"><span data-stu-id="6eea4-103">Get connectionOperation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6eea4-104">Получение свойств объекта [коннектионоператион](../resources/connectionoperation.md).</span><span class="sxs-lookup"><span data-stu-id="6eea4-104">Retrieve the properties of a [connectionOperation](../resources/connectionoperation.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6eea4-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6eea4-105">Permissions</span></span>

<span data-ttu-id="6eea4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6eea4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6eea4-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6eea4-108">Permission type</span></span>                        | <span data-ttu-id="6eea4-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6eea4-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6eea4-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6eea4-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="6eea4-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6eea4-111">Not supported.</span></span> |
| <span data-ttu-id="6eea4-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6eea4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6eea4-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6eea4-113">Not supported.</span></span> |
| <span data-ttu-id="6eea4-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6eea4-114">Application</span></span>                            | <span data-ttu-id="6eea4-115">Екстерналитем. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="6eea4-115">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6eea4-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6eea4-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections/{connection-id}/operations/{operation-id}
```

## <a name="request-headers"></a><span data-ttu-id="6eea4-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6eea4-117">Request headers</span></span>

| <span data-ttu-id="6eea4-118">Имя</span><span class="sxs-lookup"><span data-stu-id="6eea4-118">Name</span></span>          | <span data-ttu-id="6eea4-119">Описание</span><span class="sxs-lookup"><span data-stu-id="6eea4-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="6eea4-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6eea4-120">Authorization</span></span> | <span data-ttu-id="6eea4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6eea4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6eea4-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6eea4-123">Request body</span></span>

<span data-ttu-id="6eea4-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6eea4-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6eea4-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="6eea4-125">Response</span></span>

<span data-ttu-id="6eea4-126">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [коннектионоператион](../resources/connectionoperation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6eea4-126">If successful, this method returns a `200 OK` response code and the requested [connectionOperation](../resources/connectionoperation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6eea4-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="6eea4-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6eea4-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="6eea4-128">Request</span></span>

<span data-ttu-id="6eea4-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6eea4-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_connectionoperation"
}-->

```http
GET https://graph.microsoft.com/beta/connections/contosohr/operations/3ed1595a-4bae-43c2-acda-ef973e581323
```

<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="6eea4-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="6eea4-130">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="6eea4-131">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6eea4-131">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "expectError": true,
  "@odata.type": "microsoft.graph.connectionOperation"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "3ed1595a-4bae-43c2-acda-ef973e581323",
  "status": "failed",
  "error": {
    "message": "Server error, something went wrong"
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get connectionOperation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
