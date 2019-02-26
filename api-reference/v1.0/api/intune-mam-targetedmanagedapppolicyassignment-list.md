---
title: Перечисление объектов targetedManagedAppPolicyAssignment
description: Список свойств и связей объектов targetedManagedAppPolicyAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 10b1e91d3f1582988b0a1d18e0962eff50521973
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254599"
---
# <a name="list-targetedmanagedapppolicyassignments"></a><span data-ttu-id="6acbc-103">Перечисление объектов targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="6acbc-103">List targetedManagedAppPolicyAssignments</span></span>

> <span data-ttu-id="6acbc-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6acbc-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6acbc-105">Список свойств и связей объектов [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6acbc-105">List properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6acbc-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6acbc-106">Prerequisites</span></span>
<span data-ttu-id="6acbc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6acbc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6acbc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6acbc-109">Permission type</span></span>|<span data-ttu-id="6acbc-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6acbc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6acbc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6acbc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6acbc-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6acbc-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="6acbc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6acbc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6acbc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6acbc-114">Not supported.</span></span>|
|<span data-ttu-id="6acbc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6acbc-115">Application</span></span>|<span data-ttu-id="6acbc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6acbc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6acbc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6acbc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments
GET /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/assignments
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assignments
GET /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/assignments
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="6acbc-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6acbc-118">Request headers</span></span>
|<span data-ttu-id="6acbc-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6acbc-119">Header</span></span>|<span data-ttu-id="6acbc-120">Значение</span><span class="sxs-lookup"><span data-stu-id="6acbc-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6acbc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6acbc-121">Authorization</span></span>|<span data-ttu-id="6acbc-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6acbc-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6acbc-123">Accept</span><span class="sxs-lookup"><span data-stu-id="6acbc-123">Accept</span></span>|<span data-ttu-id="6acbc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6acbc-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6acbc-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6acbc-125">Request body</span></span>
<span data-ttu-id="6acbc-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6acbc-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6acbc-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="6acbc-127">Response</span></span>
<span data-ttu-id="6acbc-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6acbc-128">If successful, this method returns a `200 OK` response code and a collection of [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6acbc-129">Пример</span><span class="sxs-lookup"><span data-stu-id="6acbc-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="6acbc-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="6acbc-130">Request</span></span>
<span data-ttu-id="6acbc-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6acbc-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments
```

### <a name="response"></a><span data-ttu-id="6acbc-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="6acbc-132">Response</span></span>
<span data-ttu-id="6acbc-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="6acbc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 276

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
      "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```



