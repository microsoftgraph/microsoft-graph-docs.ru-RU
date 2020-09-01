---
title: Добавление identityProvider в b2cUserFlow
description: Добавление identityProvider в b2cUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d873cb83984e9da8e58e377df4ad7257b8f6531c
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319801"
---
# <a name="add-identityprovider-to-a-b2cuserflow"></a><span data-ttu-id="f2553-103">Добавление identityProvider в b2cUserFlow</span><span class="sxs-lookup"><span data-stu-id="f2553-103">Add identityProvider to a b2cUserFlow</span></span>

<span data-ttu-id="f2553-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2553-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2553-105">Добавление поставщиков удостоверений в объект [b2cUserFlow](../resources/b2cuserflows.md) .</span><span class="sxs-lookup"><span data-stu-id="f2553-105">Add identity providers in a [b2cUserFlow](../resources/b2cuserflows.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f2553-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f2553-106">Permissions</span></span>

<span data-ttu-id="f2553-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2553-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2553-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f2553-109">Permission type</span></span>      | <span data-ttu-id="f2553-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f2553-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2553-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f2553-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f2553-112">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f2553-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="f2553-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f2553-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="f2553-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2553-114">Not supported.</span></span>|
|<span data-ttu-id="f2553-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="f2553-115">Application</span></span>| <span data-ttu-id="f2553-116">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f2553-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="f2553-117">Рабочая или учебная учетная запись должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="f2553-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="f2553-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="f2553-118">Global administrator</span></span>
* <span data-ttu-id="f2553-119">Администратор внешнего пользовательского процесса идентификации</span><span class="sxs-lookup"><span data-stu-id="f2553-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="f2553-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f2553-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /b2cUserFlows/{id}/identityProviders/$ref
```

## <a name="request-headers"></a><span data-ttu-id="f2553-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f2553-121">Request headers</span></span>

|<span data-ttu-id="f2553-122">Имя</span><span class="sxs-lookup"><span data-stu-id="f2553-122">Name</span></span>|<span data-ttu-id="f2553-123">Описание</span><span class="sxs-lookup"><span data-stu-id="f2553-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="f2553-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f2553-124">Authorization</span></span>|<span data-ttu-id="f2553-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f2553-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f2553-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f2553-127">Content-Type</span></span>|<span data-ttu-id="f2553-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f2553-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2553-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f2553-130">Request body</span></span>

<span data-ttu-id="f2553-131">В тексте запроса укажите представление объекта IdentityProvider, который требуется добавить, в формате JSON `id` . [identityProvider](../resources/identityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="f2553-131">In the request body, provide a JSON representation of the `id` of the [identityProvider](../resources/identityprovider.md) you want to add.</span></span> <span data-ttu-id="f2553-132">Дополнительные сведения о поставщиках удостоверений, доступных для пользовательских потоков, представлены в справочнике по API [идентитипровидерс](../resources/identityprovider.md) .</span><span class="sxs-lookup"><span data-stu-id="f2553-132">For more information about identity providers available for user flows, see the [identityProviders](../resources/identityprovider.md) API reference.</span></span>

## <a name="response"></a><span data-ttu-id="f2553-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2553-133">Response</span></span>

<span data-ttu-id="f2553-134">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f2553-134">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="f2553-135">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="f2553-135">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="f2553-136">Пример</span><span class="sxs-lookup"><span data-stu-id="f2553-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2553-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="f2553-137">Request</span></span>

<span data-ttu-id="f2553-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f2553-138">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_b2cuserflows_identityprovider"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/identityProviders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/identityProviders/{id}"
}
```

### <a name="response"></a><span data-ttu-id="f2553-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2553-139">Response</span></span>

<span data-ttu-id="f2553-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f2553-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
