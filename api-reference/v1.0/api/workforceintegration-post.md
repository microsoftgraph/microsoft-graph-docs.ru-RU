---
title: Создание рабочей силыИнтеграция
description: Создание нового объекта workforceIntegration.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 2eee6b620bcd22e571a2b526d4a43e70fe91416a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055647"
---
# <a name="create-workforceintegration"></a><span data-ttu-id="de262-103">Создание рабочей силыИнтеграция</span><span class="sxs-lookup"><span data-stu-id="de262-103">Create workforceIntegration</span></span>

<span data-ttu-id="de262-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de262-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="de262-105">Создание нового [объекта workforceIntegration.](../resources/workforceintegration.md)</span><span class="sxs-lookup"><span data-stu-id="de262-105">Create a new [workforceIntegration](../resources/workforceintegration.md) object.</span></span>
<span data-ttu-id="de262-106">Можно настроить, для каких сущностям необходимо получать уведомления о синхронных изменениях Shifts, и настроить фильтрацию по правилам WFM, в том числе запросам на обмен.</span><span class="sxs-lookup"><span data-stu-id="de262-106">You can set up which entities you want to receive Shifts synchronous change notifications on and set entities to configure filtering by WFM rules eligibility for, including swap requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="de262-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="de262-107">Permissions</span></span>

<span data-ttu-id="de262-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de262-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="de262-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de262-110">Permission type</span></span>                        | <span data-ttu-id="de262-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="de262-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="de262-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de262-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="de262-113">WorkforceIntegration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de262-113">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="de262-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de262-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de262-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de262-115">Not supported.</span></span> |
| <span data-ttu-id="de262-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="de262-116">Application</span></span>                            | <span data-ttu-id="de262-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de262-117">Not supported.</span></span> |

> <span data-ttu-id="de262-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="de262-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="de262-119">Глобальные администраторы могут получать доступ к группам, в которых они не являются членами.</span><span class="sxs-lookup"><span data-stu-id="de262-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="de262-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de262-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teamwork/workforceIntegrations
```

## <a name="request-headers"></a><span data-ttu-id="de262-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="de262-121">Request headers</span></span>

| <span data-ttu-id="de262-122">Имя</span><span class="sxs-lookup"><span data-stu-id="de262-122">Name</span></span>          | <span data-ttu-id="de262-123">Описание</span><span class="sxs-lookup"><span data-stu-id="de262-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="de262-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="de262-124">Authorization</span></span> | <span data-ttu-id="de262-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="de262-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="de262-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="de262-127">Content-type</span></span> | <span data-ttu-id="de262-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="de262-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="de262-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="de262-130">Request body</span></span>

<span data-ttu-id="de262-131">В теле запроса поставляем представление JSON объекта [workforceIntegration.](../resources/workforceintegration.md)</span><span class="sxs-lookup"><span data-stu-id="de262-131">In the request body, supply a JSON representation of a [workforceIntegration](../resources/workforceintegration.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="de262-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="de262-132">Response</span></span>

<span data-ttu-id="de262-133">В случае успешной работы этот метод возвращает код отклика и новый объект `201 Created` [workforceIntegration](../resources/workforceintegration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="de262-133">If successful, this method returns a `201 Created` response code and a new [workforceIntegration](../resources/workforceintegration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="de262-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="de262-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="de262-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="de262-135">Request</span></span>

<span data-ttu-id="de262-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="de262-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="de262-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="de262-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_workforceintegration_from_teamwork"
}-->

```http
POST https://graph.microsoft.com/v1.0/teamwork/workforceIntegrations
Content-type: application/json

{
  "displayName": "displayName-value",
  "apiVersion": 99,
  "encryption": {
    "protocol": "protocol-value",
    "secret": "secret-value"
  },
  "isActive": true,
  "url": "url-value",
  "supportedEntities": "supportedEntities-value"
}
```
# <a name="c"></a>[<span data-ttu-id="de262-138">C#</span><span class="sxs-lookup"><span data-stu-id="de262-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-workforceintegration-from-teamwork-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="de262-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="de262-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-workforceintegration-from-teamwork-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="de262-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="de262-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-workforceintegration-from-teamwork-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="de262-141">Java</span><span class="sxs-lookup"><span data-stu-id="de262-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-workforceintegration-from-teamwork-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="de262-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="de262-142">Response</span></span>

<span data-ttu-id="de262-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="de262-143">The following is an example of the response.</span></span>

> <span data-ttu-id="de262-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="de262-144">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workforceIntegration"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "displayName": "displayName-value",
  "apiVersion": 99,
  "encryption": {
    "protocol": "protocol-value",
    "secret": "secret-value"
  },
  "isActive": true,
  "url": "url-value",
  "supportedEntities": "supportedEntities-value"
}
```

