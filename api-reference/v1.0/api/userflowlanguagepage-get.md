---
title: Get userFlowLanguagePage
description: Чтение значений в объекте userFlowLanguagePage для языка в потоке пользователей.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 5b1edf34635e94a3bb45500df34309c7ba1fac59
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51883347"
---
# <a name="get-userflowlanguagepage"></a><span data-ttu-id="0600a-103">Get userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="0600a-103">Get userFlowLanguagePage</span></span>

<span data-ttu-id="0600a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0600a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0600a-105">Чтение значений в [объекте userFlowLanguagePage](../resources/userflowlanguagepage.md) для языка в потоке пользователей.</span><span class="sxs-lookup"><span data-stu-id="0600a-105">Read the values in a [userFlowLanguagePage](../resources/userflowlanguagepage.md) object for a language in a user flow.</span></span> <span data-ttu-id="0600a-106">Эти значения показаны пользователю во время путешествия пользователя, определенного потоком пользователей.</span><span class="sxs-lookup"><span data-stu-id="0600a-106">These values are shown to a user during a user journey defined by a user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="0600a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0600a-107">Permissions</span></span>

<span data-ttu-id="0600a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0600a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0600a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0600a-110">Permission type</span></span>      | <span data-ttu-id="0600a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0600a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0600a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0600a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0600a-113">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0600a-113">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="0600a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0600a-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="0600a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0600a-115">Not supported.</span></span>|
|<span data-ttu-id="0600a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0600a-116">Application</span></span>|<span data-ttu-id="0600a-117">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0600a-117">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="0600a-118">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="0600a-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="0600a-119">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="0600a-119">Global administrator</span></span>
* <span data-ttu-id="0600a-120">Администратор потока внешних пользователей удостоверений</span><span class="sxs-lookup"><span data-stu-id="0600a-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="0600a-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0600a-121">HTTP request</span></span>

<span data-ttu-id="0600a-122">Чтобы ссылаться на содержимое объекта, необходимо использовать `$value` .</span><span class="sxs-lookup"><span data-stu-id="0600a-122">To reference the content within the object, you must use `$value`.</span></span> <span data-ttu-id="0600a-123">Это возвращает содержимое объекта и позволяет ссылаться на него напрямую.</span><span class="sxs-lookup"><span data-stu-id="0600a-123">This returns the content within the object and allows you to reference it directly.</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2xUserFlows/{id}/languages/{id}/defaultPages/{id}/$value
GET /identity/b2xUserFlows/{id}/languages/{id}/overridesPages/{id}/$value
```

## <a name="request-headers"></a><span data-ttu-id="0600a-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0600a-124">Request headers</span></span>

|<span data-ttu-id="0600a-125">Имя</span><span class="sxs-lookup"><span data-stu-id="0600a-125">Name</span></span>|<span data-ttu-id="0600a-126">Описание</span><span class="sxs-lookup"><span data-stu-id="0600a-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0600a-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0600a-127">Authorization</span></span>|<span data-ttu-id="0600a-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0600a-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0600a-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0600a-130">Request body</span></span>

<span data-ttu-id="0600a-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0600a-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0600a-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="0600a-132">Response</span></span>

<span data-ttu-id="0600a-133">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект userFlowLanguagePage](../resources/userflowlanguagepage.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="0600a-133">If successful, this method returns a `200 OK` response code and a [userFlowLanguagePage](../resources/userflowlanguagepage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0600a-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="0600a-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0600a-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="0600a-135">Request</span></span>

<span data-ttu-id="0600a-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0600a-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_userflowlanguagepage_3"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_Partner/languages/en/defaultPages/idpselections/$value
```

### <a name="response"></a><span data-ttu-id="0600a-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="0600a-137">Response</span></span>

<span data-ttu-id="0600a-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0600a-138">The following is an example of the response.</span></span>

<span data-ttu-id="0600a-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0600a-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
        "ElementType": "ErrorMessage",
        "ElementId": null,
        "StringId": "ServiceThrottled",
        "Override": false,
        "Value": "There are too many requests at this moment. Please wait for some time and try again."
      }
   ]
}
```
