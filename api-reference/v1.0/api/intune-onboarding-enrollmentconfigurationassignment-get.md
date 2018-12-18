---
title: Get enrollmentConfigurationAssignment
description: Чтение свойств и связей объекта enrollmentConfigurationAssignment.
author: tfitzmac
ms.openlocfilehash: 05b04b29b41ceb2c3e79e9836a3252ae386d59d3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342723"
---
# <a name="get-enrollmentconfigurationassignment"></a><span data-ttu-id="ffd2f-103">Get enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="ffd2f-103">Get enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="ffd2f-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ffd2f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ffd2f-105">Чтение свойств и связей объекта [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ffd2f-105">Read properties and relationships of the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ffd2f-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="ffd2f-106">Prerequisites</span></span>
<span data-ttu-id="ffd2f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ffd2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ffd2f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ffd2f-109">Permission type</span></span>|<span data-ttu-id="ffd2f-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ffd2f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ffd2f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ffd2f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ffd2f-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ffd2f-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="ffd2f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ffd2f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ffd2f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ffd2f-114">Not supported.</span></span>|
|<span data-ttu-id="ffd2f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ffd2f-115">Application</span></span>|<span data-ttu-id="ffd2f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ffd2f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ffd2f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ffd2f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ffd2f-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ffd2f-118">Optional query parameters</span></span>
<span data-ttu-id="ffd2f-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ffd2f-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ffd2f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ffd2f-120">Request headers</span></span>
|<span data-ttu-id="ffd2f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ffd2f-121">Header</span></span>|<span data-ttu-id="ffd2f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ffd2f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ffd2f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ffd2f-123">Authorization</span></span>|<span data-ttu-id="ffd2f-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ffd2f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ffd2f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ffd2f-125">Accept</span></span>|<span data-ttu-id="ffd2f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ffd2f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ffd2f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ffd2f-127">Request body</span></span>
<span data-ttu-id="ffd2f-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ffd2f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ffd2f-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="ffd2f-129">Response</span></span>
<span data-ttu-id="ffd2f-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ffd2f-130">If successful, this method returns a `200 OK` response code and [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ffd2f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ffd2f-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="ffd2f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ffd2f-132">Request</span></span>
<span data-ttu-id="ffd2f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ffd2f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="ffd2f-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="ffd2f-134">Response</span></span>
<span data-ttu-id="ffd2f-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ffd2f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 251

{
  "value": {
    "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
    "id": "705b021c-021c-705b-1c02-5b701c025b70",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```



