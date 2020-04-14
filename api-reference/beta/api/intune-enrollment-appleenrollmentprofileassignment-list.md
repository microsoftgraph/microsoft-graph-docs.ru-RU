---
title: Список Апплинроллментпрофилеассигнментс
description: Список свойств и связей объектов Апплинроллментпрофилеассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 264b94a856cbe3818e8ca61a2d046d5a28c8ee99
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43321239"
---
# <a name="list-appleenrollmentprofileassignments"></a><span data-ttu-id="b1620-103">Список Апплинроллментпрофилеассигнментс</span><span class="sxs-lookup"><span data-stu-id="b1620-103">List appleEnrollmentProfileAssignments</span></span>

<span data-ttu-id="b1620-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1620-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b1620-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1620-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1620-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b1620-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1620-107">Список свойств и связей объектов [апплинроллментпрофилеассигнмент](../resources/intune-enrollment-appleenrollmentprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="b1620-107">List properties and relationships of the [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b1620-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b1620-108">Prerequisites</span></span>
<span data-ttu-id="b1620-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1620-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1620-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b1620-111">Permission type</span></span>|<span data-ttu-id="b1620-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b1620-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1620-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b1620-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b1620-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b1620-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="b1620-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b1620-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1620-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1620-116">Not supported.</span></span>|
|<span data-ttu-id="b1620-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b1620-117">Application</span></span>|<span data-ttu-id="b1620-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b1620-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1620-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1620-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="b1620-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b1620-120">Request headers</span></span>
|<span data-ttu-id="b1620-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b1620-121">Header</span></span>|<span data-ttu-id="b1620-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b1620-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1620-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b1620-123">Authorization</span></span>|<span data-ttu-id="b1620-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1620-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1620-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b1620-125">Accept</span></span>|<span data-ttu-id="b1620-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b1620-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1620-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b1620-127">Request body</span></span>
<span data-ttu-id="b1620-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b1620-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b1620-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="b1620-129">Response</span></span>
<span data-ttu-id="b1620-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [апплинроллментпрофилеассигнмент](../resources/intune-enrollment-appleenrollmentprofileassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b1620-130">If successful, this method returns a `200 OK` response code and a collection of [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1620-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b1620-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b1620-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1620-132">Request</span></span>
<span data-ttu-id="b1620-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b1620-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}/assignments
```

### <a name="response"></a><span data-ttu-id="b1620-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1620-134">Response</span></span>
<span data-ttu-id="b1620-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b1620-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 274

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.appleEnrollmentProfileAssignment",
      "id": "5b603771-3771-5b60-7137-605b7137605b",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```



