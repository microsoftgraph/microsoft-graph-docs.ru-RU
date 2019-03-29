---
title: Список объектов enrollmentConfigurationAssignment
description: Список свойств и связей объектов enrollmentConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0dbcb2c3809f426c1c56b87d061dfaff92c3677f
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30979909"
---
# <a name="list-enrollmentconfigurationassignments"></a><span data-ttu-id="5edb4-103">Список объектов enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="5edb4-103">List enrollmentConfigurationAssignments</span></span>

> <span data-ttu-id="5edb4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5edb4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5edb4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5edb4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5edb4-106">Список свойств и связей объектов [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5edb4-106">List properties and relationships of the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5edb4-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5edb4-107">Prerequisites</span></span>
<span data-ttu-id="5edb4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5edb4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5edb4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5edb4-110">Permission type</span></span>|<span data-ttu-id="5edb4-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5edb4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5edb4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5edb4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5edb4-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="5edb4-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="5edb4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5edb4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5edb4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5edb4-115">Not supported.</span></span>|
|<span data-ttu-id="5edb4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5edb4-116">Application</span></span>|<span data-ttu-id="5edb4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5edb4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5edb4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5edb4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="5edb4-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5edb4-119">Request headers</span></span>
|<span data-ttu-id="5edb4-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5edb4-120">Header</span></span>|<span data-ttu-id="5edb4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5edb4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5edb4-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5edb4-122">Authorization</span></span>|<span data-ttu-id="5edb4-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5edb4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5edb4-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5edb4-124">Accept</span></span>|<span data-ttu-id="5edb4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5edb4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5edb4-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5edb4-126">Request body</span></span>
<span data-ttu-id="5edb4-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5edb4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5edb4-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="5edb4-128">Response</span></span>
<span data-ttu-id="5edb4-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5edb4-129">If successful, this method returns a `200 OK` response code and a collection of [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5edb4-130">Пример</span><span class="sxs-lookup"><span data-stu-id="5edb4-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="5edb4-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="5edb4-131">Request</span></span>
<span data-ttu-id="5edb4-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5edb4-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="5edb4-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="5edb4-133">Response</span></span>
<span data-ttu-id="5edb4-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5edb4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




