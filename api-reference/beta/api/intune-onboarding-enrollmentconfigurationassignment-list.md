---
title: Список объектов enrollmentConfigurationAssignment
description: Список свойств и связей объектов enrollmentConfigurationAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b95737942b88d6f4ec1b5b6546a3921a976333e4
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33900077"
---
# <a name="list-enrollmentconfigurationassignments"></a><span data-ttu-id="5706b-103">Список объектов enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="5706b-103">List enrollmentConfigurationAssignments</span></span>

> <span data-ttu-id="5706b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5706b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5706b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5706b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5706b-106">Список свойств и связей объектов [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5706b-106">List properties and relationships of the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5706b-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5706b-107">Prerequisites</span></span>
<span data-ttu-id="5706b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5706b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5706b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5706b-110">Permission type</span></span>|<span data-ttu-id="5706b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5706b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5706b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5706b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5706b-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="5706b-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="5706b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5706b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5706b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5706b-115">Not supported.</span></span>|
|<span data-ttu-id="5706b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5706b-116">Application</span></span>|<span data-ttu-id="5706b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5706b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5706b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5706b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="5706b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5706b-119">Request headers</span></span>
|<span data-ttu-id="5706b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5706b-120">Header</span></span>|<span data-ttu-id="5706b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5706b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5706b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5706b-122">Authorization</span></span>|<span data-ttu-id="5706b-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5706b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5706b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5706b-124">Accept</span></span>|<span data-ttu-id="5706b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5706b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5706b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5706b-126">Request body</span></span>
<span data-ttu-id="5706b-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5706b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5706b-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="5706b-128">Response</span></span>
<span data-ttu-id="5706b-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5706b-129">If successful, this method returns a `200 OK` response code and a collection of [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5706b-130">Пример</span><span class="sxs-lookup"><span data-stu-id="5706b-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="5706b-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="5706b-131">Request</span></span>
<span data-ttu-id="5706b-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5706b-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="5706b-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="5706b-133">Response</span></span>
<span data-ttu-id="5706b-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5706b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




