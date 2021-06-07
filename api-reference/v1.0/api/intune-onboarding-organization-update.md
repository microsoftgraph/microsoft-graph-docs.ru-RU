---
title: Обновление организации
description: Обновление свойств объекта organization.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b66eea4b04f21f85aa38b9777a17cb73e87fe6fc
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751463"
---
# <a name="update-organization"></a><span data-ttu-id="45a4b-103">Обновление организации</span><span class="sxs-lookup"><span data-stu-id="45a4b-103">Update organization</span></span>

<span data-ttu-id="45a4b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45a4b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="45a4b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="45a4b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45a4b-106">Обновление свойств объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="45a4b-106">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="45a4b-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="45a4b-107">Prerequisites</span></span>
<span data-ttu-id="45a4b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45a4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45a4b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="45a4b-110">Permission type</span></span>|<span data-ttu-id="45a4b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="45a4b-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45a4b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="45a4b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="45a4b-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45a4b-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="45a4b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="45a4b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45a4b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45a4b-115">Not supported.</span></span>|
|<span data-ttu-id="45a4b-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="45a4b-116">Application</span></span>|<span data-ttu-id="45a4b-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45a4b-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="45a4b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="45a4b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /organization/{organizationId}
```

## <a name="request-headers"></a><span data-ttu-id="45a4b-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="45a4b-119">Request headers</span></span>
|<span data-ttu-id="45a4b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="45a4b-120">Header</span></span>|<span data-ttu-id="45a4b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="45a4b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45a4b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="45a4b-122">Authorization</span></span>|<span data-ttu-id="45a4b-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="45a4b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45a4b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="45a4b-124">Accept</span></span>|<span data-ttu-id="45a4b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="45a4b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45a4b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="45a4b-126">Request body</span></span>
<span data-ttu-id="45a4b-127">В теле запроса добавьте представление объекта [organization](../resources/intune-onboarding-organization.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="45a4b-127">In the request body, supply a JSON representation for the [organization](../resources/intune-onboarding-organization.md) object.</span></span>

<span data-ttu-id="45a4b-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="45a4b-128">The following table shows the properties that are required when you create the [organization](../resources/intune-onboarding-organization.md).</span></span>

|<span data-ttu-id="45a4b-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="45a4b-129">Property</span></span>|<span data-ttu-id="45a4b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="45a4b-130">Type</span></span>|<span data-ttu-id="45a4b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="45a4b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45a4b-132">id</span><span class="sxs-lookup"><span data-stu-id="45a4b-132">id</span></span>|<span data-ttu-id="45a4b-133">String</span><span class="sxs-lookup"><span data-stu-id="45a4b-133">String</span></span>|<span data-ttu-id="45a4b-134">GUID объекта.</span><span class="sxs-lookup"><span data-stu-id="45a4b-134">The GUID for the object.</span></span>|
|<span data-ttu-id="45a4b-135">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="45a4b-135">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="45a4b-136">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="45a4b-136">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="45a4b-137">Центр управления мобильными устройствами.</span><span class="sxs-lookup"><span data-stu-id="45a4b-137">Mobile device management authority.</span></span> <span data-ttu-id="45a4b-138">Возможные значения: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="45a4b-138">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|



## <a name="response"></a><span data-ttu-id="45a4b-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="45a4b-139">Response</span></span>
<span data-ttu-id="45a4b-140">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [organization](../resources/intune-onboarding-organization.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="45a4b-140">If successful, this method returns a `200 OK` response code and an updated [organization](../resources/intune-onboarding-organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45a4b-141">Пример</span><span class="sxs-lookup"><span data-stu-id="45a4b-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="45a4b-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="45a4b-142">Request</span></span>
<span data-ttu-id="45a4b-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="45a4b-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/organization/{organizationId}
Content-type: application/json
Content-length: 102

{
  "@odata.type": "#microsoft.graph.organization",
  "mobileDeviceManagementAuthority": "intune"
}
```

### <a name="response"></a><span data-ttu-id="45a4b-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="45a4b-144">Response</span></span>
<span data-ttu-id="45a4b-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="45a4b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 151

{
  "@odata.type": "#microsoft.graph.organization",
  "id": "9efe224a-224a-9efe-4a22-fe9e4a22fe9e",
  "mobileDeviceManagementAuthority": "intune"
}
```