## <a name="examples-for-use-cases-of-workforceintegration-entity-for-filtering-by-wfm-rules-eligibility"></a><span data-ttu-id="de262-145">Примеры использования случаев использования объекта WorkforceIntegration для фильтрации по правилам WFM</span><span class="sxs-lookup"><span data-stu-id="de262-145">Examples for Use cases of WorkforceIntegration entity for Filtering by WFM rules eligibility</span></span>

### <a name="use-case-create-a-new-workforceintegration-with-swaprequest-enabled-for-eligibility-filtering"></a><span data-ttu-id="de262-146">Пример использования. Создание новой рабочей силы с помощью функции SwapRequest, включенной для фильтрации прав</span><span class="sxs-lookup"><span data-stu-id="de262-146">Use case: Create a new WorkforceIntegration with SwapRequest enabled for eligibility filtering</span></span>

### <a name="request"></a><span data-ttu-id="de262-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="de262-147">Request</span></span>

<span data-ttu-id="de262-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="de262-148">The following is an example of the request.</span></span> 
```
POST https://graph.microsoft.com/v1.0/teamwork/workforceIntegrations/
{
  "displayName": "ABCWorkforceIntegration",
  "apiVersion": 1,
  "isActive": true,
  "encryption": {
    "protocol": "sharedSecret",
    "secret": "My Secret"
  },
  "url": "https://ABCWorkforceIntegration.com/Contoso/",
  "supports": "Shift,SwapRequest",
  "eligibilityFilteringEnabledEntities": "SwapRequest"
}
Authorization: Bearer {token}
Content-type: application/json
```
### <a name="response"></a><span data-ttu-id="de262-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="de262-149">Response</span></span>

<span data-ttu-id="de262-150">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="de262-150">The following is an example of the response.</span></span>
```
HTTP/1.1 200 OK
{
  "id": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "displayName": "ABCWorkforceIntegration",
  "apiVersion": 1,
  "isActive": true,
  "encryption": {
    "protocol": "sharedSecret",
    "secret": null
  },
  "url": "https://abcWorkforceIntegration.com/Contoso/",
  "supports": "Shift,SwapRequest",
  "eligibilityFilteringEnabledEntities": "SwapRequest"
}

```
<span data-ttu-id="de262-151">Узнайте, как обновить существующую рабочую силу с помощью swapRequest, включенной для фильтрации прав, см. в [статью Обновление](../api/workforceintegration-update.md).</span><span class="sxs-lookup"><span data-stu-id="de262-151">To see how to update an existing workforceintegration with SwapRequest enabled for eligibility filtering, see [Update](../api/workforceintegration-update.md).</span></span>

## <a name="example-of-fetching-eligible-shifts-when-swaprequest-is-included-in-eligibilityfilteringenabledentities"></a><span data-ttu-id="de262-152">Пример получения подходящих сдвигов при включении SwapRequest в eligibilityFilteringEnabledEntities</span><span class="sxs-lookup"><span data-stu-id="de262-152">Example of fetching eligible shifts when SwapRequest is included in eligibilityFilteringEnabledEntities</span></span>
<span data-ttu-id="de262-153">Взаимодействие между конечными точками интеграции shifts и рабочей силой будет следовать существующему шаблону.</span><span class="sxs-lookup"><span data-stu-id="de262-153">The interaction between Shifts app and workforce integration endpoints will follow the existing pattern.</span></span>

### <a name="request"></a><span data-ttu-id="de262-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="de262-154">Request</span></span>

<span data-ttu-id="de262-155">Ниже приводится пример запроса shifts to the workforce integration endpoint to fetch eligible shifts for a swap request.</span><span class="sxs-lookup"><span data-stu-id="de262-155">The following is an example of the request made by Shifts to the workforce integration endpoint to fetch eligible shifts for a swap request.</span></span>

```
POST https://abcWorkforceIntegration.com/Contoso/{apiVersion}/team/{teamId}/read
Accept-Language: en-us
{
  "requests": [
  {
     "id": "{shiftId}",
     "method": "GET”,
     "url": “/shifts/{shiftId}/requestableShifts?requestType={requestType}&startDateTime={startDateTime}&endDateTime={endDateTime}”
   }]
}
```
### <a name="response"></a><span data-ttu-id="de262-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="de262-156">Response</span></span>

<span data-ttu-id="de262-157">Ниже приводится пример ответа службы интеграции рабочей силы.</span><span class="sxs-lookup"><span data-stu-id="de262-157">The following is an example of the response from the workforce integration service.</span></span>
```
HTTP/1.1 200 OK
{
  "responses": [
  {
    "body": {
      "SHFT_6548f642-cbc1-4228-8621-054327576457",
      "SHFT_6548f642-cbc1-4228-8621-054327571234"
  }
    "id": "{shiftId}",
    "status: 200,
    "body": {
       "data": [{ShiftId}, {ShiftId}...]
       "error": null
    }
  ]
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create workforceIntegration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

