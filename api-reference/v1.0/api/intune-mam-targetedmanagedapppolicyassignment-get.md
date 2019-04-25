---
title: Get targetedManagedAppPolicyAssignment
description: Чтение свойств и связей объекта targetedManagedAppPolicyAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4b3ca412f0b6b56579672cc225883dfca0a69781
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583153"
---
# <a name="get-targetedmanagedapppolicyassignment"></a><span data-ttu-id="8207e-103">Get targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="8207e-103">Get targetedManagedAppPolicyAssignment</span></span>

> <span data-ttu-id="8207e-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8207e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8207e-105">Чтение свойств и связей объекта [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8207e-105">Read properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8207e-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="8207e-106">Prerequisites</span></span>
<span data-ttu-id="8207e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8207e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8207e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8207e-109">Permission type</span></span>|<span data-ttu-id="8207e-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8207e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8207e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8207e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8207e-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8207e-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="8207e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8207e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8207e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8207e-114">Not supported.</span></span>|
|<span data-ttu-id="8207e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8207e-115">Application</span></span>|<span data-ttu-id="8207e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8207e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8207e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8207e-117">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="8207e-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8207e-118">Optional query parameters</span></span>
<span data-ttu-id="8207e-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8207e-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8207e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8207e-120">Request headers</span></span>
|<span data-ttu-id="8207e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8207e-121">Header</span></span>|<span data-ttu-id="8207e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8207e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8207e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8207e-123">Authorization</span></span>|<span data-ttu-id="8207e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8207e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8207e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8207e-125">Accept</span></span>|<span data-ttu-id="8207e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8207e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8207e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8207e-127">Request body</span></span>
<span data-ttu-id="8207e-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8207e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8207e-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="8207e-129">Response</span></span>
<span data-ttu-id="8207e-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8207e-130">If successful, this method returns a `200 OK` response code and [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8207e-131">Пример</span><span class="sxs-lookup"><span data-stu-id="8207e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="8207e-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8207e-132">Request</span></span>
<span data-ttu-id="8207e-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8207e-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
```

### <a name="response"></a><span data-ttu-id="8207e-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="8207e-134">Response</span></span>
<span data-ttu-id="8207e-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8207e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



