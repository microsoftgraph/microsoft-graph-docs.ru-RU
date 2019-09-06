---
title: Создание Воркбуккомментрепли
description: Используйте этот API для создания нового Воркбуккомментрепли.
localization_priority: Normal
author: grangeryy
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: edf4dafa40c7323bde788234f1efa4308f401fd3
ms.sourcegitcommit: c74195b8725c3f28bb3bded43c855261590a0cec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/06/2019
ms.locfileid: "36775771"
---
# <a name="create-workbookcommentreply"></a><span data-ttu-id="66643-103">Создание Воркбуккомментрепли</span><span class="sxs-lookup"><span data-stu-id="66643-103">Create workbookCommentReply</span></span>

<span data-ttu-id="66643-104">Создание нового объекта [воркбуккомментрепли](../resources/workbookcommentreply.md) .</span><span class="sxs-lookup"><span data-stu-id="66643-104">Create a new [workbookCommentReply](../resources/workbookcommentreply.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="66643-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="66643-105">Permissions</span></span>

<span data-ttu-id="66643-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66643-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="66643-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="66643-108">Permission type</span></span>                        | <span data-ttu-id="66643-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="66643-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="66643-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="66643-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="66643-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66643-111">Files.ReadWrite</span></span> |
| <span data-ttu-id="66643-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="66643-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66643-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66643-113">Not supported.</span></span> |
| <span data-ttu-id="66643-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="66643-114">Application</span></span>                            | <span data-ttu-id="66643-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66643-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="66643-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="66643-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /workbook/comments/{id}/replies
```

## <a name="request-headers"></a><span data-ttu-id="66643-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="66643-117">Request headers</span></span>

| <span data-ttu-id="66643-118">Имя</span><span class="sxs-lookup"><span data-stu-id="66643-118">Name</span></span>          | <span data-ttu-id="66643-119">Описание</span><span class="sxs-lookup"><span data-stu-id="66643-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="66643-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="66643-120">Authorization</span></span> | <span data-ttu-id="66643-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="66643-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="66643-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="66643-123">Request body</span></span>

<span data-ttu-id="66643-124">В тексте запроса добавьте представление объекта [воркбуккомментрепли](../resources/workbookcommentreply.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="66643-124">In the request body, supply a JSON representation of a [workbookCommentReply](../resources/workbookcommentreply.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="66643-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="66643-125">Response</span></span>

<span data-ttu-id="66643-126">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [воркбуккомментрепли](../resources/workbookcommentreply.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="66643-126">If successful, this method returns a `201 Created` response code and a new [workbookCommentReply](../resources/workbookcommentreply.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="66643-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="66643-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="66643-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="66643-128">Request</span></span>

<span data-ttu-id="66643-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="66643-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_workbookcommentreply_from_workbookcomment"
}-->

```http
POST https://graph.microsoft.com/v1.0/drive/root/workbook/comments/{id}/replies
Content-type: application/json

{
  "content": "This is my reply to the comment.",
  "contentType": "plain"
}
```

### <a name="response"></a><span data-ttu-id="66643-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="66643-130">Response</span></span>

<span data-ttu-id="66643-131">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="66643-131">The following is an example of the response.</span></span>

> <span data-ttu-id="66643-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="66643-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookCommentReply"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "content": "This is my reply to the comment.",
  "contentType": "plain",
  "id": "{97A21473-8339-4BF0-BCB6-F55E4909FFB8}"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create workbookCommentReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
