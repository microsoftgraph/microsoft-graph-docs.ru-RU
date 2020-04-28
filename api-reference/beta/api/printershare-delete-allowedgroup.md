---
title: Удаление Алловедграуп
description: Отозвать доступ указанной группы, чтобы отправить задания печати на соответствующий общий ресурс принтера.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: f154cbf1b59a67a8d2e306ea14e1ef490c63b3fe
ms.sourcegitcommit: 195fa0d441a49662e144323d37518dbba0c76fc7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2020
ms.locfileid: "43807137"
---
# <a name="delete-allowedgroup"></a><span data-ttu-id="de6ba-103">Удаление Алловедграуп</span><span class="sxs-lookup"><span data-stu-id="de6ba-103">Delete allowedGroup</span></span>

<span data-ttu-id="de6ba-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de6ba-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de6ba-105">Отозвать доступ указанной группы, чтобы послать задания печати в связанный [принтершаре](../resources/printershare.md).</span><span class="sxs-lookup"><span data-stu-id="de6ba-105">Revoke the specified group's access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="de6ba-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="de6ba-106">Permissions</span></span>
<span data-ttu-id="de6ba-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de6ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="de6ba-109">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="de6ba-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="de6ba-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de6ba-110">Permission type</span></span> | <span data-ttu-id="de6ba-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="de6ba-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="de6ba-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de6ba-112">Delegated (work or school account)</span></span>| <span data-ttu-id="de6ba-113">Users. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="de6ba-113">Users.Read.All</span></span> |
|<span data-ttu-id="de6ba-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de6ba-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de6ba-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de6ba-115">Not Supported.</span></span>|
|<span data-ttu-id="de6ba-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="de6ba-116">Application</span></span>|<span data-ttu-id="de6ba-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de6ba-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="de6ba-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de6ba-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/printerShares/{id}/allowedGroups/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="de6ba-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="de6ba-119">Request headers</span></span>
| <span data-ttu-id="de6ba-120">Имя</span><span class="sxs-lookup"><span data-stu-id="de6ba-120">Name</span></span>          | <span data-ttu-id="de6ba-121">Описание</span><span class="sxs-lookup"><span data-stu-id="de6ba-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="de6ba-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="de6ba-122">Authorization</span></span> | <span data-ttu-id="de6ba-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="de6ba-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="de6ba-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="de6ba-125">Request body</span></span>
<span data-ttu-id="de6ba-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="de6ba-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="de6ba-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="de6ba-127">Response</span></span>
<span data-ttu-id="de6ba-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="de6ba-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de6ba-130">Пример</span><span class="sxs-lookup"><span data-stu-id="de6ba-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="de6ba-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="de6ba-131">Request</span></span>
<span data-ttu-id="de6ba-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="de6ba-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_allowedgroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/printerShares/{id}/allowedGroup/{id}/$ref
```
##### <a name="response"></a><span data-ttu-id="de6ba-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="de6ba-133">Response</span></span>
<span data-ttu-id="de6ba-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="de6ba-134">The following is an example of the response.</span></span>
><span data-ttu-id="de6ba-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="de6ba-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete allowedGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->