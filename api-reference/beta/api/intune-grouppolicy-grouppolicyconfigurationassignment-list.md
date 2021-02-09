---
title: Список groupPolicyConfigurationAssignments
description: Список свойств и связей объектов groupPolicyConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 54601807802df51ef984761e8558795d2b11abb7
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153937"
---
# <a name="list-grouppolicyconfigurationassignments"></a><span data-ttu-id="390b8-103">Список groupPolicyConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="390b8-103">List groupPolicyConfigurationAssignments</span></span>

<span data-ttu-id="390b8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="390b8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="390b8-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="390b8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="390b8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="390b8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="390b8-107">Список свойств и связей объектов [groupPolicyConfigurationAssignment.](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="390b8-107">List properties and relationships of the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="390b8-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="390b8-108">Prerequisites</span></span>
<span data-ttu-id="390b8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="390b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="390b8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="390b8-111">Permission type</span></span>|<span data-ttu-id="390b8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="390b8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="390b8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="390b8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="390b8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="390b8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="390b8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="390b8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="390b8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="390b8-116">Not supported.</span></span>|
|<span data-ttu-id="390b8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="390b8-117">Application</span></span>|<span data-ttu-id="390b8-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="390b8-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="390b8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="390b8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="390b8-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="390b8-120">Request headers</span></span>
|<span data-ttu-id="390b8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="390b8-121">Header</span></span>|<span data-ttu-id="390b8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="390b8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="390b8-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="390b8-123">Authorization</span></span>|<span data-ttu-id="390b8-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="390b8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="390b8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="390b8-125">Accept</span></span>|<span data-ttu-id="390b8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="390b8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="390b8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="390b8-127">Request body</span></span>
<span data-ttu-id="390b8-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="390b8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="390b8-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="390b8-129">Response</span></span>
<span data-ttu-id="390b8-130">В случае успешного выполнения этот метод возвращает код отклика и коллекцию объектов `200 OK` [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="390b8-130">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="390b8-131">Пример</span><span class="sxs-lookup"><span data-stu-id="390b8-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="390b8-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="390b8-132">Request</span></span>
<span data-ttu-id="390b8-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="390b8-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="390b8-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="390b8-134">Response</span></span>
<span data-ttu-id="390b8-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="390b8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 575

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
      "id": "2a4161e9-61e9-2a41-e961-412ae961412a",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      }
    }
  ]
}
```




