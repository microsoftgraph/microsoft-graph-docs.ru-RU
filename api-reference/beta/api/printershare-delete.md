---
title: Удаление Принтершаре
description: Удаление общего принтера (отменяйте общий доступ к связанному принтеру). Это действие невозможно отменить. Если к принтеру предоставлен общий доступ в будущем, все пользователи Windows, на которых ранее устанавливался принтер, должны обнаружить и повторно установить его.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 534dc61037efd99f92100c87bc911cdea6dfb6a5
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42896212"
---
# <a name="delete-printershare"></a><span data-ttu-id="67d7a-105">Удаление Принтершаре</span><span class="sxs-lookup"><span data-stu-id="67d7a-105">Delete printerShare</span></span>

<span data-ttu-id="67d7a-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67d7a-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67d7a-107">Удаление общего принтера (отменяйте общий доступ к связанному [принтеру](../resources/printer.md)).</span><span class="sxs-lookup"><span data-stu-id="67d7a-107">Delete a printer share (unshare the associated [printer](../resources/printer.md)).</span></span> <span data-ttu-id="67d7a-108">Это действие невозможно отменить.</span><span class="sxs-lookup"><span data-stu-id="67d7a-108">This action cannot be undone.</span></span> <span data-ttu-id="67d7a-109">Если к [принтеру](../resources/printer.md) предоставлен общий доступ в будущем, все пользователи Windows, на которых ранее устанавливался [принтер](../resources/printer.md) , должны обнаружить и переустановить его.</span><span class="sxs-lookup"><span data-stu-id="67d7a-109">If the [printer](../resources/printer.md) is shared again in the future, any Windows users who had previously installed the [printer](../resources/printer.md) will need to discover and reinstall it.</span></span>

## <a name="permissions"></a><span data-ttu-id="67d7a-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="67d7a-110">Permissions</span></span>
<span data-ttu-id="67d7a-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67d7a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="67d7a-113">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="67d7a-113">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="67d7a-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="67d7a-114">Permission type</span></span> | <span data-ttu-id="67d7a-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="67d7a-115">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="67d7a-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="67d7a-116">Delegated (work or school account)</span></span>| <span data-ttu-id="67d7a-117">Users. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="67d7a-117">Users.Read.All</span></span> |
|<span data-ttu-id="67d7a-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="67d7a-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67d7a-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67d7a-119">Not Supported.</span></span>|
|<span data-ttu-id="67d7a-120">Для приложения</span><span class="sxs-lookup"><span data-stu-id="67d7a-120">Application</span></span>|<span data-ttu-id="67d7a-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67d7a-121">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="67d7a-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="67d7a-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/printerShares/{id}
DELETE /print/printers/{id}/share
```
## <a name="request-headers"></a><span data-ttu-id="67d7a-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="67d7a-123">Request headers</span></span>
| <span data-ttu-id="67d7a-124">Имя</span><span class="sxs-lookup"><span data-stu-id="67d7a-124">Name</span></span>          | <span data-ttu-id="67d7a-125">Описание</span><span class="sxs-lookup"><span data-stu-id="67d7a-125">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="67d7a-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="67d7a-126">Authorization</span></span> | <span data-ttu-id="67d7a-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="67d7a-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="67d7a-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="67d7a-129">Request body</span></span>
<span data-ttu-id="67d7a-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="67d7a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="67d7a-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="67d7a-131">Response</span></span>
<span data-ttu-id="67d7a-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="67d7a-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67d7a-134">Пример</span><span class="sxs-lookup"><span data-stu-id="67d7a-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="67d7a-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="67d7a-135">Request</span></span>
<span data-ttu-id="67d7a-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="67d7a-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_printershare"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/printerShares/{id}
```
##### <a name="response"></a><span data-ttu-id="67d7a-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="67d7a-137">Response</span></span>
<span data-ttu-id="67d7a-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="67d7a-138">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete printerShare",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->