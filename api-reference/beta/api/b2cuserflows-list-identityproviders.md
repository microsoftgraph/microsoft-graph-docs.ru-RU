---
title: Перечисление всех Идентитипровидерс в b2cUserFlow
description: Перечисление всех Идентитипровидерс в b2cUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 450a3465a70a2a8e09acf28fbcafb6a81e9f275f
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319816"
---
# <a name="list-all-identityproviders-in-a-b2cuserflow"></a><span data-ttu-id="323ed-103">Перечисление всех Идентитипровидерс в b2cUserFlow</span><span class="sxs-lookup"><span data-stu-id="323ed-103">List all identityProviders in a b2cUserFlow</span></span>

<span data-ttu-id="323ed-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="323ed-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="323ed-105">Получение поставщиков удостоверений в объекте [b2cUserFlow](../resources/b2cuserflows.md)</span><span class="sxs-lookup"><span data-stu-id="323ed-105">Get the identity providers in a [b2cUserFlow](../resources/b2cuserflows.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="323ed-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="323ed-106">Permissions</span></span>

<span data-ttu-id="323ed-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="323ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="323ed-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="323ed-109">Permission type</span></span>      | <span data-ttu-id="323ed-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="323ed-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="323ed-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="323ed-111">Delegated (work or school account)</span></span>|<span data-ttu-id="323ed-112">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="323ed-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="323ed-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="323ed-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="323ed-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="323ed-114">Not supported.</span></span>|
|<span data-ttu-id="323ed-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="323ed-115">Application</span></span>| <span data-ttu-id="323ed-116">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="323ed-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="323ed-117">Рабочая или учебная учетная запись должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="323ed-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="323ed-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="323ed-118">Global administrator</span></span>
* <span data-ttu-id="323ed-119">Администратор внешнего пользовательского процесса идентификации</span><span class="sxs-lookup"><span data-stu-id="323ed-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="323ed-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="323ed-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /b2cUserFlows/{id}/identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="323ed-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="323ed-121">Request headers</span></span>

|<span data-ttu-id="323ed-122">Имя</span><span class="sxs-lookup"><span data-stu-id="323ed-122">Name</span></span>|<span data-ttu-id="323ed-123">Описание</span><span class="sxs-lookup"><span data-stu-id="323ed-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="323ed-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="323ed-124">Authorization</span></span>|<span data-ttu-id="323ed-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="323ed-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="323ed-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="323ed-127">Request body</span></span>

<span data-ttu-id="323ed-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="323ed-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="323ed-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="323ed-129">Response</span></span>

<span data-ttu-id="323ed-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и представление объекта [идентитипровидерс](../resources/identityprovider.md) в тексте отклика в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="323ed-130">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityProviders](../resources/identityprovider.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="323ed-131">Пример</span><span class="sxs-lookup"><span data-stu-id="323ed-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="323ed-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="323ed-132">Request</span></span>

<span data-ttu-id="323ed-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="323ed-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_b2cUserFlow_list_identityProviders"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/identityProviders
```

### <a name="response"></a><span data-ttu-id="323ed-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="323ed-134">Response</span></span>

<span data-ttu-id="323ed-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="323ed-135">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityProvider"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "Facebook-OAuth",
            "type": "Facebook",
            "name": "Facebook",
            "clientId": "clientIdFromFacebook",
            "clientSecret": "*****"
        },
        {
            "id": "Google-OAuth",
            "type": "Google",
            "name": "Google",
            "clientId": "clientIdFromGoogle",
            "clientSecret": "*****"
        }
    ]
}
```
