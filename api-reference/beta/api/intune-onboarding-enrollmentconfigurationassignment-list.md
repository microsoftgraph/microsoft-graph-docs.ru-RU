---
title: Список объектов enrollmentConfigurationAssignment
description: Список свойств и связей объектов enrollmentConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7663e8c630b5debddbd824be85cd1e51d6acc984
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156870"
---
# <a name="list-enrollmentconfigurationassignments"></a><span data-ttu-id="790ab-103">Список объектов enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="790ab-103">List enrollmentConfigurationAssignments</span></span>

<span data-ttu-id="790ab-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="790ab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="790ab-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="790ab-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="790ab-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="790ab-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="790ab-107">Список свойств и связей объектов [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="790ab-107">List properties and relationships of the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="790ab-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="790ab-108">Prerequisites</span></span>
<span data-ttu-id="790ab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="790ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="790ab-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="790ab-111">Permission type</span></span>|<span data-ttu-id="790ab-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="790ab-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="790ab-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="790ab-113">Delegated (work or school account)</span></span>|<span data-ttu-id="790ab-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="790ab-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="790ab-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="790ab-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="790ab-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="790ab-116">Not supported.</span></span>|
|<span data-ttu-id="790ab-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="790ab-117">Application</span></span>|<span data-ttu-id="790ab-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="790ab-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="790ab-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="790ab-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="790ab-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="790ab-120">Request headers</span></span>
|<span data-ttu-id="790ab-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="790ab-121">Header</span></span>|<span data-ttu-id="790ab-122">Значение</span><span class="sxs-lookup"><span data-stu-id="790ab-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="790ab-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="790ab-123">Authorization</span></span>|<span data-ttu-id="790ab-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="790ab-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="790ab-125">Accept</span><span class="sxs-lookup"><span data-stu-id="790ab-125">Accept</span></span>|<span data-ttu-id="790ab-126">application/json</span><span class="sxs-lookup"><span data-stu-id="790ab-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="790ab-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="790ab-127">Request body</span></span>
<span data-ttu-id="790ab-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="790ab-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="790ab-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="790ab-129">Response</span></span>
<span data-ttu-id="790ab-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="790ab-130">If successful, this method returns a `200 OK` response code and a collection of [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="790ab-131">Пример</span><span class="sxs-lookup"><span data-stu-id="790ab-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="790ab-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="790ab-132">Request</span></span>
<span data-ttu-id="790ab-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="790ab-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="790ab-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="790ab-134">Response</span></span>
<span data-ttu-id="790ab-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="790ab-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 575

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
      "id": "705b021c-021c-705b-1c02-5b701c025b70",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      },
      "source": "policySets",
      "sourceId": "Source Id value"
    }
  ]
}
```




