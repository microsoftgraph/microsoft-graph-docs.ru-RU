---
title: 'cloudPcOnPremisesConnection: updateAdDomainPassword'
description: Обновление пароля домена AD для успешного подключения onPremisesConnection.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: b43179d906d8fa14e961cd097b21a43605576893
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2021
ms.locfileid: "50092325"
---
# <a name="cloudpconpremisesconnection-updateaddomainpassword"></a><span data-ttu-id="0525d-103">cloudPcOnPremisesConnection: updateAdDomainPassword</span><span class="sxs-lookup"><span data-stu-id="0525d-103">cloudPcOnPremisesConnection: updateAdDomainPassword</span></span>
<span data-ttu-id="0525d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0525d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0525d-105">Обновление пароля домена Active Directory для [onPremisesConnection.](../resources/cloudpconpremisesconnection.md)</span><span class="sxs-lookup"><span data-stu-id="0525d-105">Update Active Directory domain password for an [onPremisesConnection](../resources/cloudpconpremisesconnection.md).</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="0525d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0525d-106">Permissions</span></span>
<span data-ttu-id="0525d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0525d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0525d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0525d-109">Permission type</span></span>|<span data-ttu-id="0525d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0525d-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0525d-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0525d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0525d-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0525d-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="0525d-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0525d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0525d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0525d-114">Not supported.</span></span>|
|<span data-ttu-id="0525d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0525d-115">Application</span></span>|<span data-ttu-id="0525d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0525d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0525d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0525d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/virtualEndpoint/onPremisesConnections/{Id}/UpdateAdDomainPassword
```

## <a name="request-headers"></a><span data-ttu-id="0525d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0525d-118">Request headers</span></span>
|<span data-ttu-id="0525d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0525d-119">Name</span></span>|<span data-ttu-id="0525d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0525d-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0525d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0525d-121">Authorization</span></span>|<span data-ttu-id="0525d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0525d-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0525d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0525d-124">Content-Type</span></span>|<span data-ttu-id="0525d-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0525d-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0525d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0525d-127">Request body</span></span>
<span data-ttu-id="0525d-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0525d-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="0525d-129">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="0525d-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="0525d-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="0525d-130">Parameter</span></span>|<span data-ttu-id="0525d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0525d-131">Type</span></span>|<span data-ttu-id="0525d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0525d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0525d-133">adDomainPassword</span><span class="sxs-lookup"><span data-stu-id="0525d-133">adDomainPassword</span></span>|<span data-ttu-id="0525d-134">String</span><span class="sxs-lookup"><span data-stu-id="0525d-134">String</span></span>|<span data-ttu-id="0525d-135">Пароль, связанный с adDomainUsername</span><span class="sxs-lookup"><span data-stu-id="0525d-135">The password associated with adDomainUsername</span></span>|



## <a name="response"></a><span data-ttu-id="0525d-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="0525d-136">Response</span></span>

<span data-ttu-id="0525d-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0525d-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="0525d-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="0525d-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0525d-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="0525d-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="0525d-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="0525d-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "cloudpconpremisesconnection_updateaddomainpassword"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections/{Id}/UpdateAdDomainPassword
Content-Type: application/json
Content-length: 36

{
  "adDomainPassword": "AdDomainPassword value"
}
```
# <a name="javascript"></a>[<span data-ttu-id="0525d-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0525d-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cloudpconpremisesconnection-updateaddomainpassword-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0525d-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0525d-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cloudpconpremisesconnection-updateaddomainpassword-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="0525d-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="0525d-143">Response</span></span>
<span data-ttu-id="0525d-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0525d-144">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
