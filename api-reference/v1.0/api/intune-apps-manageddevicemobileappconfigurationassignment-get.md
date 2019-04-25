---
title: Get managedDeviceMobileAppConfigurationAssignment
description: Чтение свойств и связей объекта managedDeviceMobileAppConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8c42aaadd5809d77ed70cc22f5b4d08ba7f1c5cc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32578528"
---
# <a name="get-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="13a29-103">Get managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="13a29-103">Get managedDeviceMobileAppConfigurationAssignment</span></span>

> <span data-ttu-id="13a29-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="13a29-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13a29-105">Чтение свойств и связей объекта [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="13a29-105">Read properties and relationships of the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13a29-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="13a29-106">Prerequisites</span></span>
<span data-ttu-id="13a29-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13a29-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13a29-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="13a29-109">Permission type</span></span>|<span data-ttu-id="13a29-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="13a29-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13a29-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="13a29-111">Delegated (work or school account)</span></span>|<span data-ttu-id="13a29-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="13a29-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="13a29-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="13a29-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13a29-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13a29-114">Not supported.</span></span>|
|<span data-ttu-id="13a29-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="13a29-115">Application</span></span>|<span data-ttu-id="13a29-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13a29-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="13a29-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="13a29-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="13a29-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="13a29-118">Optional query parameters</span></span>
<span data-ttu-id="13a29-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="13a29-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="13a29-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="13a29-120">Request headers</span></span>
|<span data-ttu-id="13a29-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="13a29-121">Header</span></span>|<span data-ttu-id="13a29-122">Значение</span><span class="sxs-lookup"><span data-stu-id="13a29-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13a29-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="13a29-123">Authorization</span></span>|<span data-ttu-id="13a29-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="13a29-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13a29-125">Accept</span><span class="sxs-lookup"><span data-stu-id="13a29-125">Accept</span></span>|<span data-ttu-id="13a29-126">application/json</span><span class="sxs-lookup"><span data-stu-id="13a29-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13a29-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="13a29-127">Request body</span></span>
<span data-ttu-id="13a29-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="13a29-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13a29-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="13a29-129">Response</span></span>
<span data-ttu-id="13a29-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="13a29-130">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13a29-131">Пример</span><span class="sxs-lookup"><span data-stu-id="13a29-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="13a29-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="13a29-132">Request</span></span>
<span data-ttu-id="13a29-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="13a29-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="13a29-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="13a29-134">Response</span></span>
<span data-ttu-id="13a29-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="13a29-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 263

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
    "id": "4df81c9c-1c9c-4df8-9c1c-f84d9c1cf84d",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```



