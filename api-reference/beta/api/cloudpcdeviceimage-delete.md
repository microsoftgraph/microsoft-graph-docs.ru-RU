---
title: Удаление Клаудпкдевицеимаже
description: Удаление объекта Клаудпкдевицеимаже.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: a65350162f7810da9c5d20b5f1982d75bc74ef4f
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563333"
---
# <a name="delete-cloudpcdeviceimage"></a><span data-ttu-id="6bfd8-103">Удаление Клаудпкдевицеимаже</span><span class="sxs-lookup"><span data-stu-id="6bfd8-103">Delete cloudPcDeviceImage</span></span>

<span data-ttu-id="6bfd8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6bfd8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6bfd8-105">Удаление объекта [клаудпкдевицеимаже](../resources/cloudpcdeviceimage.md) .</span><span class="sxs-lookup"><span data-stu-id="6bfd8-105">Delete a [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="permissions"></a><span data-ttu-id="6bfd8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6bfd8-106">Permissions</span></span>

<span data-ttu-id="6bfd8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6bfd8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6bfd8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6bfd8-109">Permission type</span></span>|<span data-ttu-id="6bfd8-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6bfd8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6bfd8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6bfd8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6bfd8-112">Клаудпк. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="6bfd8-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="6bfd8-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6bfd8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6bfd8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6bfd8-114">Not supported.</span></span>|
|<span data-ttu-id="6bfd8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6bfd8-115">Application</span></span>|<span data-ttu-id="6bfd8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6bfd8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6bfd8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6bfd8-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /deviceManagement/virtualEndpoint/deviceImages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6bfd8-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6bfd8-118">Request headers</span></span>

|<span data-ttu-id="6bfd8-119">Имя</span><span class="sxs-lookup"><span data-stu-id="6bfd8-119">Name</span></span>|<span data-ttu-id="6bfd8-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6bfd8-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6bfd8-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6bfd8-121">Authorization</span></span>|<span data-ttu-id="6bfd8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6bfd8-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6bfd8-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6bfd8-124">Request body</span></span>

<span data-ttu-id="6bfd8-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6bfd8-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6bfd8-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="6bfd8-126">Response</span></span>

<span data-ttu-id="6bfd8-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6bfd8-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="6bfd8-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="6bfd8-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6bfd8-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="6bfd8-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="6bfd8-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="6bfd8-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_deviceimages_from_virtualendpoint"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/deviceImages/{id}
```
# <a name="c"></a>[<span data-ttu-id="6bfd8-131">C#</span><span class="sxs-lookup"><span data-stu-id="6bfd8-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-deviceimages-from-virtualendpoint-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6bfd8-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6bfd8-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-deviceimages-from-virtualendpoint-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6bfd8-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6bfd8-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-deviceimages-from-virtualendpoint-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6bfd8-134">Java</span><span class="sxs-lookup"><span data-stu-id="6bfd8-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-deviceimages-from-virtualendpoint-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6bfd8-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="6bfd8-135">Response</span></span>

<span data-ttu-id="6bfd8-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6bfd8-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
