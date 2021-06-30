---
title: Удаление cloudPcUserSetting
description: Удаление объекта cloudPcUserSetting.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 6f434d4536eff7361311ad20d2bc17498b700af3
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207853"
---
# <a name="delete-cloudpcusersetting"></a><span data-ttu-id="a8f1b-103">Удаление cloudPcUserSetting</span><span class="sxs-lookup"><span data-stu-id="a8f1b-103">Delete cloudPcUserSetting</span></span>

<span data-ttu-id="a8f1b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8f1b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8f1b-105">Удаление [объекта cloudPcUserSetting.](../resources/cloudpcusersetting.md)</span><span class="sxs-lookup"><span data-stu-id="a8f1b-105">Delete a [cloudPcUserSetting](../resources/cloudpcusersetting.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="permissions"></a><span data-ttu-id="a8f1b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a8f1b-106">Permissions</span></span>

<span data-ttu-id="a8f1b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8f1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8f1b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a8f1b-109">Permission type</span></span>|<span data-ttu-id="a8f1b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a8f1b-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8f1b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a8f1b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a8f1b-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8f1b-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="a8f1b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a8f1b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8f1b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8f1b-114">Not supported.</span></span>|
|<span data-ttu-id="a8f1b-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="a8f1b-115">Application</span></span>|<span data-ttu-id="a8f1b-116">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8f1b-116">CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8f1b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a8f1b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /deviceManagement/virtualEndpoint/userSettings/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a8f1b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a8f1b-118">Request headers</span></span>
|<span data-ttu-id="a8f1b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a8f1b-119">Name</span></span>|<span data-ttu-id="a8f1b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a8f1b-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a8f1b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a8f1b-121">Authorization</span></span>|<span data-ttu-id="a8f1b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a8f1b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8f1b-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a8f1b-124">Request body</span></span>
<span data-ttu-id="a8f1b-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a8f1b-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a8f1b-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8f1b-126">Response</span></span>

<span data-ttu-id="a8f1b-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a8f1b-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="a8f1b-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="a8f1b-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a8f1b-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="a8f1b-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a8f1b-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="a8f1b-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_cloudpcusersetting"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/userSettings/b0c2d35f-3385-46c8-a6f5-6c3dfad7ffff
```
# <a name="c"></a>[<span data-ttu-id="a8f1b-131">C#</span><span class="sxs-lookup"><span data-stu-id="a8f1b-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-cloudpcusersetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a8f1b-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a8f1b-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-cloudpcusersetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a8f1b-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a8f1b-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-cloudpcusersetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a8f1b-134">Java</span><span class="sxs-lookup"><span data-stu-id="a8f1b-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-cloudpcusersetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="a8f1b-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8f1b-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
