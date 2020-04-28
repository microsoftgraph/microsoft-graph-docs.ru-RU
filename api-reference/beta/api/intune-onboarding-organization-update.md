---
title: Обновление организации
description: Обновление свойств объекта organization.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 99bafa9aa4098700376a6281af359dfb02c77de1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43463147"
---
# <a name="update-organization"></a><span data-ttu-id="2a588-103">Обновление организации</span><span class="sxs-lookup"><span data-stu-id="2a588-103">Update organization</span></span>

<span data-ttu-id="2a588-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a588-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2a588-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a588-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a588-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2a588-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a588-107">Обновление свойств объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="2a588-107">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2a588-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2a588-108">Prerequisites</span></span>
<span data-ttu-id="2a588-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a588-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a588-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2a588-111">Permission type</span></span>|<span data-ttu-id="2a588-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2a588-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a588-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2a588-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2a588-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a588-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2a588-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2a588-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a588-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a588-116">Not supported.</span></span>|
|<span data-ttu-id="2a588-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2a588-117">Application</span></span>|<span data-ttu-id="2a588-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a588-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a588-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2a588-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /organization/{organizationId}
```

## <a name="request-headers"></a><span data-ttu-id="2a588-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2a588-120">Request headers</span></span>
|<span data-ttu-id="2a588-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2a588-121">Header</span></span>|<span data-ttu-id="2a588-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2a588-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a588-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2a588-123">Authorization</span></span>|<span data-ttu-id="2a588-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2a588-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a588-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2a588-125">Accept</span></span>|<span data-ttu-id="2a588-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2a588-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a588-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2a588-127">Request body</span></span>
<span data-ttu-id="2a588-128">В теле запроса добавьте представление объекта [organization](../resources/intune-onboarding-organization.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2a588-128">In the request body, supply a JSON representation for the [organization](../resources/intune-onboarding-organization.md) object.</span></span>

<span data-ttu-id="2a588-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="2a588-129">The following table shows the properties that are required when you create the [organization](../resources/intune-onboarding-organization.md).</span></span>

|<span data-ttu-id="2a588-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2a588-130">Property</span></span>|<span data-ttu-id="2a588-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2a588-131">Type</span></span>|<span data-ttu-id="2a588-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2a588-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a588-133">id</span><span class="sxs-lookup"><span data-stu-id="2a588-133">id</span></span>|<span data-ttu-id="2a588-134">String</span><span class="sxs-lookup"><span data-stu-id="2a588-134">String</span></span>|<span data-ttu-id="2a588-135">GUID объекта.</span><span class="sxs-lookup"><span data-stu-id="2a588-135">The GUID for the object.</span></span>|
|<span data-ttu-id="2a588-136">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="2a588-136">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="2a588-137">мдмаусорити</span><span class="sxs-lookup"><span data-stu-id="2a588-137">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="2a588-138">Центр управления мобильными устройствами.</span><span class="sxs-lookup"><span data-stu-id="2a588-138">Mobile device management authority.</span></span> <span data-ttu-id="2a588-139">Возможные значения: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="2a588-139">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|
|<span data-ttu-id="2a588-140">цертификатеконнекторсеттинг</span><span class="sxs-lookup"><span data-stu-id="2a588-140">certificateConnectorSetting</span></span>|[<span data-ttu-id="2a588-141">цертификатеконнекторсеттинг</span><span class="sxs-lookup"><span data-stu-id="2a588-141">certificateConnectorSetting</span></span>](../resources/intune-onboarding-certificateconnectorsetting.md)|<span data-ttu-id="2a588-142">Параметр соединителя сертификатов.</span><span class="sxs-lookup"><span data-stu-id="2a588-142">Certificate connector setting.</span></span>|



## <a name="response"></a><span data-ttu-id="2a588-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a588-143">Response</span></span>
<span data-ttu-id="2a588-144">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [organization](../resources/intune-onboarding-organization.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2a588-144">If successful, this method returns a `200 OK` response code and an updated [organization](../resources/intune-onboarding-organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a588-145">Пример</span><span class="sxs-lookup"><span data-stu-id="2a588-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="2a588-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="2a588-146">Request</span></span>
<span data-ttu-id="2a588-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2a588-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/organization/{organizationId}
Content-type: application/json
Content-length: 492

{
  "@odata.type": "#microsoft.graph.organization",
  "mobileDeviceManagementAuthority": "intune",
  "certificateConnectorSetting": {
    "@odata.type": "microsoft.graph.certificateConnectorSetting",
    "status": 6,
    "certExpiryTime": "2017-01-01T00:00:03.9979674-08:00",
    "enrollmentError": "Enrollment Error value",
    "lastConnectorConnectionTime": "2017-01-01T00:02:50.2393584-08:00",
    "connectorVersion": "Connector Version value",
    "lastUploadVersion": 1
  }
}
```

### <a name="response"></a><span data-ttu-id="2a588-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a588-148">Response</span></span>
<span data-ttu-id="2a588-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2a588-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 541

{
  "@odata.type": "#microsoft.graph.organization",
  "id": "9efe224a-224a-9efe-4a22-fe9e4a22fe9e",
  "mobileDeviceManagementAuthority": "intune",
  "certificateConnectorSetting": {
    "@odata.type": "microsoft.graph.certificateConnectorSetting",
    "status": 6,
    "certExpiryTime": "2017-01-01T00:00:03.9979674-08:00",
    "enrollmentError": "Enrollment Error value",
    "lastConnectorConnectionTime": "2017-01-01T00:02:50.2393584-08:00",
    "connectorVersion": "Connector Version value",
    "lastUploadVersion": 1
  }
}
```



