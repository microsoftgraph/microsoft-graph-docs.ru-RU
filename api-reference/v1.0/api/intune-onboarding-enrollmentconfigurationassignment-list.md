---
title: Список объектов enrollmentConfigurationAssignment
description: Список свойств и связей объектов enrollmentConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4c4dd32834c7db0401f571c103f6e37f78f9795d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561602"
---
# <a name="list-enrollmentconfigurationassignments"></a><span data-ttu-id="475c7-103">Список объектов enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="475c7-103">List enrollmentConfigurationAssignments</span></span>

> <span data-ttu-id="475c7-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="475c7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="475c7-105">Список свойств и связей объектов [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="475c7-105">List properties and relationships of the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="475c7-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="475c7-106">Prerequisites</span></span>
<span data-ttu-id="475c7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="475c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="475c7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="475c7-109">Permission type</span></span>|<span data-ttu-id="475c7-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="475c7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="475c7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="475c7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="475c7-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="475c7-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="475c7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="475c7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="475c7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="475c7-114">Not supported.</span></span>|
|<span data-ttu-id="475c7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="475c7-115">Application</span></span>|<span data-ttu-id="475c7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="475c7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="475c7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="475c7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="475c7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="475c7-118">Request headers</span></span>
|<span data-ttu-id="475c7-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="475c7-119">Header</span></span>|<span data-ttu-id="475c7-120">Значение</span><span class="sxs-lookup"><span data-stu-id="475c7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="475c7-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="475c7-121">Authorization</span></span>|<span data-ttu-id="475c7-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="475c7-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="475c7-123">Accept</span><span class="sxs-lookup"><span data-stu-id="475c7-123">Accept</span></span>|<span data-ttu-id="475c7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="475c7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="475c7-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="475c7-125">Request body</span></span>
<span data-ttu-id="475c7-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="475c7-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="475c7-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="475c7-127">Response</span></span>
<span data-ttu-id="475c7-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="475c7-128">If successful, this method returns a `200 OK` response code and a collection of [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="475c7-129">Пример</span><span class="sxs-lookup"><span data-stu-id="475c7-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="475c7-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="475c7-130">Request</span></span>
<span data-ttu-id="475c7-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="475c7-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="475c7-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="475c7-132">Response</span></span>
<span data-ttu-id="475c7-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="475c7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



