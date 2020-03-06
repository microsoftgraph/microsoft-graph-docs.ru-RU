---
title: Get enrollmentConfigurationAssignment
description: Чтение свойств и связей объекта enrollmentConfigurationAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 771dd837945258cd3d8a8fa4f2a65e8b908b225d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512491"
---
# <a name="get-enrollmentconfigurationassignment"></a><span data-ttu-id="b11dc-103">Get enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="b11dc-103">Get enrollmentConfigurationAssignment</span></span>

<span data-ttu-id="b11dc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b11dc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b11dc-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b11dc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b11dc-106">Чтение свойств и связей объекта [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b11dc-106">Read properties and relationships of the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b11dc-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="b11dc-107">Prerequisites</span></span>
<span data-ttu-id="b11dc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b11dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b11dc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b11dc-110">Permission type</span></span>|<span data-ttu-id="b11dc-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b11dc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b11dc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b11dc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b11dc-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b11dc-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="b11dc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b11dc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b11dc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b11dc-115">Not supported.</span></span>|
|<span data-ttu-id="b11dc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b11dc-116">Application</span></span>|<span data-ttu-id="b11dc-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b11dc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b11dc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b11dc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b11dc-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b11dc-119">Optional query parameters</span></span>
<span data-ttu-id="b11dc-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b11dc-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b11dc-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b11dc-121">Request headers</span></span>
|<span data-ttu-id="b11dc-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b11dc-122">Header</span></span>|<span data-ttu-id="b11dc-123">Значение</span><span class="sxs-lookup"><span data-stu-id="b11dc-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b11dc-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b11dc-124">Authorization</span></span>|<span data-ttu-id="b11dc-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b11dc-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b11dc-126">Accept</span><span class="sxs-lookup"><span data-stu-id="b11dc-126">Accept</span></span>|<span data-ttu-id="b11dc-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b11dc-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b11dc-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b11dc-128">Request body</span></span>
<span data-ttu-id="b11dc-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b11dc-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b11dc-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="b11dc-130">Response</span></span>
<span data-ttu-id="b11dc-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b11dc-131">If successful, this method returns a `200 OK` response code and [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b11dc-132">Пример</span><span class="sxs-lookup"><span data-stu-id="b11dc-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="b11dc-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b11dc-133">Request</span></span>
<span data-ttu-id="b11dc-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b11dc-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="b11dc-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="b11dc-135">Response</span></span>
<span data-ttu-id="b11dc-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b11dc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




