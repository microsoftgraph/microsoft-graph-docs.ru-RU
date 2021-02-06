---
title: 'synchronization: acquireAccessToken'
description: Получение маркера доступа OAuth для авторизации службы предоставления Azure AD для предоставления пользователям доступа к приложению
author: ArvindHarinder1
localization_priority: Normal
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: da06e05145949a4001600bae87d2322a532544f0
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128248"
---
# <a name="acquireaccesstoken"></a><span data-ttu-id="6369b-103">acquireAccessToken</span><span class="sxs-lookup"><span data-stu-id="6369b-103">acquireAccessToken</span></span>
<span data-ttu-id="6369b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6369b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6369b-105">Получение маркера доступа OAuth для авторизации службы подготовка Azure AD для предоставления пользователей в приложении.</span><span class="sxs-lookup"><span data-stu-id="6369b-105">Acquire an OAuth Access token to authorize the Azure AD provisioning service to provision users into an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="6369b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6369b-106">Permissions</span></span>
<span data-ttu-id="6369b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6369b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6369b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6369b-109">Permission type</span></span>|<span data-ttu-id="6369b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6369b-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6369b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6369b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6369b-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6369b-112">Directory.ReadWrite.All</span></span>|
|<span data-ttu-id="6369b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6369b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6369b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6369b-114">Not supported.</span></span>|
|<span data-ttu-id="6369b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6369b-115">Application</span></span>|<span data-ttu-id="6369b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6369b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6369b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6369b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /applications/{applicationsId}/synchronization/acquireAccessToken
POST /servicePrincipals/{servicePrincipalsId}/synchronization/acquireAccessToken
```

## <a name="request-headers"></a><span data-ttu-id="6369b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6369b-118">Request headers</span></span>
|<span data-ttu-id="6369b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="6369b-119">Name</span></span>|<span data-ttu-id="6369b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6369b-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6369b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6369b-121">Authorization</span></span>|<span data-ttu-id="6369b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6369b-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6369b-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6369b-124">Content-Type</span></span>|<span data-ttu-id="6369b-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6369b-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6369b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6369b-127">Request body</span></span>
<span data-ttu-id="6369b-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6369b-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="6369b-129">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="6369b-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="6369b-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="6369b-130">Parameter</span></span>|<span data-ttu-id="6369b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6369b-131">Type</span></span>|<span data-ttu-id="6369b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6369b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6369b-133">credentials</span><span class="sxs-lookup"><span data-stu-id="6369b-133">credentials</span></span>|<span data-ttu-id="6369b-134">[Коллекция synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="6369b-134">[synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md) collection</span></span>|<span data-ttu-id="6369b-135">Представляет одно значение секрета.</span><span class="sxs-lookup"><span data-stu-id="6369b-135">Represents a single secret value.</span></span>|



## <a name="response"></a><span data-ttu-id="6369b-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="6369b-136">Response</span></span>

<span data-ttu-id="6369b-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6369b-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="6369b-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="6369b-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6369b-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="6369b-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="6369b-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="6369b-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronization_acquireaccesstoken"
}
-->
``` http
POST https://graph.microsoft.com/beta/applications/{applicationsId}/synchronization/acquireAccessToken
Content-Type: application/json
Content-length: 123

{
  "credentials": [
    {
      "@odata.type": "microsoft.graph.synchronizationSecretKeyStringValuePair"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="6369b-141">C#</span><span class="sxs-lookup"><span data-stu-id="6369b-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronization-acquireaccesstoken-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6369b-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6369b-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronization-acquireaccesstoken-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6369b-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6369b-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronization-acquireaccesstoken-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6369b-144">Java</span><span class="sxs-lookup"><span data-stu-id="6369b-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/synchronization-acquireaccesstoken-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="6369b-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="6369b-145">Response</span></span>
<span data-ttu-id="6369b-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6369b-146">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


