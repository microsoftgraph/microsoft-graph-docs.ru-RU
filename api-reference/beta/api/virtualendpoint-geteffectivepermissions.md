---
title: 'virtualEndpoint: getEffectivePermissions'
description: '**GetEffectivePermissions — это функция, которая получает эффективные разрешения текущего пользователя, который проходит проверку подлинности, что помогает пользовательскому интерфейсу скрывать или отключать содержимое, к которому у текущего пользователя нет доступа.**'
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 89150ac339a955db1a8d48f3da9e71c3823f9852
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874041"
---
# <a name="virtualendpoint-geteffectivepermissions"></a><span data-ttu-id="294d0-103">virtualEndpoint: getEffectivePermissions</span><span class="sxs-lookup"><span data-stu-id="294d0-103">virtualEndpoint: getEffectivePermissions</span></span>

<span data-ttu-id="294d0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="294d0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="294d0-105">Просмотр эффективных разрешений для пользователя, который в настоящее время проходит проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="294d0-105">View the effective permissions of the currently authenticated user.</span></span> <span data-ttu-id="294d0-106">GetEffectivePermissions — это функция, которая получает эффективные разрешения текущего пользователя, который проходит проверку подлинности, что помогает пользовательскому интерфейсу скрывать или отключать содержимое, к которому у текущего пользователя нет доступа.</span><span class="sxs-lookup"><span data-stu-id="294d0-106">GetEffectivePermissions is a function that retrives the effective permissions of the currently authenticated user, which helps UX hide or disable content that the current user doesn't have access to.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="294d0-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="294d0-107">Permissions</span></span>

<span data-ttu-id="294d0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="294d0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="294d0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="294d0-110">Permission type</span></span>|<span data-ttu-id="294d0-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="294d0-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="294d0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="294d0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="294d0-113">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="294d0-113">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="294d0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="294d0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="294d0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="294d0-115">Not supported.</span></span>|
|<span data-ttu-id="294d0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="294d0-116">Application</span></span>| <span data-ttu-id="294d0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="294d0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="294d0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="294d0-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/getEffectivePermissions
```

## <a name="request-headers"></a><span data-ttu-id="294d0-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="294d0-119">Request headers</span></span>

| <span data-ttu-id="294d0-120">Имя</span><span class="sxs-lookup"><span data-stu-id="294d0-120">Name</span></span>          | <span data-ttu-id="294d0-121">Описание</span><span class="sxs-lookup"><span data-stu-id="294d0-121">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="294d0-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="294d0-122">Authorization</span></span> | <span data-ttu-id="294d0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="294d0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="294d0-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="294d0-125">Request body</span></span>

<span data-ttu-id="294d0-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="294d0-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="294d0-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="294d0-127">Response</span></span>

<span data-ttu-id="294d0-128">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="294d0-128">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span> <span data-ttu-id="294d0-129">Если у пользователя есть полные разрешения, ответ будет `["*"]` .</span><span class="sxs-lookup"><span data-stu-id="294d0-129">If the user has full permissions, the response is `["*"]`.</span></span>

## <a name="examples"></a><span data-ttu-id="294d0-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="294d0-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="294d0-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="294d0-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="294d0-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="294d0-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "virtualendpoint_geteffectivepermissions"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/getEffectivePermissions
```
# <a name="c"></a>[<span data-ttu-id="294d0-133">C#</span><span class="sxs-lookup"><span data-stu-id="294d0-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/virtualendpoint-geteffectivepermissions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="294d0-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="294d0-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/virtualendpoint-geteffectivepermissions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="294d0-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="294d0-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/virtualendpoint-geteffectivepermissions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="294d0-136">Java</span><span class="sxs-lookup"><span data-stu-id="294d0-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/virtualendpoint-geteffectivepermissions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="294d0-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="294d0-137">Response</span></span>

<span data-ttu-id="294d0-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="294d0-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(Edm.String)"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
   "value":[
      "Microsoft.CloudPC/CloudPCs/Read"
   ]
}
```
