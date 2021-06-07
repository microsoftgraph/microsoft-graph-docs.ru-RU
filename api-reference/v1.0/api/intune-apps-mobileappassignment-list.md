---
title: Перечисление объектов mobileAppAssignment
description: Список свойств и связей объектов mobileAppAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 709466f2c758c365c8ebb353481bcd77ad08738a
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754114"
---
# <a name="list-mobileappassignments"></a><span data-ttu-id="ba8a4-103">Перечисление объектов mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="ba8a4-103">List mobileAppAssignments</span></span>

<span data-ttu-id="ba8a4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba8a4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ba8a4-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ba8a4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba8a4-106">Список свойств и связей объектов [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ba8a4-106">List properties and relationships of the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ba8a4-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ba8a4-107">Prerequisites</span></span>
<span data-ttu-id="ba8a4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba8a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba8a4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba8a4-110">Permission type</span></span>|<span data-ttu-id="ba8a4-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ba8a4-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba8a4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba8a4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ba8a4-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba8a4-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ba8a4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba8a4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba8a4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba8a4-115">Not supported.</span></span>|
|<span data-ttu-id="ba8a4-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="ba8a4-116">Application</span></span>|<span data-ttu-id="ba8a4-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba8a4-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba8a4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba8a4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="ba8a4-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ba8a4-119">Request headers</span></span>
|<span data-ttu-id="ba8a4-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ba8a4-120">Header</span></span>|<span data-ttu-id="ba8a4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ba8a4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ba8a4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba8a4-122">Authorization</span></span>|<span data-ttu-id="ba8a4-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ba8a4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ba8a4-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ba8a4-124">Accept</span></span>|<span data-ttu-id="ba8a4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ba8a4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba8a4-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ba8a4-126">Request body</span></span>
<span data-ttu-id="ba8a4-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ba8a4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba8a4-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba8a4-128">Response</span></span>
<span data-ttu-id="ba8a4-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ba8a4-129">If successful, this method returns a `200 OK` response code and a collection of [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba8a4-130">Пример</span><span class="sxs-lookup"><span data-stu-id="ba8a4-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ba8a4-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="ba8a4-131">Request</span></span>
<span data-ttu-id="ba8a4-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ba8a4-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

### <a name="response"></a><span data-ttu-id="ba8a4-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba8a4-133">Response</span></span>
<span data-ttu-id="ba8a4-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ba8a4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 446

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppAssignment",
      "id": "591620b7-20b7-5916-b720-1659b7201659",
      "intent": "required",
      "target": {
        "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget"
      },
      "settings": {
        "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings",
        "vpnConfigurationId": "Vpn Configuration Id value"
      }
    }
  ]
}
```




