---
title: Список объектов enrollmentConfigurationAssignment
description: Список свойств и связей объектов enrollmentConfigurationAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1bf57092a5b27dda0358b61e097015963fc6ff88
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36352618"
---
# <a name="list-enrollmentconfigurationassignments"></a><span data-ttu-id="a8f61-103">Список объектов enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="a8f61-103">List enrollmentConfigurationAssignments</span></span>

> <span data-ttu-id="a8f61-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8f61-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a8f61-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a8f61-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8f61-106">Список свойств и связей объектов [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a8f61-106">List properties and relationships of the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a8f61-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a8f61-107">Prerequisites</span></span>
<span data-ttu-id="a8f61-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8f61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8f61-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a8f61-110">Permission type</span></span>|<span data-ttu-id="a8f61-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a8f61-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8f61-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a8f61-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a8f61-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8f61-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="a8f61-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a8f61-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8f61-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8f61-115">Not supported.</span></span>|
|<span data-ttu-id="a8f61-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a8f61-116">Application</span></span>|<span data-ttu-id="a8f61-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8f61-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8f61-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a8f61-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="a8f61-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a8f61-119">Request headers</span></span>
|<span data-ttu-id="a8f61-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a8f61-120">Header</span></span>|<span data-ttu-id="a8f61-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a8f61-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8f61-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a8f61-122">Authorization</span></span>|<span data-ttu-id="a8f61-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a8f61-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a8f61-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a8f61-124">Accept</span></span>|<span data-ttu-id="a8f61-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a8f61-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8f61-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a8f61-126">Request body</span></span>
<span data-ttu-id="a8f61-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a8f61-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a8f61-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="a8f61-128">Response</span></span>
<span data-ttu-id="a8f61-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a8f61-129">If successful, this method returns a `200 OK` response code and a collection of [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8f61-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a8f61-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a8f61-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a8f61-131">Request</span></span>
<span data-ttu-id="a8f61-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a8f61-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="a8f61-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8f61-133">Response</span></span>
<span data-ttu-id="a8f61-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a8f61-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






