---
title: Get targetedManagedAppPolicyAssignment
description: Чтение свойств и связей объекта targetedManagedAppPolicyAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 940dcd331bcc05cde7b65aabaad338d6d94b7391
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33903035"
---
# <a name="get-targetedmanagedapppolicyassignment"></a><span data-ttu-id="74cf2-103">Get targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="74cf2-103">Get targetedManagedAppPolicyAssignment</span></span>

> <span data-ttu-id="74cf2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74cf2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="74cf2-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="74cf2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74cf2-106">Чтение свойств и связей объекта [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="74cf2-106">Read properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="74cf2-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="74cf2-107">Prerequisites</span></span>
<span data-ttu-id="74cf2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74cf2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74cf2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="74cf2-110">Permission type</span></span>|<span data-ttu-id="74cf2-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="74cf2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74cf2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="74cf2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="74cf2-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="74cf2-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="74cf2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="74cf2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74cf2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74cf2-115">Not supported.</span></span>|
|<span data-ttu-id="74cf2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="74cf2-116">Application</span></span>|<span data-ttu-id="74cf2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74cf2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="74cf2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="74cf2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
GET /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assignments/{targetedManagedAppPolicyAssignmentId}
GET /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/assignments/{targetedManagedAppPolicyAssignmentId}
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/assignments/{targetedManagedAppPolicyAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="74cf2-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="74cf2-119">Optional query parameters</span></span>
<span data-ttu-id="74cf2-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="74cf2-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="74cf2-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="74cf2-121">Request headers</span></span>
|<span data-ttu-id="74cf2-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="74cf2-122">Header</span></span>|<span data-ttu-id="74cf2-123">Значение</span><span class="sxs-lookup"><span data-stu-id="74cf2-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74cf2-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="74cf2-124">Authorization</span></span>|<span data-ttu-id="74cf2-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="74cf2-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74cf2-126">Accept</span><span class="sxs-lookup"><span data-stu-id="74cf2-126">Accept</span></span>|<span data-ttu-id="74cf2-127">application/json</span><span class="sxs-lookup"><span data-stu-id="74cf2-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74cf2-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="74cf2-128">Request body</span></span>
<span data-ttu-id="74cf2-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="74cf2-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="74cf2-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="74cf2-130">Response</span></span>
<span data-ttu-id="74cf2-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="74cf2-131">If successful, this method returns a `200 OK` response code and [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74cf2-132">Пример</span><span class="sxs-lookup"><span data-stu-id="74cf2-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="74cf2-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="74cf2-133">Request</span></span>
<span data-ttu-id="74cf2-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="74cf2-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
```

### <a name="response"></a><span data-ttu-id="74cf2-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="74cf2-135">Response</span></span>
<span data-ttu-id="74cf2-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="74cf2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 252

{
  "value": {
    "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
    "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```




