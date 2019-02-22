---
title: Обновление организации
description: Обновление свойств объекта organization.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a1f1a2e48e882cf6e314f3aa58a2c7bab99b2832
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157759"
---
# <a name="update-organization"></a><span data-ttu-id="e0018-103">Обновление организации</span><span class="sxs-lookup"><span data-stu-id="e0018-103">Update organization</span></span>

> <span data-ttu-id="e0018-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0018-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e0018-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e0018-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0018-106">Обновление свойств объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="e0018-106">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e0018-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e0018-107">Prerequisites</span></span>
<span data-ttu-id="e0018-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e0018-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e0018-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e0018-110">Permission type</span></span>|<span data-ttu-id="e0018-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e0018-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0018-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e0018-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e0018-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0018-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e0018-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e0018-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0018-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0018-115">Not supported.</span></span>|
|<span data-ttu-id="e0018-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e0018-116">Application</span></span>|<span data-ttu-id="e0018-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0018-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0018-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e0018-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /organization/{organizationId}
```

## <a name="request-headers"></a><span data-ttu-id="e0018-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e0018-119">Request headers</span></span>
|<span data-ttu-id="e0018-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e0018-120">Header</span></span>|<span data-ttu-id="e0018-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e0018-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0018-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e0018-122">Authorization</span></span>|<span data-ttu-id="e0018-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e0018-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0018-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e0018-124">Accept</span></span>|<span data-ttu-id="e0018-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e0018-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0018-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e0018-126">Request body</span></span>
<span data-ttu-id="e0018-127">В теле запроса добавьте представление объекта [organization](../resources/intune-onboarding-organization.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e0018-127">In the request body, supply a JSON representation for the [organization](../resources/intune-onboarding-organization.md) object.</span></span>

<span data-ttu-id="e0018-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="e0018-128">The following table shows the properties that are required when you create the [organization](../resources/intune-onboarding-organization.md).</span></span>

|<span data-ttu-id="e0018-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e0018-129">Property</span></span>|<span data-ttu-id="e0018-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e0018-130">Type</span></span>|<span data-ttu-id="e0018-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e0018-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0018-132">id</span><span class="sxs-lookup"><span data-stu-id="e0018-132">id</span></span>|<span data-ttu-id="e0018-133">String</span><span class="sxs-lookup"><span data-stu-id="e0018-133">String</span></span>|<span data-ttu-id="e0018-134">GUID объекта.</span><span class="sxs-lookup"><span data-stu-id="e0018-134">The GUID for the object.</span></span>|
|<span data-ttu-id="e0018-135">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="e0018-135">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="e0018-136">Мдмаусорити</span><span class="sxs-lookup"><span data-stu-id="e0018-136">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="e0018-137">Центр управления мобильными устройствами.</span><span class="sxs-lookup"><span data-stu-id="e0018-137">Mobile device management authority.</span></span> <span data-ttu-id="e0018-138">Возможные значения: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="e0018-138">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|
|<span data-ttu-id="e0018-139">Цертификатеконнекторсеттинг</span><span class="sxs-lookup"><span data-stu-id="e0018-139">certificateConnectorSetting</span></span>|[<span data-ttu-id="e0018-140">Цертификатеконнекторсеттинг</span><span class="sxs-lookup"><span data-stu-id="e0018-140">certificateConnectorSetting</span></span>](../resources/intune-onboarding-certificateconnectorsetting.md)|<span data-ttu-id="e0018-141">Параметр соединителя сертификатов.</span><span class="sxs-lookup"><span data-stu-id="e0018-141">Certificate connector setting.</span></span>|



## <a name="response"></a><span data-ttu-id="e0018-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0018-142">Response</span></span>
<span data-ttu-id="e0018-143">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [organization](../resources/intune-onboarding-organization.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e0018-143">If successful, this method returns a `200 OK` response code and an updated [organization](../resources/intune-onboarding-organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0018-144">Пример</span><span class="sxs-lookup"><span data-stu-id="e0018-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="e0018-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="e0018-145">Request</span></span>
<span data-ttu-id="e0018-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e0018-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e0018-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="e0018-147">Response</span></span>
<span data-ttu-id="e0018-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e0018-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




