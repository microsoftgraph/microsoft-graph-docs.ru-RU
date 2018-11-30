---
title: Обновление организации
description: Обновление свойств объекта organization.
ms.openlocfilehash: 32e9cf3cccecf0a763d20b201040d79d4442cdfe
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082801"
---
# <a name="update-organization"></a><span data-ttu-id="a8bb0-103">Обновление организации</span><span class="sxs-lookup"><span data-stu-id="a8bb0-103">Update organization</span></span>

> <span data-ttu-id="a8bb0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a8bb0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a8bb0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8bb0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a8bb0-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a8bb0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a8bb0-107">Обновление свойств объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="a8bb0-107">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a8bb0-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a8bb0-108">Prerequisites</span></span>
<span data-ttu-id="a8bb0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8bb0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8bb0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a8bb0-111">Permission type</span></span>|<span data-ttu-id="a8bb0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a8bb0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8bb0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a8bb0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a8bb0-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8bb0-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a8bb0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a8bb0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8bb0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8bb0-116">Not supported.</span></span>|
|<span data-ttu-id="a8bb0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a8bb0-117">Application</span></span>|<span data-ttu-id="a8bb0-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8bb0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8bb0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a8bb0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /organization/{organizationId}
```

## <a name="request-headers"></a><span data-ttu-id="a8bb0-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a8bb0-120">Request headers</span></span>
|<span data-ttu-id="a8bb0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a8bb0-121">Header</span></span>|<span data-ttu-id="a8bb0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a8bb0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8bb0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8bb0-123">Authorization</span></span>|<span data-ttu-id="a8bb0-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a8bb0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a8bb0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a8bb0-125">Accept</span></span>|<span data-ttu-id="a8bb0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a8bb0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8bb0-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a8bb0-127">Request body</span></span>
<span data-ttu-id="a8bb0-128">В теле запроса добавьте представление объекта [organization](../resources/intune-onboarding-organization.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a8bb0-128">In the request body, supply a JSON representation for the [organization](../resources/intune-onboarding-organization.md) object.</span></span>

<span data-ttu-id="a8bb0-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="a8bb0-129">The following table shows the properties that are required when you create the [organization](../resources/intune-onboarding-organization.md).</span></span>

|<span data-ttu-id="a8bb0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a8bb0-130">Property</span></span>|<span data-ttu-id="a8bb0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a8bb0-131">Type</span></span>|<span data-ttu-id="a8bb0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a8bb0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8bb0-133">id</span><span class="sxs-lookup"><span data-stu-id="a8bb0-133">id</span></span>|<span data-ttu-id="a8bb0-134">String</span><span class="sxs-lookup"><span data-stu-id="a8bb0-134">String</span></span>|<span data-ttu-id="a8bb0-135">GUID объекта.</span><span class="sxs-lookup"><span data-stu-id="a8bb0-135">The GUID for the object.</span></span>|
|<span data-ttu-id="a8bb0-136">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="a8bb0-136">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="a8bb0-137">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="a8bb0-137">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="a8bb0-138">Центр управления мобильными устройствами.</span><span class="sxs-lookup"><span data-stu-id="a8bb0-138">Mobile device management authority.</span></span> <span data-ttu-id="a8bb0-139">Возможные значения: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="a8bb0-139">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|
|<span data-ttu-id="a8bb0-140">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="a8bb0-140">certificateConnectorSetting</span></span>|[<span data-ttu-id="a8bb0-141">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="a8bb0-141">certificateConnectorSetting</span></span>](../resources/intune-onboarding-certificateconnectorsetting.md)|<span data-ttu-id="a8bb0-142">Параметр соединителя сертификата.</span><span class="sxs-lookup"><span data-stu-id="a8bb0-142">Certificate connector setting.</span></span>|



## <a name="response"></a><span data-ttu-id="a8bb0-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8bb0-143">Response</span></span>
<span data-ttu-id="a8bb0-144">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [organization](../resources/intune-onboarding-organization.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a8bb0-144">If successful, this method returns a `200 OK` response code and an updated [organization](../resources/intune-onboarding-organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8bb0-145">Пример</span><span class="sxs-lookup"><span data-stu-id="a8bb0-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="a8bb0-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="a8bb0-146">Request</span></span>
<span data-ttu-id="a8bb0-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a8bb0-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/organization/{organizationId}
Content-type: application/json
Content-length: 441

{
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

### <a name="response"></a><span data-ttu-id="a8bb0-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="a8bb0-148">Response</span></span>
<span data-ttu-id="a8bb0-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="a8bb0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





