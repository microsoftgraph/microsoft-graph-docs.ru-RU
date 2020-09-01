---
title: Удаление b2xUserFlow
description: Удаление объекта b2xUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2e408c96d70efc04168954cbe82448a9e6a71cd1
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319805"
---
# <a name="delete-b2xuserflow"></a><span data-ttu-id="ce3e5-103">Удаление b2xUserFlow</span><span class="sxs-lookup"><span data-stu-id="ce3e5-103">Delete b2xUserFlow</span></span>

<span data-ttu-id="ce3e5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce3e5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce3e5-105">Удаление объекта [b2xUserFlow](../resources/b2xuserflows.md) .</span><span class="sxs-lookup"><span data-stu-id="ce3e5-105">Delete a [b2xUserFlow](../resources/b2xuserflows.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ce3e5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ce3e5-106">Permissions</span></span>

<span data-ttu-id="ce3e5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce3e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce3e5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ce3e5-109">Permission type</span></span>      | <span data-ttu-id="ce3e5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ce3e5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce3e5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ce3e5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ce3e5-112">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ce3e5-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="ce3e5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ce3e5-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="ce3e5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce3e5-114">Not supported.</span></span>|
|<span data-ttu-id="ce3e5-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="ce3e5-115">Application</span></span>|<span data-ttu-id="ce3e5-116">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ce3e5-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="ce3e5-117">Рабочая или учебная учетная запись должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="ce3e5-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="ce3e5-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="ce3e5-118">Global administrator</span></span>
* <span data-ttu-id="ce3e5-119">Администратор внешнего пользовательского процесса идентификации</span><span class="sxs-lookup"><span data-stu-id="ce3e5-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="ce3e5-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ce3e5-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identity/b2xUserFlows/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ce3e5-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ce3e5-121">Request headers</span></span>

|<span data-ttu-id="ce3e5-122">Имя</span><span class="sxs-lookup"><span data-stu-id="ce3e5-122">Name</span></span>|<span data-ttu-id="ce3e5-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ce3e5-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="ce3e5-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ce3e5-124">Authorization</span></span>|<span data-ttu-id="ce3e5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ce3e5-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce3e5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ce3e5-127">Request body</span></span>

<span data-ttu-id="ce3e5-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ce3e5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce3e5-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce3e5-129">Response</span></span>

<span data-ttu-id="ce3e5-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ce3e5-130">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ce3e5-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ce3e5-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ce3e5-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ce3e5-132">Request</span></span>

<span data-ttu-id="ce3e5-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ce3e5-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_b2xUserFlows"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2xUserFlows/{id}
```

### <a name="response"></a><span data-ttu-id="ce3e5-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce3e5-134">Response</span></span>

<span data-ttu-id="ce3e5-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ce3e5-135">The following is an example of the response.</span></span>

<span data-ttu-id="ce3e5-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ce3e5-136">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
