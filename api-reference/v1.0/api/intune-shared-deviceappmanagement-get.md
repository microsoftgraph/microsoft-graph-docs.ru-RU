---
title: Get deviceAppManagement
description: Чтение свойств и связей объекта deviceAppManagement.
ms.openlocfilehash: 02ccc2ab618187824ca69fb536f0a73b922ef1d7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025665"
---
# <a name="get-deviceappmanagement"></a><span data-ttu-id="343ba-103">Get deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="343ba-103">Get deviceAppManagement</span></span>

> <span data-ttu-id="343ba-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="343ba-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="343ba-105">Чтение свойств и связей объекта [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="343ba-105">Read properties and relationships of the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="343ba-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="343ba-106">Prerequisites</span></span>

<span data-ttu-id="343ba-107">Чтобы вызвать этот интерфейс API необходимо одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="343ba-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="343ba-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="343ba-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="343ba-109">Обратите внимание на то, что соответствующим разрешением изменяется в зависимости от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="343ba-109">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="343ba-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="343ba-110">Permission type</span></span>|<span data-ttu-id="343ba-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="343ba-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="343ba-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="343ba-112">Delegated (work or school account)</span></span>|<span data-ttu-id="343ba-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="343ba-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
|<span data-ttu-id="343ba-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="343ba-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="343ba-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="343ba-115">Not supported.</span></span>|
|<span data-ttu-id="343ba-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="343ba-116">Application</span></span>|<span data-ttu-id="343ba-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="343ba-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="343ba-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="343ba-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="343ba-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="343ba-119">Optional query parameters</span></span>
<span data-ttu-id="343ba-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="343ba-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="343ba-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="343ba-121">Request headers</span></span>
|<span data-ttu-id="343ba-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="343ba-122">Header</span></span>|<span data-ttu-id="343ba-123">Значение</span><span class="sxs-lookup"><span data-stu-id="343ba-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="343ba-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="343ba-124">Authorization</span></span>|<span data-ttu-id="343ba-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="343ba-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="343ba-126">Accept</span><span class="sxs-lookup"><span data-stu-id="343ba-126">Accept</span></span>|<span data-ttu-id="343ba-127">application/json</span><span class="sxs-lookup"><span data-stu-id="343ba-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="343ba-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="343ba-128">Request body</span></span>
<span data-ttu-id="343ba-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="343ba-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="343ba-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="343ba-130">Response</span></span>
<span data-ttu-id="343ba-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="343ba-131">If successful, this method returns a `200 OK` response code and [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example-request"></a><span data-ttu-id="343ba-132">Пример запроса</span><span class="sxs-lookup"><span data-stu-id="343ba-132">Example request</span></span>

``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement
```

## <a name="example-response"></a><span data-ttu-id="343ba-133">Пример ответа</span><span class="sxs-lookup"><span data-stu-id="343ba-133">Example response</span></span>
<span data-ttu-id="343ba-134">Для краткости может усекаться объект ответа, показано ниже.</span><span class="sxs-lookup"><span data-stu-id="343ba-134">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="343ba-135">Будут возвращены все свойства из фактический вызов.</span><span class="sxs-lookup"><span data-stu-id="343ba-135">All properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 133

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceAppManagement",
    "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
  }
}
```



