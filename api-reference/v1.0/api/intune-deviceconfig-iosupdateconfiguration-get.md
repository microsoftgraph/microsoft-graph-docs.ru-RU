---
title: Get iosUpdateConfiguration
description: Чтение свойств и связей объекта iosUpdateConfiguration.
author: tfitzmac
ms.openlocfilehash: 09c27673f1ea379ece5d42348235b224bd80ec18
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344795"
---
# <a name="get-iosupdateconfiguration"></a><span data-ttu-id="73fdd-103">Get iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="73fdd-103">Get iosUpdateConfiguration</span></span>

> <span data-ttu-id="73fdd-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="73fdd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="73fdd-105">Чтение свойств и связей объекта [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="73fdd-105">Read properties and relationships of the [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="73fdd-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="73fdd-106">Prerequisites</span></span>
<span data-ttu-id="73fdd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73fdd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73fdd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="73fdd-109">Permission type</span></span>|<span data-ttu-id="73fdd-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="73fdd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73fdd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="73fdd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="73fdd-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="73fdd-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="73fdd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="73fdd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73fdd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73fdd-114">Not supported.</span></span>|
|<span data-ttu-id="73fdd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="73fdd-115">Application</span></span>|<span data-ttu-id="73fdd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73fdd-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="73fdd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="73fdd-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="73fdd-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="73fdd-118">Optional query parameters</span></span>
<span data-ttu-id="73fdd-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="73fdd-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="73fdd-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="73fdd-120">Request headers</span></span>
|<span data-ttu-id="73fdd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="73fdd-121">Header</span></span>|<span data-ttu-id="73fdd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="73fdd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73fdd-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="73fdd-123">Authorization</span></span>|<span data-ttu-id="73fdd-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="73fdd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73fdd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="73fdd-125">Accept</span></span>|<span data-ttu-id="73fdd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="73fdd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73fdd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="73fdd-127">Request body</span></span>
<span data-ttu-id="73fdd-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="73fdd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73fdd-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="73fdd-129">Response</span></span>
<span data-ttu-id="73fdd-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="73fdd-130">If successful, this method returns a `200 OK` response code and [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73fdd-131">Пример</span><span class="sxs-lookup"><span data-stu-id="73fdd-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="73fdd-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="73fdd-132">Request</span></span>
<span data-ttu-id="73fdd-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="73fdd-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="73fdd-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="73fdd-134">Response</span></span>
<span data-ttu-id="73fdd-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="73fdd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 542

{
  "value": {
    "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
    "id": "321aef09-ef09-321a-09ef-1a3209ef1a32",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "activeHoursStart": "12:00:05.5020000",
    "activeHoursEnd": "11:59:00.8990000",
    "scheduledInstallDays": [
      "monday"
    ],
    "utcTimeOffsetInMinutes": 6
  }
}
```



