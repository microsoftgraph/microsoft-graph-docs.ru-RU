---
title: Get managedAppOperation
description: Чтение свойств и связей объекта managedAppOperation.
author: tfitzmac
ms.openlocfilehash: e8a70f52ea696dd77957c35cd2206bb24427497d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344200"
---
# <a name="get-managedappoperation"></a><span data-ttu-id="6ff29-103">Get managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="6ff29-103">Get managedAppOperation</span></span>

> <span data-ttu-id="6ff29-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6ff29-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6ff29-105">Чтение свойств и связей объекта [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="6ff29-105">Read properties and relationships of the [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6ff29-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="6ff29-106">Prerequisites</span></span>
<span data-ttu-id="6ff29-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ff29-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ff29-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6ff29-109">Permission type</span></span>|<span data-ttu-id="6ff29-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6ff29-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ff29-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6ff29-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6ff29-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ff29-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="6ff29-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6ff29-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ff29-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ff29-114">Not supported.</span></span>|
|<span data-ttu-id="6ff29-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6ff29-115">Application</span></span>|<span data-ttu-id="6ff29-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ff29-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ff29-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6ff29-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6ff29-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6ff29-118">Optional query parameters</span></span>
<span data-ttu-id="6ff29-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6ff29-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6ff29-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6ff29-120">Request headers</span></span>
|<span data-ttu-id="6ff29-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6ff29-121">Header</span></span>|<span data-ttu-id="6ff29-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6ff29-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6ff29-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6ff29-123">Authorization</span></span>|<span data-ttu-id="6ff29-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6ff29-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6ff29-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6ff29-125">Accept</span></span>|<span data-ttu-id="6ff29-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6ff29-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ff29-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6ff29-127">Request body</span></span>
<span data-ttu-id="6ff29-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6ff29-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ff29-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="6ff29-129">Response</span></span>
<span data-ttu-id="6ff29-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedAppOperation](../resources/intune-mam-managedappoperation.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6ff29-130">If successful, this method returns a `200 OK` response code and [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ff29-131">Пример</span><span class="sxs-lookup"><span data-stu-id="6ff29-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="6ff29-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ff29-132">Request</span></span>
<span data-ttu-id="6ff29-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6ff29-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
```

### <a name="response"></a><span data-ttu-id="6ff29-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="6ff29-134">Response</span></span>
<span data-ttu-id="6ff29-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="6ff29-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 303

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAppOperation",
    "displayName": "Display Name value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "state": "State value",
    "id": "f2867b06-7b06-f286-067b-86f2067b86f2",
    "version": "Version value"
  }
}
```



