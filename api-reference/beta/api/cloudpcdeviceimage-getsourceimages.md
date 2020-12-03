---
title: 'Клаудпкдевицеимаже: Жетсаурцеимажес'
description: Просмотрите список всех ресурсов управляемых образов из ваших подписок Azure. Эти исходные изображения можно отправить и использовать на облачных компьютерах.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 824a33fbe28aeca25ea5e1420559cbac71ebffc5
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563398"
---
# <a name="cloudpcdeviceimage-getsourceimages"></a><span data-ttu-id="3a2b7-104">Клаудпкдевицеимаже: Жетсаурцеимажес</span><span class="sxs-lookup"><span data-stu-id="3a2b7-104">cloudPcDeviceImage: getSourceImages</span></span>

<span data-ttu-id="3a2b7-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a2b7-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a2b7-106">Получение объектов [клаудпксаурцедевицеимаже](../resources/cloudpcsourcedeviceimage.md) .</span><span class="sxs-lookup"><span data-stu-id="3a2b7-106">Get [cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) objects.</span></span> <span data-ttu-id="3a2b7-107">Просмотр списка всех ресурсов управляемых образов из ваших подписок на Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3a2b7-107">View a list of all the managed image resources from your Azure Active Directory subscriptions.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="permissions"></a><span data-ttu-id="3a2b7-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3a2b7-108">Permissions</span></span>

<span data-ttu-id="3a2b7-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a2b7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a2b7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a2b7-111">Permission type</span></span>|<span data-ttu-id="3a2b7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a2b7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a2b7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a2b7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3a2b7-114">Клаудпк. ReadWrite. ALL, Клаудпк. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="3a2b7-114">CloudPC.ReadWrite.All, CloudPC.Read.All</span></span>|
|<span data-ttu-id="3a2b7-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a2b7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a2b7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a2b7-116">Not supported.</span></span>|
|<span data-ttu-id="3a2b7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3a2b7-117">Application</span></span>|<span data-ttu-id="3a2b7-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a2b7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a2b7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a2b7-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/deviceImages/getSourceImages
```

## <a name="request-headers"></a><span data-ttu-id="3a2b7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3a2b7-120">Request headers</span></span>

|<span data-ttu-id="3a2b7-121">Имя</span><span class="sxs-lookup"><span data-stu-id="3a2b7-121">Name</span></span>|<span data-ttu-id="3a2b7-122">Описание</span><span class="sxs-lookup"><span data-stu-id="3a2b7-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3a2b7-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3a2b7-123">Authorization</span></span>|<span data-ttu-id="3a2b7-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3a2b7-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a2b7-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3a2b7-126">Request body</span></span>

<span data-ttu-id="3a2b7-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3a2b7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a2b7-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a2b7-128">Response</span></span>

<span data-ttu-id="3a2b7-129">В случае успеха эта функция возвращает `200 OK` код отклика и коллекцию [клаудпксаурцедевицеимаже](../resources/cloudpcsourcedeviceimage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3a2b7-129">If successful, this function returns a `200 OK` response code and a [cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3a2b7-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="3a2b7-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3a2b7-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a2b7-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="3a2b7-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="3a2b7-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "cloudpcdeviceimage_getsourceimages"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/deviceImages/getSourceImages
```
# <a name="c"></a>[<span data-ttu-id="3a2b7-133">C#</span><span class="sxs-lookup"><span data-stu-id="3a2b7-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/cloudpcdeviceimage-getsourceimages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3a2b7-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3a2b7-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cloudpcdeviceimage-getsourceimages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3a2b7-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3a2b7-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cloudpcdeviceimage-getsourceimages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3a2b7-136">Java</span><span class="sxs-lookup"><span data-stu-id="3a2b7-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/cloudpcdeviceimage-getsourceimages-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3a2b7-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a2b7-137">Response</span></span>

<span data-ttu-id="3a2b7-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3a2b7-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.cloudPcSourceDeviceImage)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.cloudPcSourceDeviceImage",
      "id": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG/providers/Microsoft.Compute/images/ExampleImage",
      "displayName": "Display Name value"
    }
  ]
}
```
