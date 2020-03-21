---
title: Удаление соединителя
description: Удаление (Отмена регистрации) соединителя.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 1404bbf5851770eec12c3234ac80e84461ffb029
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42896326"
---
# <a name="delete-connector"></a><span data-ttu-id="95c3b-103">Удаление соединителя</span><span class="sxs-lookup"><span data-stu-id="95c3b-103">Delete connector</span></span>

<span data-ttu-id="95c3b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95c3b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95c3b-105">Удаление (Отмена регистрации) **принтконнектор**.</span><span class="sxs-lookup"><span data-stu-id="95c3b-105">Delete (unregister) a **printConnector**.</span></span>

## <a name="permissions"></a><span data-ttu-id="95c3b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="95c3b-106">Permissions</span></span>
<span data-ttu-id="95c3b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95c3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="95c3b-109">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="95c3b-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="95c3b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="95c3b-110">Permission type</span></span> | <span data-ttu-id="95c3b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="95c3b-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="95c3b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="95c3b-112">Delegated (work or school account)</span></span>| <span data-ttu-id="95c3b-113">Users. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="95c3b-113">Users.Read.All</span></span> |
|<span data-ttu-id="95c3b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="95c3b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95c3b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95c3b-115">Not Supported.</span></span>|
|<span data-ttu-id="95c3b-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="95c3b-116">Application</span></span>|<span data-ttu-id="95c3b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95c3b-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="95c3b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="95c3b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/connectors/{id}
```
## <a name="request-headers"></a><span data-ttu-id="95c3b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="95c3b-119">Request headers</span></span>
| <span data-ttu-id="95c3b-120">Имя</span><span class="sxs-lookup"><span data-stu-id="95c3b-120">Name</span></span>          | <span data-ttu-id="95c3b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="95c3b-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="95c3b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="95c3b-122">Authorization</span></span> | <span data-ttu-id="95c3b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="95c3b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="95c3b-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="95c3b-125">Request body</span></span>
<span data-ttu-id="95c3b-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="95c3b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="95c3b-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="95c3b-127">Response</span></span>
<span data-ttu-id="95c3b-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="95c3b-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

### <a name="error-conditions-and-messages"></a><span data-ttu-id="95c3b-130">Условия и сообщения об ошибках</span><span class="sxs-lookup"><span data-stu-id="95c3b-130">Error conditions and messages</span></span>

|<span data-ttu-id="95c3b-131">Сценарий</span><span class="sxs-lookup"><span data-stu-id="95c3b-131">Scenario</span></span>|<span data-ttu-id="95c3b-132">Метод</span><span class="sxs-lookup"><span data-stu-id="95c3b-132">Method</span></span>|<span data-ttu-id="95c3b-133">Код</span><span class="sxs-lookup"><span data-stu-id="95c3b-133">Code</span></span>|<span data-ttu-id="95c3b-134">Сообщение</span><span class="sxs-lookup"><span data-stu-id="95c3b-134">Message</span></span>|
|--------|------|----|-------|
|<span data-ttu-id="95c3b-135">Пользователь пытается удалить соединитель с одним или несколькими зарегистрированными принтерами</span><span class="sxs-lookup"><span data-stu-id="95c3b-135">User attempts to delete a connector that has one or more printers registered</span></span>|<span data-ttu-id="95c3b-136">DELETE</span><span class="sxs-lookup"><span data-stu-id="95c3b-136">DELETE</span></span>|<span data-ttu-id="95c3b-137">409</span><span class="sxs-lookup"><span data-stu-id="95c3b-137">409</span></span>|<span data-ttu-id="95c3b-138">Перед удалением соединителя отмените регистрацию связанных принтеров.</span><span class="sxs-lookup"><span data-stu-id="95c3b-138">Before deleting the connector, please unregister the associated printers.</span></span>|

## <a name="example"></a><span data-ttu-id="95c3b-139">Пример</span><span class="sxs-lookup"><span data-stu-id="95c3b-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="95c3b-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="95c3b-140">Request</span></span>
<span data-ttu-id="95c3b-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="95c3b-141">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_connector"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/connectors/{id}
```
##### <a name="response"></a><span data-ttu-id="95c3b-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="95c3b-142">Response</span></span>
<span data-ttu-id="95c3b-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="95c3b-143">The following is an example of the response.</span></span>
><span data-ttu-id="95c3b-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="95c3b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete connector",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->