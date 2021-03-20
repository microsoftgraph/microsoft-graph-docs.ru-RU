---
title: Получить adminConsentRequestPolicy
description: Ознакомьтесь с свойствами и отношениями объекта adminConsentRequestPolicy.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 2867e880bd6e0eb155681986d615d274383241b4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952310"
---
# <a name="get-adminconsentrequestpolicy"></a><span data-ttu-id="ff038-103">Получить adminConsentRequestPolicy</span><span class="sxs-lookup"><span data-stu-id="ff038-103">Get adminConsentRequestPolicy</span></span>
<span data-ttu-id="ff038-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff038-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff038-105">Ознакомьтесь с свойствами и отношениями объекта [adminConsentRequestPolicy.](../resources/adminconsentrequestpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ff038-105">Read the properties and relationships of an [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ff038-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ff038-106">Permissions</span></span>
<span data-ttu-id="ff038-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff038-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff038-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ff038-109">Permission type</span></span>|<span data-ttu-id="ff038-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ff038-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff038-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ff038-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ff038-112">Policy.Read.All, Policy.ReadWrite.ConsentRequest</span><span class="sxs-lookup"><span data-stu-id="ff038-112">Policy.Read.All, Policy.ReadWrite.ConsentRequest</span></span>|
|<span data-ttu-id="ff038-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ff038-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff038-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff038-114">Not supported.</span></span>|
|<span data-ttu-id="ff038-115">Application</span><span class="sxs-lookup"><span data-stu-id="ff038-115">Application</span></span>|<span data-ttu-id="ff038-116">Policy.Read.All, Policy.ReadWrite.ConsentRequest</span><span class="sxs-lookup"><span data-stu-id="ff038-116">Policy.Read.All, Policy.ReadWrite.ConsentRequest</span></span>|

<span data-ttu-id="ff038-117">При вызове от имени пользователя пользователю необходимо принадлежать к одной из следующих ролей каталога.</span><span class="sxs-lookup"><span data-stu-id="ff038-117">When calling on behalf of a user, the user needs to belong to one of the following directory roles.</span></span> <span data-ttu-id="ff038-118">Дополнительные информацию о роли каталогов см. в встроенной роли [Azure AD:](/azure/active-directory/roles/permissions-reference)</span><span class="sxs-lookup"><span data-stu-id="ff038-118">To learn more about directory roles, see [Azure AD built-in roles](/azure/active-directory/roles/permissions-reference):</span></span>
+ <span data-ttu-id="ff038-119">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="ff038-119">Global Administrator</span></span>
+ <span data-ttu-id="ff038-120">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="ff038-120">Global Reader</span></span>
+ <span data-ttu-id="ff038-121">Администратор облачного приложения</span><span class="sxs-lookup"><span data-stu-id="ff038-121">Cloud Application Administrator</span></span>
+ <span data-ttu-id="ff038-122">Администратор приложения</span><span class="sxs-lookup"><span data-stu-id="ff038-122">Application Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="ff038-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ff038-123">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/adminConsentRequestPolicy
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ff038-124">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ff038-124">Optional query parameters</span></span>
<span data-ttu-id="ff038-125">Этот метод поддерживает параметр  `$select`   запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ff038-125">This method supports the `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="ff038-126">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ff038-126">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ff038-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ff038-127">Request headers</span></span>
|<span data-ttu-id="ff038-128">Имя</span><span class="sxs-lookup"><span data-stu-id="ff038-128">Name</span></span>|<span data-ttu-id="ff038-129">Описание</span><span class="sxs-lookup"><span data-stu-id="ff038-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ff038-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ff038-130">Authorization</span></span>|<span data-ttu-id="ff038-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ff038-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff038-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ff038-133">Request body</span></span>
<span data-ttu-id="ff038-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ff038-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff038-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff038-135">Response</span></span>

<span data-ttu-id="ff038-136">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ff038-136">If successful, this method returns a `200 OK` response code and an [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ff038-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="ff038-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ff038-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="ff038-138">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_adminconsentrequestpolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/adminConsentRequestPolicy
```


### <a name="response"></a><span data-ttu-id="ff038-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff038-139">Response</span></span>
<span data-ttu-id="ff038-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ff038-140">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#policies/adminConsentRequestPolicy/$entity",
  "isEnabled": false,
  "notifyReviewers": false,
  "remindersEnabled": false,
  "requestDurationInDays": 0,
  "version": 0,
  "reviewers": []
}
```
