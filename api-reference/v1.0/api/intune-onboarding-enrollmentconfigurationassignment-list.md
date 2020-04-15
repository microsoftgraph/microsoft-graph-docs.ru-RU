---
title: Список объектов enrollmentConfigurationAssignment
description: Список свойств и связей объектов enrollmentConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a5787dd76300b45c59bcb0f466bc6d99c8294e48
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43442403"
---
# <a name="list-enrollmentconfigurationassignments"></a><span data-ttu-id="f158f-103">Список объектов enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="f158f-103">List enrollmentConfigurationAssignments</span></span>

<span data-ttu-id="f158f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f158f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f158f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f158f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f158f-106">Список свойств и связей объектов [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f158f-106">List properties and relationships of the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f158f-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f158f-107">Prerequisites</span></span>
<span data-ttu-id="f158f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f158f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f158f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f158f-110">Permission type</span></span>|<span data-ttu-id="f158f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f158f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f158f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f158f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f158f-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f158f-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="f158f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f158f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f158f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f158f-115">Not supported.</span></span>|
|<span data-ttu-id="f158f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f158f-116">Application</span></span>|<span data-ttu-id="f158f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f158f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f158f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f158f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="f158f-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f158f-119">Request headers</span></span>
|<span data-ttu-id="f158f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f158f-120">Header</span></span>|<span data-ttu-id="f158f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f158f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f158f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f158f-122">Authorization</span></span>|<span data-ttu-id="f158f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f158f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f158f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f158f-124">Accept</span></span>|<span data-ttu-id="f158f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f158f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f158f-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f158f-126">Request body</span></span>
<span data-ttu-id="f158f-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f158f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f158f-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="f158f-128">Response</span></span>
<span data-ttu-id="f158f-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f158f-129">If successful, this method returns a `200 OK` response code and a collection of [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f158f-130">Пример</span><span class="sxs-lookup"><span data-stu-id="f158f-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f158f-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="f158f-131">Request</span></span>
<span data-ttu-id="f158f-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f158f-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="f158f-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="f158f-133">Response</span></span>
<span data-ttu-id="f158f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f158f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 275

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
      "id": "705b021c-021c-705b-1c02-5b701c025b70",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```






