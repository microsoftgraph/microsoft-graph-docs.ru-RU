---
title: Get userFlowLanguagePage
description: Чтение значений в объекте userFlowLanguagePage для языка в пользовательском потоке.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a772f0df072436d9ff03c83493ec870e6bc5baec
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706416"
---
# <a name="get-userflowlanguagepage"></a><span data-ttu-id="6dc88-103">Get userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="6dc88-103">Get userFlowLanguagePage</span></span>

<span data-ttu-id="6dc88-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6dc88-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6dc88-105">Чтение значений в [объекте userFlowLanguagePage](../resources/userflowlanguagepage.md) для языка в пользовательском потоке.</span><span class="sxs-lookup"><span data-stu-id="6dc88-105">Read the values in a [userFlowLanguagePage](../resources/userflowlanguagepage.md) object for a language in a user flow.</span></span> <span data-ttu-id="6dc88-106">Эти значения показываются пользователю во время пользовательского пути, определенного пользовательским потоком.</span><span class="sxs-lookup"><span data-stu-id="6dc88-106">These values are shown to a user during a user journey defined by a user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="6dc88-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6dc88-107">Permissions</span></span>

<span data-ttu-id="6dc88-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6dc88-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6dc88-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6dc88-110">Permission type</span></span>      | <span data-ttu-id="6dc88-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6dc88-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6dc88-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6dc88-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6dc88-113">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6dc88-113">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="6dc88-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6dc88-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="6dc88-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6dc88-115">Not supported.</span></span>|
|<span data-ttu-id="6dc88-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="6dc88-116">Application</span></span>|<span data-ttu-id="6dc88-117">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6dc88-117">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="6dc88-118">Учетная запись для работы или учебного заведения должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="6dc88-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="6dc88-119">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="6dc88-119">Global administrator</span></span>
* <span data-ttu-id="6dc88-120">Администратор потока пользователей внешнего удостоверения</span><span class="sxs-lookup"><span data-stu-id="6dc88-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="6dc88-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6dc88-121">HTTP request</span></span>

<span data-ttu-id="6dc88-122">Для ссылки на содержимое в объекте необходимо использовать `$value` .</span><span class="sxs-lookup"><span data-stu-id="6dc88-122">To reference the content within the object, you must use `$value`.</span></span> <span data-ttu-id="6dc88-123">Это возвращает содержимое в объекте и позволяет ссылаться на него напрямую.</span><span class="sxs-lookup"><span data-stu-id="6dc88-123">This returns the content within the object and allows you to reference it directly.</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2cUserFlows/{id}/languages/{id}/defaultPages/{id}/$value
GET /identity/b2cUserFlows/{id}/languages/{id}/overridesPages/{id}/$value
GET /identity/b2xUserFlows/{id}/languages/{id}/defaultPages/{id}/$value
GET /identity/b2xUserFlows/{id}/languages/{id}/overridesPages/{id}/$value
```

## <a name="request-headers"></a><span data-ttu-id="6dc88-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6dc88-124">Request headers</span></span>

|<span data-ttu-id="6dc88-125">Имя</span><span class="sxs-lookup"><span data-stu-id="6dc88-125">Name</span></span>|<span data-ttu-id="6dc88-126">Описание</span><span class="sxs-lookup"><span data-stu-id="6dc88-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6dc88-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6dc88-127">Authorization</span></span>|<span data-ttu-id="6dc88-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6dc88-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6dc88-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6dc88-130">Request body</span></span>

<span data-ttu-id="6dc88-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6dc88-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6dc88-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="6dc88-132">Response</span></span>

<span data-ttu-id="6dc88-133">В случае успеха этот метод возвращает код отклика и объект `200 OK` [userFlowLanguagePage](../resources/userflowlanguagepage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6dc88-133">If successful, this method returns a `200 OK` response code and a [userFlowLanguagePage](../resources/userflowlanguagepage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6dc88-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="6dc88-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6dc88-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="6dc88-135">Request</span></span>

<span data-ttu-id="6dc88-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6dc88-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_userflowlanguagepage"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_Customer/languages/en/defaultPages/idpselections/$value
```

### <a name="response"></a><span data-ttu-id="6dc88-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="6dc88-137">Response</span></span>

<span data-ttu-id="6dc88-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6dc88-138">The following is an example of the response.</span></span>

<span data-ttu-id="6dc88-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6dc88-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userFlowLanguagePage"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "LocalizedStrings": [
      {
        "ElementType": "ClaimsProvider",
        "ElementId": null,
        "StringId": "AmazonExchange",
        "Override": false,
        "Value": "Amazon"
      },
      {
        "ElementType": "ClaimsProvider",
        "ElementId": null,
        "StringId": "FacebookExchange",
        "Override": false,
        "Value": "Facebook"
      }
   ]
}
```
