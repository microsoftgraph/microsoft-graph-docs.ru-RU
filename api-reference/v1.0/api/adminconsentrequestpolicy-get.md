---
title: Получить adminConsentRequestPolicy
description: Ознакомьтесь с свойствами и отношениями объекта adminConsentRequestPolicy.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: f9a6d19c1671265034ca5f2663ab55aa701eeda8
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469660"
---
# <a name="get-adminconsentrequestpolicy"></a><span data-ttu-id="94747-103">Получить adminConsentRequestPolicy</span><span class="sxs-lookup"><span data-stu-id="94747-103">Get adminConsentRequestPolicy</span></span>

<span data-ttu-id="94747-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94747-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="94747-105">Ознакомьтесь с свойствами и отношениями объекта [adminConsentRequestPolicy.](../resources/adminconsentrequestpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="94747-105">Read the properties and relationships of an [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="94747-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="94747-106">Permissions</span></span>

<span data-ttu-id="94747-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94747-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94747-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="94747-109">Permission type</span></span>|<span data-ttu-id="94747-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="94747-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="94747-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="94747-111">Delegated (work or school account)</span></span>|<span data-ttu-id="94747-112">Policy.Read.All, Policy.ReadWrite.ConsentRequest, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94747-112">Policy.Read.All, Policy.ReadWrite.ConsentRequest, Directory.Read.All, Directory.ReadWrite.All</span></span>|
|<span data-ttu-id="94747-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="94747-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94747-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94747-114">Not supported.</span></span>|
|<span data-ttu-id="94747-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="94747-115">Application</span></span>|<span data-ttu-id="94747-116">Policy.Read.All, Policy.ReadWrite.ConsentRequest, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94747-116">Policy.Read.All, Policy.ReadWrite.ConsentRequest, Directory.Read.All, Directory.ReadWrite.All</span></span>|

<span data-ttu-id="94747-117">При вызове от имени пользователя пользователю необходимо принадлежать к одной из следующих ролей каталога.</span><span class="sxs-lookup"><span data-stu-id="94747-117">When calling on behalf of a user, the user needs to belong to one of the following directory roles.</span></span> <span data-ttu-id="94747-118">Дополнительные информацию о роли каталогов см. в встроенной роли [Azure AD:](/azure/active-directory/roles/permissions-reference)</span><span class="sxs-lookup"><span data-stu-id="94747-118">To learn more about directory roles, see [Azure AD built-in roles](/azure/active-directory/roles/permissions-reference):</span></span>
+ <span data-ttu-id="94747-119">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="94747-119">Global Administrator</span></span>
+ <span data-ttu-id="94747-120">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="94747-120">Global Reader</span></span>
+ <span data-ttu-id="94747-121">Администратор облачного приложения</span><span class="sxs-lookup"><span data-stu-id="94747-121">Cloud Application Administrator</span></span>
+ <span data-ttu-id="94747-122">Администратор приложения</span><span class="sxs-lookup"><span data-stu-id="94747-122">Application Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="94747-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="94747-123">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/adminConsentRequestPolicy
```

## <a name="optional-query-parameters"></a><span data-ttu-id="94747-124">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="94747-124">Optional query parameters</span></span>

<span data-ttu-id="94747-125">Этот метод поддерживает параметр  `$select`   запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="94747-125">This method supports the `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="94747-126">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="94747-126">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="94747-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="94747-127">Request headers</span></span>

|<span data-ttu-id="94747-128">Имя</span><span class="sxs-lookup"><span data-stu-id="94747-128">Name</span></span>|<span data-ttu-id="94747-129">Описание</span><span class="sxs-lookup"><span data-stu-id="94747-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="94747-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="94747-130">Authorization</span></span>|<span data-ttu-id="94747-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="94747-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="94747-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="94747-133">Request body</span></span>

<span data-ttu-id="94747-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="94747-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94747-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="94747-135">Response</span></span>

<span data-ttu-id="94747-136">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="94747-136">If successful, this method returns a `200 OK` response code and an [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="94747-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="94747-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="94747-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="94747-138">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_adminconsentrequestpolicy"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/policies/adminConsentRequestPolicy
```

### <a name="response"></a><span data-ttu-id="94747-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="94747-139">Response</span></span>

<span data-ttu-id="94747-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="94747-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.adminConsentRequestPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#policies/adminConsentRequestPolicy/$entity",
  "isEnabled": true,
  "notifyReviewers": false,
  "remindersEnabled": false,
  "requestDurationInDays": 0,
  "version": 0,
  "reviewers": [
    {
      "query": "/users/906e0ee5-6372-4cc8-8248-fdf2846b48ed",
      "queryType": "MicrosoftGraph",
      "queryRoot": null
    },
    {
      "query": "/users/daddef1a-acb0-4f62-96d0-49df2495d657",
      "queryType": "MicrosoftGraph",
      "queryRoot": null
    }
  ]
}
```
