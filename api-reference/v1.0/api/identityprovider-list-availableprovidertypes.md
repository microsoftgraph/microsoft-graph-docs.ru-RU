---
title: Список доступныхProviderTypes
description: Извлечение всех доступных типов поставщика удостоверений в каталоге.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 6c7c2189db2d4f1ffcca093bac6dc1a9a127c85e
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51883339"
---
# <a name="list-availableprovidertypes"></a><span data-ttu-id="817f9-103">Список доступныхProviderTypes</span><span class="sxs-lookup"><span data-stu-id="817f9-103">List availableProviderTypes</span></span>

<span data-ttu-id="817f9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="817f9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="817f9-105">Извлекает все типы поставщиков удостоверений, доступные в каталоге.</span><span class="sxs-lookup"><span data-stu-id="817f9-105">Retrieves all identity provider types available in a directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="817f9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="817f9-106">Permissions</span></span>

<span data-ttu-id="817f9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="817f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="817f9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="817f9-109">Permission type</span></span>      | <span data-ttu-id="817f9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="817f9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="817f9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="817f9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="817f9-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="817f9-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="817f9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="817f9-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="817f9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="817f9-114">Not supported.</span></span>|
|<span data-ttu-id="817f9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="817f9-115">Application</span></span>|<span data-ttu-id="817f9-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="817f9-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="817f9-117">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="817f9-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="817f9-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="817f9-118">Global Administrator</span></span>
* <span data-ttu-id="817f9-119">Администратор внешнего поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="817f9-119">External Identity Provider Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="817f9-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="817f9-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityProviders/availableProviderTypes
```

## <a name="request-headers"></a><span data-ttu-id="817f9-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="817f9-121">Request headers</span></span>

|<span data-ttu-id="817f9-122">Имя</span><span class="sxs-lookup"><span data-stu-id="817f9-122">Name</span></span>|<span data-ttu-id="817f9-123">Описание</span><span class="sxs-lookup"><span data-stu-id="817f9-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="817f9-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="817f9-124">Authorization</span></span>|<span data-ttu-id="817f9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="817f9-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="817f9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="817f9-127">Request body</span></span>

<span data-ttu-id="817f9-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="817f9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="817f9-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="817f9-129">Response</span></span>

<span data-ttu-id="817f9-130">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="817f9-130">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="817f9-131">Пример</span><span class="sxs-lookup"><span data-stu-id="817f9-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="817f9-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="817f9-132">Request</span></span>

<span data-ttu-id="817f9-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="817f9-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "identityprovider_availableprovidertypes"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identityProviders/availableProviderTypes
```

### <a name="response"></a><span data-ttu-id="817f9-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="817f9-134">Response</span></span>

<span data-ttu-id="817f9-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="817f9-135">The following is an example of the response.</span></span>

<span data-ttu-id="817f9-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="817f9-136">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(Edm.String)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
      "Google",
      "Facebook",
      "MicrosoftAccount",
      "EmailOTP"
  ]
}
```
