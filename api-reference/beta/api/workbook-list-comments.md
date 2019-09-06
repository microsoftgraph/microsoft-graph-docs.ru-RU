---
title: Список Воркбуккомментс
description: Получение списка объектов Воркбуккомментс.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: d78176ecee83f1c233c7bf9a2844ba0a12fa2dea
ms.sourcegitcommit: c74195b8725c3f28bb3bded43c855261590a0cec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/06/2019
ms.locfileid: "36775848"
---
# <a name="list-workbookcomments"></a><span data-ttu-id="bdb80-103">Список Воркбуккомментс</span><span class="sxs-lookup"><span data-stu-id="bdb80-103">List workbookComments</span></span>

<span data-ttu-id="bdb80-104">Получение списка объектов [воркбуккоммент](../resources/workbookcomment.md) .</span><span class="sxs-lookup"><span data-stu-id="bdb80-104">Retrieve a list of  [workbookComment](../resources/workbookcomment.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="bdb80-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bdb80-105">Permissions</span></span>

<span data-ttu-id="bdb80-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bdb80-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bdb80-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bdb80-108">Permission type</span></span>                        | <span data-ttu-id="bdb80-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bdb80-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bdb80-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bdb80-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="bdb80-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bdb80-111">Files.ReadWrite</span></span> |
| <span data-ttu-id="bdb80-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bdb80-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bdb80-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bdb80-113">Not supported.</span></span> |
| <span data-ttu-id="bdb80-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bdb80-114">Application</span></span>                            | <span data-ttu-id="bdb80-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bdb80-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bdb80-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bdb80-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /workbook/comments
```

## <a name="request-headers"></a><span data-ttu-id="bdb80-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bdb80-117">Request headers</span></span>

| <span data-ttu-id="bdb80-118">Имя</span><span class="sxs-lookup"><span data-stu-id="bdb80-118">Name</span></span>      |<span data-ttu-id="bdb80-119">Описание</span><span class="sxs-lookup"><span data-stu-id="bdb80-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bdb80-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bdb80-120">Authorization</span></span> | <span data-ttu-id="bdb80-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bdb80-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bdb80-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bdb80-123">Request body</span></span>

<span data-ttu-id="bdb80-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bdb80-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bdb80-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="bdb80-125">Response</span></span>

<span data-ttu-id="bdb80-126">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [воркбуккоммент](../resources/workbookcomment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bdb80-126">If successful, this method returns a `200 OK` response code and a collection of [workbookComment](../resources/workbookcomment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bdb80-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="bdb80-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bdb80-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="bdb80-128">Request</span></span>

<span data-ttu-id="bdb80-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bdb80-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_comments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/root/workbook/comments
```

### <a name="response"></a><span data-ttu-id="bdb80-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="bdb80-130">Response</span></span>

<span data-ttu-id="bdb80-131">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bdb80-131">The following is an example of the response.</span></span>

> <span data-ttu-id="bdb80-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bdb80-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookComment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "content": "This is text of comment.",
      "contentType": "plain",
      "id": "{97A21473-8339-4BF0-BCB6-F55E4909FFB8}"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List comments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
