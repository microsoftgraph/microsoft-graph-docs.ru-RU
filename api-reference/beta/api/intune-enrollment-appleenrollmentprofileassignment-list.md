---
title: Список Апплинроллментпрофилеассигнментс
description: Список свойств и связей объектов Апплинроллментпрофилеассигнмент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 636e871495ddc1f5c141541a7de7f86658b011f8
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37525814"
---
# <a name="list-appleenrollmentprofileassignments"></a><span data-ttu-id="8d735-103">Список Апплинроллментпрофилеассигнментс</span><span class="sxs-lookup"><span data-stu-id="8d735-103">List appleEnrollmentProfileAssignments</span></span>

> <span data-ttu-id="8d735-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d735-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d735-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8d735-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d735-106">Список свойств и связей объектов [апплинроллментпрофилеассигнмент](../resources/intune-enrollment-appleenrollmentprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="8d735-106">List properties and relationships of the [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8d735-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8d735-107">Prerequisites</span></span>
<span data-ttu-id="8d735-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d735-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d735-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8d735-110">Permission type</span></span>|<span data-ttu-id="8d735-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8d735-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d735-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8d735-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8d735-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="8d735-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="8d735-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8d735-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d735-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d735-115">Not supported.</span></span>|
|<span data-ttu-id="8d735-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="8d735-116">Application</span></span>|<span data-ttu-id="8d735-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="8d735-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d735-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8d735-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="8d735-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8d735-119">Request headers</span></span>
|<span data-ttu-id="8d735-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8d735-120">Header</span></span>|<span data-ttu-id="8d735-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8d735-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d735-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8d735-122">Authorization</span></span>|<span data-ttu-id="8d735-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8d735-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d735-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8d735-124">Accept</span></span>|<span data-ttu-id="8d735-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8d735-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d735-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8d735-126">Request body</span></span>
<span data-ttu-id="8d735-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8d735-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d735-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="8d735-128">Response</span></span>
<span data-ttu-id="8d735-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [апплинроллментпрофилеассигнмент](../resources/intune-enrollment-appleenrollmentprofileassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8d735-129">If successful, this method returns a `200 OK` response code and a collection of [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d735-130">Пример</span><span class="sxs-lookup"><span data-stu-id="8d735-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="8d735-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d735-131">Request</span></span>
<span data-ttu-id="8d735-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8d735-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}/assignments
```

### <a name="response"></a><span data-ttu-id="8d735-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d735-133">Response</span></span>
<span data-ttu-id="8d735-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8d735-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






