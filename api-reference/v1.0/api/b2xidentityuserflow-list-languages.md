---
title: Перечисление языков
description: Извлечение списка языков, поддерживаемых для настройки в потоке пользователей B2X.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 8458bff2364c9d8f5ac9fa084f72dcd57681a90c
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51883371"
---
# <a name="list-languages"></a><span data-ttu-id="ffa2e-103">Перечисление языков</span><span class="sxs-lookup"><span data-stu-id="ffa2e-103">List languages</span></span>

<span data-ttu-id="ffa2e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ffa2e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ffa2e-105">Извлечение списка языков, поддерживаемых для настройки в потоке пользователей B2X.</span><span class="sxs-lookup"><span data-stu-id="ffa2e-105">Retrieve a list of languages supported for customization in a B2X user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="ffa2e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ffa2e-106">Permissions</span></span>

<span data-ttu-id="ffa2e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ffa2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ffa2e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ffa2e-109">Permission type</span></span>      | <span data-ttu-id="ffa2e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ffa2e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ffa2e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ffa2e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ffa2e-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffa2e-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="ffa2e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ffa2e-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="ffa2e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ffa2e-114">Not supported.</span></span>|
|<span data-ttu-id="ffa2e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ffa2e-115">Application</span></span>|<span data-ttu-id="ffa2e-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffa2e-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="ffa2e-117">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="ffa2e-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="ffa2e-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="ffa2e-118">Global administrator</span></span>
* <span data-ttu-id="ffa2e-119">Администратор потока внешних пользователей удостоверений</span><span class="sxs-lookup"><span data-stu-id="ffa2e-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="ffa2e-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ffa2e-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2xUserFlows/{id}/languages
```

## <a name="request-headers"></a><span data-ttu-id="ffa2e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ffa2e-121">Request headers</span></span>

|<span data-ttu-id="ffa2e-122">Имя</span><span class="sxs-lookup"><span data-stu-id="ffa2e-122">Name</span></span>|<span data-ttu-id="ffa2e-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ffa2e-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ffa2e-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ffa2e-124">Authorization</span></span>|<span data-ttu-id="ffa2e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ffa2e-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ffa2e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ffa2e-127">Request body</span></span>

<span data-ttu-id="ffa2e-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ffa2e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ffa2e-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ffa2e-129">Response</span></span>

<span data-ttu-id="ffa2e-130">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ffa2e-130">If successful, this method returns a `200 OK` response code and a collection of [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ffa2e-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="ffa2e-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ffa2e-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ffa2e-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_userflowlanguageconfiguration_2"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_PartnerSignUp/languages
```

### <a name="response"></a><span data-ttu-id="ffa2e-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="ffa2e-133">Response</span></span>

<span data-ttu-id="ffa2e-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ffa2e-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.userFlowLanguageConfiguration)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/b2xUserFlows('B2X_1_PartnerSignUp')/languages",
  "value": [
    {
      "id": "en",
      "isEnabled": true,
      "displayName": "English"
    },
    {
      "id": "de",
      "isEnabled": true,
      "displayName": "Deutsch"
    }
  ]
}
```
