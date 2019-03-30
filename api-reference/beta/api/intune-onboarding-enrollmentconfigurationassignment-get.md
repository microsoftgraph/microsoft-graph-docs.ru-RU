---
title: Get enrollmentConfigurationAssignment
description: Чтение свойств и связей объекта enrollmentConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3655eda5240f4770931b8cfad9a4685ad79f671c
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30987421"
---
# <a name="get-enrollmentconfigurationassignment"></a><span data-ttu-id="a6ee1-103">Get enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="a6ee1-103">Get enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="a6ee1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6ee1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6ee1-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a6ee1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6ee1-106">Чтение свойств и связей объекта [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a6ee1-106">Read properties and relationships of the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a6ee1-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="a6ee1-107">Prerequisites</span></span>
<span data-ttu-id="a6ee1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6ee1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6ee1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a6ee1-110">Permission type</span></span>|<span data-ttu-id="a6ee1-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a6ee1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6ee1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a6ee1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a6ee1-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="a6ee1-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="a6ee1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a6ee1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6ee1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6ee1-115">Not supported.</span></span>|
|<span data-ttu-id="a6ee1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a6ee1-116">Application</span></span>|<span data-ttu-id="a6ee1-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6ee1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6ee1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a6ee1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a6ee1-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a6ee1-119">Optional query parameters</span></span>
<span data-ttu-id="a6ee1-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a6ee1-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a6ee1-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a6ee1-121">Request headers</span></span>
|<span data-ttu-id="a6ee1-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a6ee1-122">Header</span></span>|<span data-ttu-id="a6ee1-123">Значение</span><span class="sxs-lookup"><span data-stu-id="a6ee1-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6ee1-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a6ee1-124">Authorization</span></span>|<span data-ttu-id="a6ee1-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a6ee1-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6ee1-126">Accept</span><span class="sxs-lookup"><span data-stu-id="a6ee1-126">Accept</span></span>|<span data-ttu-id="a6ee1-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a6ee1-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6ee1-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a6ee1-128">Request body</span></span>
<span data-ttu-id="a6ee1-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a6ee1-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6ee1-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="a6ee1-130">Response</span></span>
<span data-ttu-id="a6ee1-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a6ee1-131">If successful, this method returns a `200 OK` response code and [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6ee1-132">Пример</span><span class="sxs-lookup"><span data-stu-id="a6ee1-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6ee1-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="a6ee1-133">Request</span></span>
<span data-ttu-id="a6ee1-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a6ee1-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="a6ee1-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6ee1-135">Response</span></span>
<span data-ttu-id="a6ee1-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a6ee1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




