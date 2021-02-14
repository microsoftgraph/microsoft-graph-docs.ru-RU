---
title: 'synchronization: acquireAccessToken'
description: Получение маркера доступа OAuth для авторизации службы предоставления Azure AD для предоставления пользователям доступа к приложению
author: ArvindHarinder1
localization_priority: Normal
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 52933139560b117e0a5311a17907b9037825bd99
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239466"
---
# <a name="acquireaccesstoken"></a><span data-ttu-id="c7cc5-103">acquireAccessToken</span><span class="sxs-lookup"><span data-stu-id="c7cc5-103">acquireAccessToken</span></span>
<span data-ttu-id="c7cc5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7cc5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c7cc5-105">Получение маркера доступа OAuth для авторизации службы подготовка Azure AD для предоставления пользователей в приложении.</span><span class="sxs-lookup"><span data-stu-id="c7cc5-105">Acquire an OAuth Access token to authorize the Azure AD provisioning service to provision users into an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="c7cc5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c7cc5-106">Permissions</span></span>
<span data-ttu-id="c7cc5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7cc5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7cc5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c7cc5-109">Permission type</span></span>|<span data-ttu-id="c7cc5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c7cc5-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7cc5-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c7cc5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c7cc5-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7cc5-112">Directory.ReadWrite.All</span></span>|
|<span data-ttu-id="c7cc5-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c7cc5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7cc5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7cc5-114">Not supported.</span></span>|
|<span data-ttu-id="c7cc5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c7cc5-115">Application</span></span>|<span data-ttu-id="c7cc5-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7cc5-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7cc5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7cc5-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /applications/{applicationsId}/synchronization/acquireAccessToken
POST /servicePrincipals/{servicePrincipalsId}/synchronization/acquireAccessToken
```

## <a name="request-headers"></a><span data-ttu-id="c7cc5-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c7cc5-118">Request headers</span></span>
|<span data-ttu-id="c7cc5-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c7cc5-119">Name</span></span>|<span data-ttu-id="c7cc5-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c7cc5-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c7cc5-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c7cc5-121">Authorization</span></span>|<span data-ttu-id="c7cc5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7cc5-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c7cc5-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c7cc5-124">Content-Type</span></span>|<span data-ttu-id="c7cc5-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7cc5-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7cc5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c7cc5-127">Request body</span></span>
<span data-ttu-id="c7cc5-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c7cc5-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c7cc5-129">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="c7cc5-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c7cc5-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="c7cc5-130">Parameter</span></span>|<span data-ttu-id="c7cc5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c7cc5-131">Type</span></span>|<span data-ttu-id="c7cc5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c7cc5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7cc5-133">credentials</span><span class="sxs-lookup"><span data-stu-id="c7cc5-133">credentials</span></span>|<span data-ttu-id="c7cc5-134">[Коллекция synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="c7cc5-134">[synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md) collection</span></span>|<span data-ttu-id="c7cc5-135">Представляет одно значение секрета.</span><span class="sxs-lookup"><span data-stu-id="c7cc5-135">Represents a single secret value.</span></span>|



## <a name="response"></a><span data-ttu-id="c7cc5-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="c7cc5-136">Response</span></span>

<span data-ttu-id="c7cc5-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c7cc5-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="c7cc5-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="c7cc5-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c7cc5-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7cc5-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c7cc5-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="c7cc5-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c7cc5-141">C#</span><span class="sxs-lookup"><span data-stu-id="c7cc5-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronization-acquireaccesstoken-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c7cc5-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c7cc5-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronization-acquireaccesstoken-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c7cc5-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c7cc5-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronization-acquireaccesstoken-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c7cc5-144">Java</span><span class="sxs-lookup"><span data-stu-id="c7cc5-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/synchronization-acquireaccesstoken-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="c7cc5-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7cc5-145">Response</span></span>
<span data-ttu-id="c7cc5-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c7cc5-146">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


