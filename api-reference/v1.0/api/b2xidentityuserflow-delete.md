---
title: Удаление b2xIdentityUserFlow
description: Удаление объекта b2xIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: 7742d2243f79e89b0d1df39e247d97ebff940dcb
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51883079"
---
# <a name="delete-b2xidentityuserflow"></a><span data-ttu-id="1cbf3-103">Удаление b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="1cbf3-103">Delete b2xIdentityUserFlow</span></span>

<span data-ttu-id="1cbf3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1cbf3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1cbf3-105">Удаление [объекта b2xIdentityUserFlow.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="1cbf3-105">Delete a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1cbf3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1cbf3-106">Permissions</span></span>

<span data-ttu-id="1cbf3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1cbf3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1cbf3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1cbf3-109">Permission type</span></span>      | <span data-ttu-id="1cbf3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1cbf3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1cbf3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1cbf3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1cbf3-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1cbf3-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="1cbf3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1cbf3-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="1cbf3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1cbf3-114">Not supported.</span></span>|
|<span data-ttu-id="1cbf3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1cbf3-115">Application</span></span>|<span data-ttu-id="1cbf3-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1cbf3-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="1cbf3-117">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="1cbf3-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="1cbf3-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="1cbf3-118">Global administrator</span></span>
* <span data-ttu-id="1cbf3-119">Администратор потока внешних пользователей удостоверений</span><span class="sxs-lookup"><span data-stu-id="1cbf3-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="1cbf3-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1cbf3-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identity/b2xUserFlows/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1cbf3-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1cbf3-121">Request headers</span></span>

|<span data-ttu-id="1cbf3-122">Имя</span><span class="sxs-lookup"><span data-stu-id="1cbf3-122">Name</span></span>|<span data-ttu-id="1cbf3-123">Описание</span><span class="sxs-lookup"><span data-stu-id="1cbf3-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="1cbf3-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1cbf3-124">Authorization</span></span>|<span data-ttu-id="1cbf3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1cbf3-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1cbf3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1cbf3-127">Request body</span></span>

<span data-ttu-id="1cbf3-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1cbf3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1cbf3-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="1cbf3-129">Response</span></span>

<span data-ttu-id="1cbf3-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1cbf3-130">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1cbf3-131">Пример</span><span class="sxs-lookup"><span data-stu-id="1cbf3-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="1cbf3-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1cbf3-132">Request</span></span>

<span data-ttu-id="1cbf3-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1cbf3-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_b2xUserFlows"
}
-->

``` http
DELETE https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_Partner
```

### <a name="response"></a><span data-ttu-id="1cbf3-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="1cbf3-134">Response</span></span>

<span data-ttu-id="1cbf3-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1cbf3-135">The following is an example of the response.</span></span>

<span data-ttu-id="1cbf3-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1cbf3-136">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
