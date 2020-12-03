---
title: 'Виртуалендпоинт: getEffectivePermissions'
description: '**GetEffectivePermissions — это функция, которая ретривес действующие разрешения пользователя, прошедшего проверку подлинности, что позволяет скрыть или отключить контент, к которому у текущего пользователя нет доступа.**'
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: df6d0ffbdffdf01c30f5dda2220cc96392b0f6ed
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563914"
---
# <a name="virtualendpoint-geteffectivepermissions"></a><span data-ttu-id="d16e5-103">Виртуалендпоинт: getEffectivePermissions</span><span class="sxs-lookup"><span data-stu-id="d16e5-103">virtualEndpoint: getEffectivePermissions</span></span>

<span data-ttu-id="d16e5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d16e5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d16e5-105">Просмотр действующих разрешений текущего пользователя, прошедшего проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="d16e5-105">View the effective permissions of the currently authenticated user.</span></span> <span data-ttu-id="d16e5-106">GetEffectivePermissions — это функция, которая ретривес действующие разрешения пользователя, прошедшего проверку подлинности, что позволяет скрыть или отключить контент, к которому у текущего пользователя нет доступа.</span><span class="sxs-lookup"><span data-stu-id="d16e5-106">GetEffectivePermissions is a function that retrives the effective permissions of the currently authenticated user, which helps UX hide or disable content that the current user doesn't have access to.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="d16e5-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d16e5-107">Permissions</span></span>

<span data-ttu-id="d16e5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d16e5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d16e5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d16e5-110">Permission type</span></span>|<span data-ttu-id="d16e5-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d16e5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d16e5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d16e5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d16e5-113">Клаудпк. ReadWrite. ALL, Клаудпк. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="d16e5-113">CloudPC.ReadWrite.All, CloudPC.Read.All</span></span>|
|<span data-ttu-id="d16e5-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d16e5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d16e5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d16e5-115">Not supported.</span></span>|
|<span data-ttu-id="d16e5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d16e5-116">Application</span></span>| <span data-ttu-id="d16e5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d16e5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d16e5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d16e5-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/getEffectivePermissions
```

## <a name="request-headers"></a><span data-ttu-id="d16e5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d16e5-119">Request headers</span></span>

| <span data-ttu-id="d16e5-120">Имя</span><span class="sxs-lookup"><span data-stu-id="d16e5-120">Name</span></span>          | <span data-ttu-id="d16e5-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d16e5-121">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="d16e5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d16e5-122">Authorization</span></span> | <span data-ttu-id="d16e5-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d16e5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d16e5-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d16e5-125">Request body</span></span>

<span data-ttu-id="d16e5-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d16e5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d16e5-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="d16e5-127">Response</span></span>

<span data-ttu-id="d16e5-128">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d16e5-128">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span> <span data-ttu-id="d16e5-129">Если у пользователя есть полные разрешения, ответ — `["*"]` .</span><span class="sxs-lookup"><span data-stu-id="d16e5-129">If the user has full permissions, the response is `["*"]`.</span></span>

## <a name="examples"></a><span data-ttu-id="d16e5-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="d16e5-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d16e5-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="d16e5-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d16e5-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="d16e5-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "virtualendpoint_geteffectivepermissions"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/getEffectivePermissions
```
# <a name="c"></a>[<span data-ttu-id="d16e5-133">C#</span><span class="sxs-lookup"><span data-stu-id="d16e5-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/virtualendpoint-geteffectivepermissions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d16e5-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d16e5-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/virtualendpoint-geteffectivepermissions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d16e5-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d16e5-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/virtualendpoint-geteffectivepermissions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d16e5-136">Java</span><span class="sxs-lookup"><span data-stu-id="d16e5-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/virtualendpoint-geteffectivepermissions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d16e5-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="d16e5-137">Response</span></span>

<span data-ttu-id="d16e5-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d16e5-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(Edm.String)"
}
-->

``` http
HTTP/1.1 200 OK

Content-Type: application/json
{
  "value": [
    "Microsoft.CloudPC/CloudPCs/Read"
  ]
}
```
