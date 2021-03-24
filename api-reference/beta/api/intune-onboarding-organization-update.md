---
title: Обновление организации
description: Обновление свойств объекта organization.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5f110c15c81661a3c4b12ccc137cc8b6abfcc8c7
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51148752"
---
# <a name="update-organization"></a><span data-ttu-id="c3bd5-103">Обновление организации</span><span class="sxs-lookup"><span data-stu-id="c3bd5-103">Update organization</span></span>

<span data-ttu-id="c3bd5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3bd5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c3bd5-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3bd5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3bd5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c3bd5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3bd5-107">Обновление свойств объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="c3bd5-107">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c3bd5-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c3bd5-108">Prerequisites</span></span>
<span data-ttu-id="c3bd5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3bd5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3bd5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c3bd5-111">Permission type</span></span>|<span data-ttu-id="c3bd5-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c3bd5-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3bd5-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c3bd5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c3bd5-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3bd5-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c3bd5-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c3bd5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3bd5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3bd5-116">Not supported.</span></span>|
|<span data-ttu-id="c3bd5-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="c3bd5-117">Application</span></span>|<span data-ttu-id="c3bd5-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3bd5-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3bd5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c3bd5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /organization/{organizationId}
```

## <a name="request-headers"></a><span data-ttu-id="c3bd5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c3bd5-120">Request headers</span></span>
|<span data-ttu-id="c3bd5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c3bd5-121">Header</span></span>|<span data-ttu-id="c3bd5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c3bd5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3bd5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3bd5-123">Authorization</span></span>|<span data-ttu-id="c3bd5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c3bd5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3bd5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c3bd5-125">Accept</span></span>|<span data-ttu-id="c3bd5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c3bd5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3bd5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c3bd5-127">Request body</span></span>
<span data-ttu-id="c3bd5-128">В теле запроса добавьте представление объекта [organization](../resources/intune-onboarding-organization.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c3bd5-128">In the request body, supply a JSON representation for the [organization](../resources/intune-onboarding-organization.md) object.</span></span>

<span data-ttu-id="c3bd5-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="c3bd5-129">The following table shows the properties that are required when you create the [organization](../resources/intune-onboarding-organization.md).</span></span>

|<span data-ttu-id="c3bd5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c3bd5-130">Property</span></span>|<span data-ttu-id="c3bd5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c3bd5-131">Type</span></span>|<span data-ttu-id="c3bd5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c3bd5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3bd5-133">id</span><span class="sxs-lookup"><span data-stu-id="c3bd5-133">id</span></span>|<span data-ttu-id="c3bd5-134">Строка</span><span class="sxs-lookup"><span data-stu-id="c3bd5-134">String</span></span>|<span data-ttu-id="c3bd5-135">GUID объекта.</span><span class="sxs-lookup"><span data-stu-id="c3bd5-135">The GUID for the object.</span></span>|
|<span data-ttu-id="c3bd5-136">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="c3bd5-136">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="c3bd5-137">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="c3bd5-137">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="c3bd5-138">Центр управления мобильными устройствами.</span><span class="sxs-lookup"><span data-stu-id="c3bd5-138">Mobile device management authority.</span></span> <span data-ttu-id="c3bd5-139">Возможные значения: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="c3bd5-139">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|
|<span data-ttu-id="c3bd5-140">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="c3bd5-140">certificateConnectorSetting</span></span>|[<span data-ttu-id="c3bd5-141">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="c3bd5-141">certificateConnectorSetting</span></span>](../resources/intune-onboarding-certificateconnectorsetting.md)|<span data-ttu-id="c3bd5-142">Параметр соединиттеля сертификата.</span><span class="sxs-lookup"><span data-stu-id="c3bd5-142">Certificate connector setting.</span></span>|



## <a name="response"></a><span data-ttu-id="c3bd5-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3bd5-143">Response</span></span>
<span data-ttu-id="c3bd5-144">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [organization](../resources/intune-onboarding-organization.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c3bd5-144">If successful, this method returns a `200 OK` response code and an updated [organization](../resources/intune-onboarding-organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3bd5-145">Пример</span><span class="sxs-lookup"><span data-stu-id="c3bd5-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="c3bd5-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3bd5-146">Request</span></span>
<span data-ttu-id="c3bd5-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c3bd5-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c3bd5-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3bd5-148">Response</span></span>
<span data-ttu-id="c3bd5-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c3bd5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




