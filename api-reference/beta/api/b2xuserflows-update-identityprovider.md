---
title: Добавление identityProvider в b2xUserFlow
description: Добавление identityProvider в b2xUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a05bb5a1e45c9f6ff9c2297cabfe527b746199f6
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319802"
---
# <a name="add-identityprovider-to-a-b2xuserflow"></a><span data-ttu-id="94666-103">Добавление identityProvider в b2xUserFlow</span><span class="sxs-lookup"><span data-stu-id="94666-103">Add identityProvider to a b2xUserFlow</span></span>

<span data-ttu-id="94666-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94666-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94666-105">Обновление поставщиков удостоверений в объекте [b2xUserFlow](../resources/b2xuserflows.md) .</span><span class="sxs-lookup"><span data-stu-id="94666-105">Update the identity providers in a [b2xUserFlow](../resources/b2xuserflows.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="94666-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="94666-106">Permissions</span></span>

<span data-ttu-id="94666-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94666-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94666-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="94666-109">Permission type</span></span>      | <span data-ttu-id="94666-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="94666-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94666-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="94666-111">Delegated (work or school account)</span></span>|<span data-ttu-id="94666-112">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="94666-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="94666-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="94666-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="94666-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94666-114">Not supported.</span></span>|
|<span data-ttu-id="94666-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="94666-115">Application</span></span>| <span data-ttu-id="94666-116">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="94666-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="94666-117">Рабочая или учебная учетная запись должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="94666-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="94666-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="94666-118">Global administrator</span></span>
* <span data-ttu-id="94666-119">Администратор внешнего пользовательского процесса идентификации</span><span class="sxs-lookup"><span data-stu-id="94666-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="94666-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="94666-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /b2xUserFlows/{id}/identityProviders/$ref
```

## <a name="request-headers"></a><span data-ttu-id="94666-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="94666-121">Request headers</span></span>

|<span data-ttu-id="94666-122">Имя</span><span class="sxs-lookup"><span data-stu-id="94666-122">Name</span></span>|<span data-ttu-id="94666-123">Описание</span><span class="sxs-lookup"><span data-stu-id="94666-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="94666-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="94666-124">Authorization</span></span>|<span data-ttu-id="94666-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="94666-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="94666-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="94666-127">Content-Type</span></span>|<span data-ttu-id="94666-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="94666-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="94666-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="94666-130">Request body</span></span>

<span data-ttu-id="94666-131">В тексте запроса укажите представление объекта IdentityProvider, который требуется добавить, в формате JSON `id` . [identityProvider](../resources/identityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="94666-131">In the request body, provide a JSON representation of the `id` of the [identityProvider](../resources/identityprovider.md) you want to add.</span></span> <span data-ttu-id="94666-132">Для самостоятельной регистрации пользовательских потоков значения могут быть `Google-OAUTH` или `Facebook-OAUTH` .</span><span class="sxs-lookup"><span data-stu-id="94666-132">For self-service sign up user flows, the values can be `Google-OAUTH` or `Facebook-OAUTH`.</span></span>

## <a name="response"></a><span data-ttu-id="94666-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="94666-133">Response</span></span>

<span data-ttu-id="94666-134">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="94666-134">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="94666-135">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="94666-135">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="94666-136">Пример</span><span class="sxs-lookup"><span data-stu-id="94666-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="94666-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="94666-137">Request</span></span>

<span data-ttu-id="94666-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="94666-138">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_b2xuserflows_identityprovider"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/b2xUserFlows/{id}/identityProviders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/identityProviders/{id}"
}
```

### <a name="response"></a><span data-ttu-id="94666-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="94666-139">Response</span></span>

<span data-ttu-id="94666-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="94666-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
