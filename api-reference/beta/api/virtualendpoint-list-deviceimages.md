---
title: Список Клаудпкдевицеимажес
description: Перечисление свойств и связей образов ОС, отправленных на Облачный компьютер.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 4d392331b2cb07446374275d0ffb8e606fe7d99d
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378596"
---
# <a name="list-deviceimages"></a><span data-ttu-id="098b9-103">Список Девицеимажес</span><span class="sxs-lookup"><span data-stu-id="098b9-103">List deviceImages</span></span>

<span data-ttu-id="098b9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="098b9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="098b9-105">Список свойств и связей объектов [клаудпкдевицеимаже](../resources/cloudpcdeviceimage.md) (образов ОС), отправленных на Облачный компьютер.</span><span class="sxs-lookup"><span data-stu-id="098b9-105">List the properties and relationships of the [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) objects (OS images) uploaded to cloud PC.</span></span>

## <a name="permissions"></a><span data-ttu-id="098b9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="098b9-106">Permissions</span></span>

<span data-ttu-id="098b9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="098b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="098b9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="098b9-109">Permission type</span></span>|<span data-ttu-id="098b9-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="098b9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="098b9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="098b9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="098b9-112">Клаудпк. ReadWrite. ALL, Клаудпк. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="098b9-112">CloudPC.ReadWrite.All, CloudPC.Read.All</span></span>|
|<span data-ttu-id="098b9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="098b9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="098b9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="098b9-114">Not supported.</span></span>|
|<span data-ttu-id="098b9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="098b9-115">Application</span></span>|<span data-ttu-id="098b9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="098b9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="098b9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="098b9-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/deviceImages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="098b9-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="098b9-118">Optional query parameters</span></span>

<span data-ttu-id="098b9-119">Этот метод поддерживает `$select` и `$filter` параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="098b9-119">This method supports `$select` and `$filter` OData query parameters to help customize the response.</span></span> <span data-ttu-id="098b9-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="098b9-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="098b9-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="098b9-121">Request headers</span></span>

| <span data-ttu-id="098b9-122">Имя</span><span class="sxs-lookup"><span data-stu-id="098b9-122">Name</span></span>          | <span data-ttu-id="098b9-123">Описание</span><span class="sxs-lookup"><span data-stu-id="098b9-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="098b9-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="098b9-124">Authorization</span></span> | <span data-ttu-id="098b9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="098b9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="098b9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="098b9-127">Request body</span></span>

<span data-ttu-id="098b9-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="098b9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="098b9-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="098b9-129">Response</span></span>

<span data-ttu-id="098b9-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [клаудпкдевицеимаже](../resources/cloudpcdeviceimage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="098b9-130">If successful, this method returns a `200 OK` response code and a collection of [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="098b9-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="098b9-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="098b9-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="098b9-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_cloudpcdeviceimages"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/deviceImages
```

### <a name="response"></a><span data-ttu-id="098b9-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="098b9-133">Response</span></span>

<span data-ttu-id="098b9-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="098b9-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.cloudPcDeviceImage)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.cloudPcDeviceImage",
      "id": "eda7ed64-7705-4079-9d08-c2bd883fffff",
      "displayName": "Display Name value",
      "osBuildNumber": "OS Build Number value",
      "operatingSystem": "Operating System value",
      "version": "Version value",
      "sourceImageResourceId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG/providers/Microsoft.Compute/images/ExampleImage",
      "lastModifiedDateTime": "2020-11-03T07:03:44Z",
      "status": "pending",
      "statusDetails": null
    }
  ]
}
```
