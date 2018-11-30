---
title: Get enrollmentConfigurationAssignment
description: Чтение свойств и связей объекта enrollmentConfigurationAssignment.
ms.openlocfilehash: e9e9be8484770ae55a3daf7ac9114106a3a4846a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026543"
---
# <a name="get-enrollmentconfigurationassignment"></a><span data-ttu-id="c3049-103">Get enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="c3049-103">Get enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="c3049-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c3049-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c3049-105">Чтение свойств и связей объекта [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c3049-105">Read properties and relationships of the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c3049-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="c3049-106">Prerequisites</span></span>
<span data-ttu-id="c3049-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3049-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3049-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c3049-109">Permission type</span></span>|<span data-ttu-id="c3049-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c3049-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3049-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c3049-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c3049-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c3049-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="c3049-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c3049-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3049-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3049-114">Not supported.</span></span>|
|<span data-ttu-id="c3049-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c3049-115">Application</span></span>|<span data-ttu-id="c3049-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3049-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3049-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c3049-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c3049-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c3049-118">Optional query parameters</span></span>
<span data-ttu-id="c3049-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c3049-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c3049-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c3049-120">Request headers</span></span>
|<span data-ttu-id="c3049-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c3049-121">Header</span></span>|<span data-ttu-id="c3049-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c3049-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3049-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3049-123">Authorization</span></span>|<span data-ttu-id="c3049-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c3049-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3049-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c3049-125">Accept</span></span>|<span data-ttu-id="c3049-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c3049-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3049-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c3049-127">Request body</span></span>
<span data-ttu-id="c3049-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c3049-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c3049-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="c3049-129">Response</span></span>
<span data-ttu-id="c3049-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c3049-130">If successful, this method returns a `200 OK` response code and [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3049-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c3049-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="c3049-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3049-132">Request</span></span>
<span data-ttu-id="c3049-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c3049-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="c3049-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="c3049-134">Response</span></span>
<span data-ttu-id="c3049-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="c3049-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



