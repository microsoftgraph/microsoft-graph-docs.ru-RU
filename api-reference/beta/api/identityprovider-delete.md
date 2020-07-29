---
title: Удаление identityProvider
description: Удаление identityProvider.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c7e1d81f7a8e117bc31f9e827f83cc90bbb8db59
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509765"
---
# <a name="delete-identityprovider"></a><span data-ttu-id="e8da3-103">Удаление identityProvider</span><span class="sxs-lookup"><span data-stu-id="e8da3-103">Delete identityProvider</span></span>

<span data-ttu-id="e8da3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8da3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8da3-105">Удаление [identityProvider](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="e8da3-105">Delete an [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e8da3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e8da3-106">Permissions</span></span>

<span data-ttu-id="e8da3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8da3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8da3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e8da3-109">Permission type</span></span>      | <span data-ttu-id="e8da3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e8da3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8da3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e8da3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e8da3-112">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8da3-112">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="e8da3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e8da3-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="e8da3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8da3-114">Not supported.</span></span>|
|<span data-ttu-id="e8da3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e8da3-115">Application</span></span>|<span data-ttu-id="e8da3-116">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8da3-116">IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="e8da3-117">Рабочая или учебная учетная запись должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="e8da3-117">The work or school account needs to belong to one of the following roles:</span></span>
* <span data-ttu-id="e8da3-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="e8da3-118">Global administrator</span></span>
* <span data-ttu-id="e8da3-119">Администратор внешнего поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="e8da3-119">External Identity Provider administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="e8da3-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e8da3-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e8da3-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e8da3-121">Request headers</span></span>

|<span data-ttu-id="e8da3-122">Имя</span><span class="sxs-lookup"><span data-stu-id="e8da3-122">Name</span></span>|<span data-ttu-id="e8da3-123">Описание</span><span class="sxs-lookup"><span data-stu-id="e8da3-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="e8da3-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e8da3-124">Authorization</span></span>|<span data-ttu-id="e8da3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e8da3-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8da3-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e8da3-127">Request body</span></span>

<span data-ttu-id="e8da3-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e8da3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8da3-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8da3-129">Response</span></span>

<span data-ttu-id="e8da3-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e8da3-130">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e8da3-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e8da3-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8da3-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8da3-132">Request</span></span>

<span data-ttu-id="e8da3-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e8da3-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_identityprovider"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identityProviders/{id}
```


### <a name="response"></a><span data-ttu-id="e8da3-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8da3-134">Response</span></span>

<span data-ttu-id="e8da3-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e8da3-135">The following is an example of the response.</span></span>

<span data-ttu-id="e8da3-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e8da3-136">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
