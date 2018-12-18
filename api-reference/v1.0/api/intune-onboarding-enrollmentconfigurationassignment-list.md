---
title: Список объектов enrollmentConfigurationAssignment
description: Список свойств и связей объектов enrollmentConfigurationAssignment.
author: tfitzmac
ms.openlocfilehash: d266cb9782e8be4e7e99fd10eef18680adbf4e40
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303873"
---
# <a name="list-enrollmentconfigurationassignments"></a><span data-ttu-id="dac28-103">Список объектов enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="dac28-103">List enrollmentConfigurationAssignments</span></span>

> <span data-ttu-id="dac28-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="dac28-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dac28-105">Список свойств и связей объектов [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="dac28-105">List properties and relationships of the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dac28-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="dac28-106">Prerequisites</span></span>
<span data-ttu-id="dac28-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dac28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dac28-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dac28-109">Permission type</span></span>|<span data-ttu-id="dac28-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dac28-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dac28-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dac28-111">Delegated (work or school account)</span></span>|<span data-ttu-id="dac28-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="dac28-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="dac28-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dac28-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dac28-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dac28-114">Not supported.</span></span>|
|<span data-ttu-id="dac28-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dac28-115">Application</span></span>|<span data-ttu-id="dac28-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dac28-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dac28-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dac28-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="dac28-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dac28-118">Request headers</span></span>
|<span data-ttu-id="dac28-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dac28-119">Header</span></span>|<span data-ttu-id="dac28-120">Значение</span><span class="sxs-lookup"><span data-stu-id="dac28-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dac28-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dac28-121">Authorization</span></span>|<span data-ttu-id="dac28-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="dac28-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dac28-123">Accept</span><span class="sxs-lookup"><span data-stu-id="dac28-123">Accept</span></span>|<span data-ttu-id="dac28-124">application/json</span><span class="sxs-lookup"><span data-stu-id="dac28-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dac28-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dac28-125">Request body</span></span>
<span data-ttu-id="dac28-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dac28-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dac28-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="dac28-127">Response</span></span>
<span data-ttu-id="dac28-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="dac28-128">If successful, this method returns a `200 OK` response code and a collection of [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dac28-129">Пример</span><span class="sxs-lookup"><span data-stu-id="dac28-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="dac28-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="dac28-130">Request</span></span>
<span data-ttu-id="dac28-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dac28-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="dac28-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="dac28-132">Response</span></span>
<span data-ttu-id="dac28-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="dac28-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



