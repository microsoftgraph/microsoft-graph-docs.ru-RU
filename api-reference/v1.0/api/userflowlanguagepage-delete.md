---
title: Удаление userFlowLanguagePage
description: Удаляет значения в объекте userFlowLanguagePage.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 791c43817d9a8f8e8369e4d0d8adf5eb0a75580a
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51883350"
---
# <a name="delete-userflowlanguagepage"></a><span data-ttu-id="0543f-103">Удаление userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="0543f-103">Delete userFlowLanguagePage</span></span>

<span data-ttu-id="0543f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0543f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0543f-105">Удаляет значения в [объекте userFlowLanguagePage.](../resources/userflowlanguagepage.md)</span><span class="sxs-lookup"><span data-stu-id="0543f-105">Deletes the values in an [userFlowLanguagePage](../resources/userflowlanguagepage.md) object.</span></span> <span data-ttu-id="0543f-106">Можно удалить только значения в переопределеченной странице, которая используется для настройки значений, показанных пользователю во время пользовательского пути, определенного потоком пользователей.</span><span class="sxs-lookup"><span data-stu-id="0543f-106">You may only delete the values in an overridesPage, which is used to customize the values shown to a user during a user journey defined by a user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="0543f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0543f-107">Permissions</span></span>

<span data-ttu-id="0543f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0543f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0543f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0543f-110">Permission type</span></span>      | <span data-ttu-id="0543f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0543f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0543f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0543f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0543f-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0543f-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="0543f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0543f-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="0543f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0543f-115">Not supported.</span></span>|
|<span data-ttu-id="0543f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0543f-116">Application</span></span>|<span data-ttu-id="0543f-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0543f-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="0543f-118">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="0543f-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="0543f-119">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="0543f-119">Global administrator</span></span>
* <span data-ttu-id="0543f-120">Администратор потока внешних пользователей удостоверений</span><span class="sxs-lookup"><span data-stu-id="0543f-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="0543f-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0543f-121">HTTP request</span></span>

<span data-ttu-id="0543f-122">Чтобы ссылаться на содержимое объекта, необходимо использовать `$value` .</span><span class="sxs-lookup"><span data-stu-id="0543f-122">To reference the content within the object, you must use `$value`.</span></span> <span data-ttu-id="0543f-123">Это возвращает содержимое объекта и позволяет ссылаться на него напрямую.</span><span class="sxs-lookup"><span data-stu-id="0543f-123">This returns the content within the object and allows you to reference it directly.</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /identity/b2xUserFlows/{id}/languages/{id}/overridesPages/$value
```

## <a name="request-headers"></a><span data-ttu-id="0543f-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0543f-124">Request headers</span></span>

|<span data-ttu-id="0543f-125">Имя</span><span class="sxs-lookup"><span data-stu-id="0543f-125">Name</span></span>|<span data-ttu-id="0543f-126">Описание</span><span class="sxs-lookup"><span data-stu-id="0543f-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0543f-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0543f-127">Authorization</span></span>|<span data-ttu-id="0543f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0543f-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0543f-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0543f-130">Request body</span></span>

<span data-ttu-id="0543f-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0543f-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0543f-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="0543f-132">Response</span></span>

<span data-ttu-id="0543f-133">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0543f-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="0543f-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="0543f-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0543f-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="0543f-135">Request</span></span>

<span data-ttu-id="0543f-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0543f-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_userflowlanguagepage"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2cUserFlows/B2X_1_Partner/languages/en/overridesPages/selfasserted1_1/$value
```

### <a name="response"></a><span data-ttu-id="0543f-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="0543f-137">Response</span></span>

<span data-ttu-id="0543f-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0543f-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
