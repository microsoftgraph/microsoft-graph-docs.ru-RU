---
title: Создание Алловедграуп
description: Предоставление указанному групповому доступу на отправку заданий печати на связанный принтер.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: ce8080503f45a79dae422186ab360bc0e4071dd0
ms.sourcegitcommit: 195fa0d441a49662e144323d37518dbba0c76fc7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2020
ms.locfileid: "43807124"
---
# <a name="create-allowedgroup"></a><span data-ttu-id="1b857-103">Создание Алловедграуп</span><span class="sxs-lookup"><span data-stu-id="1b857-103">Create allowedGroup</span></span>

<span data-ttu-id="1b857-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b857-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b857-105">Предоставление указанному групповому доступу на отправку заданий печати связанному [принтершаре](../resources/printershare.md).</span><span class="sxs-lookup"><span data-stu-id="1b857-105">Grant the specified group access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1b857-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1b857-106">Permissions</span></span>
<span data-ttu-id="1b857-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b857-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="1b857-109">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="1b857-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="1b857-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1b857-110">Permission type</span></span> | <span data-ttu-id="1b857-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1b857-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="1b857-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1b857-112">Delegated (work or school account)</span></span>| <span data-ttu-id="1b857-113">Users. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="1b857-113">Users.Read.All</span></span> |
|<span data-ttu-id="1b857-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1b857-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b857-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b857-115">Not Supported.</span></span>|
|<span data-ttu-id="1b857-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1b857-116">Application</span></span>|<span data-ttu-id="1b857-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b857-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b857-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1b857-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printerShares/{id}/allowedGroups/$ref
```
## <a name="request-headers"></a><span data-ttu-id="1b857-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1b857-119">Request headers</span></span>
| <span data-ttu-id="1b857-120">Имя</span><span class="sxs-lookup"><span data-stu-id="1b857-120">Name</span></span>          | <span data-ttu-id="1b857-121">Описание</span><span class="sxs-lookup"><span data-stu-id="1b857-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="1b857-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1b857-122">Authorization</span></span> | <span data-ttu-id="1b857-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1b857-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1b857-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1b857-125">Content-type</span></span>  | <span data-ttu-id="1b857-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1b857-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b857-128">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="1b857-128">Request body</span></span>
<span data-ttu-id="1b857-129">В теле запроса добавьте ссылку на объект Group с помощью `@odata.id` формата, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="1b857-129">In the request body, supply a reference to a group entity by using the `@odata.id` format, as shown in the following example.</span></span>

## <a name="response"></a><span data-ttu-id="1b857-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="1b857-130">Response</span></span>
<span data-ttu-id="1b857-131">В случае успешного выполнения этот метод возвращает код отклика `201 Created`.</span><span class="sxs-lookup"><span data-stu-id="1b857-131">If successful, this method returns a `201 Created` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1b857-132">Пример</span><span class="sxs-lookup"><span data-stu-id="1b857-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="1b857-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="1b857-133">Request</span></span>
<span data-ttu-id="1b857-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1b857-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_allowedgroup_from_printers"
}-->
```http
POST https://graph.microsoft.com/beta/print/printerShares/{id}/allowedGroups/$ref
Content-type: application/json
Content-length: 67

{
  "@odata.id": "https://graph.microsoft.com/beta/groups/{id}"
}
```

<span data-ttu-id="1b857-135">В теле запроса добавьте ссылку на объект Group, указав URI Microsoft Graph в `@odata.id` поле тела JSON.</span><span class="sxs-lookup"><span data-stu-id="1b857-135">In the request body, supply a reference to a group entity by including the group's Microsoft Graph URI in the `@odata.id` field of the JSON body.</span></span>

### <a name="response"></a><span data-ttu-id="1b857-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="1b857-136">Response</span></span>
<span data-ttu-id="1b857-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1b857-137">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create allowedGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
