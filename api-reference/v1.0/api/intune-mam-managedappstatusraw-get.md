---
title: Get managedAppStatusRaw
description: Считывание свойств и связей объекта managedAppStatusRaw.
author: tfitzmac
ms.openlocfilehash: 731df6554e33c05d974bd0850273b485820196c4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334757"
---
# <a name="get-managedappstatusraw"></a><span data-ttu-id="51c45-103">Get managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="51c45-103">Get managedAppStatusRaw</span></span>

> <span data-ttu-id="51c45-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="51c45-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="51c45-105">Чтение свойств и связей объекта [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="51c45-105">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="51c45-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="51c45-106">Prerequisites</span></span>
<span data-ttu-id="51c45-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51c45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51c45-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51c45-109">Permission type</span></span>|<span data-ttu-id="51c45-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="51c45-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51c45-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51c45-111">Delegated (work or school account)</span></span>|<span data-ttu-id="51c45-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="51c45-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="51c45-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51c45-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51c45-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51c45-114">Not supported.</span></span>|
|<span data-ttu-id="51c45-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="51c45-115">Application</span></span>|<span data-ttu-id="51c45-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51c45-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51c45-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51c45-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppStatuses/{managedAppStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="51c45-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="51c45-118">Optional query parameters</span></span>
<span data-ttu-id="51c45-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="51c45-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="51c45-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="51c45-120">Request headers</span></span>
|<span data-ttu-id="51c45-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="51c45-121">Header</span></span>|<span data-ttu-id="51c45-122">Значение</span><span class="sxs-lookup"><span data-stu-id="51c45-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51c45-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="51c45-123">Authorization</span></span>|<span data-ttu-id="51c45-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="51c45-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51c45-125">Accept</span><span class="sxs-lookup"><span data-stu-id="51c45-125">Accept</span></span>|<span data-ttu-id="51c45-126">application/json</span><span class="sxs-lookup"><span data-stu-id="51c45-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51c45-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="51c45-127">Request body</span></span>
<span data-ttu-id="51c45-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="51c45-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51c45-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="51c45-129">Response</span></span>
<span data-ttu-id="51c45-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="51c45-130">If successful, this method returns a `200 OK` response code and [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51c45-131">Пример</span><span class="sxs-lookup"><span data-stu-id="51c45-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="51c45-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="51c45-132">Request</span></span>
<span data-ttu-id="51c45-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51c45-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppStatuses/{managedAppStatusId}
```

### <a name="response"></a><span data-ttu-id="51c45-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="51c45-134">Response</span></span>
<span data-ttu-id="51c45-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="51c45-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 279

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAppStatusRaw",
    "displayName": "Display Name value",
    "id": "80847581-7581-8084-8175-848081758480",
    "version": "Version value",
    "content": {
      "@odata.type": "microsoft.graph.Json"
    }
  }
}
```



