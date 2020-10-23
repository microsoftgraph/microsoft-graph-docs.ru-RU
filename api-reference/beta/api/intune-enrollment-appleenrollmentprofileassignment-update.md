---
title: Обновление Апплинроллментпрофилеассигнмент
description: Обновление свойств объекта Апплинроллментпрофилеассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f04da100fd863e87fea64f5dc7f0cfac0bdf8cb5
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48733394"
---
# <a name="update-appleenrollmentprofileassignment"></a><span data-ttu-id="07734-103">Обновление Апплинроллментпрофилеассигнмент</span><span class="sxs-lookup"><span data-stu-id="07734-103">Update appleEnrollmentProfileAssignment</span></span>

<span data-ttu-id="07734-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07734-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="07734-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07734-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="07734-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="07734-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07734-107">Обновление свойств объекта [апплинроллментпрофилеассигнмент](../resources/intune-enrollment-appleenrollmentprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="07734-107">Update the properties of a [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="07734-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="07734-108">Prerequisites</span></span>
<span data-ttu-id="07734-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07734-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07734-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="07734-111">Permission type</span></span>|<span data-ttu-id="07734-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="07734-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07734-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="07734-113">Delegated (work or school account)</span></span>|<span data-ttu-id="07734-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07734-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="07734-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="07734-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07734-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07734-116">Not supported.</span></span>|
|<span data-ttu-id="07734-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="07734-117">Application</span></span>|<span data-ttu-id="07734-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07734-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="07734-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="07734-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}/assignments/{appleEnrollmentProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="07734-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="07734-120">Request headers</span></span>
|<span data-ttu-id="07734-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="07734-121">Header</span></span>|<span data-ttu-id="07734-122">Значение</span><span class="sxs-lookup"><span data-stu-id="07734-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="07734-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="07734-123">Authorization</span></span>|<span data-ttu-id="07734-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="07734-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="07734-125">Accept</span><span class="sxs-lookup"><span data-stu-id="07734-125">Accept</span></span>|<span data-ttu-id="07734-126">application/json</span><span class="sxs-lookup"><span data-stu-id="07734-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07734-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="07734-127">Request body</span></span>
<span data-ttu-id="07734-128">В тексте запроса добавьте представление объекта [апплинроллментпрофилеассигнмент](../resources/intune-enrollment-appleenrollmentprofileassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="07734-128">In the request body, supply a JSON representation for the [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) object.</span></span>

<span data-ttu-id="07734-129">В следующей таблице приведены свойства, необходимые при создании [апплинроллментпрофилеассигнмент](../resources/intune-enrollment-appleenrollmentprofileassignment.md).</span><span class="sxs-lookup"><span data-stu-id="07734-129">The following table shows the properties that are required when you create the [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md).</span></span>

|<span data-ttu-id="07734-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="07734-130">Property</span></span>|<span data-ttu-id="07734-131">Тип</span><span class="sxs-lookup"><span data-stu-id="07734-131">Type</span></span>|<span data-ttu-id="07734-132">Описание</span><span class="sxs-lookup"><span data-stu-id="07734-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07734-133">id</span><span class="sxs-lookup"><span data-stu-id="07734-133">id</span></span>|<span data-ttu-id="07734-134">Строка</span><span class="sxs-lookup"><span data-stu-id="07734-134">String</span></span>|<span data-ttu-id="07734-135">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="07734-135">The key of the assignment.</span></span>|
|<span data-ttu-id="07734-136">target</span><span class="sxs-lookup"><span data-stu-id="07734-136">target</span></span>|[<span data-ttu-id="07734-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="07734-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="07734-138">Цель назначения для профиля развертывания, инициированного пользователем Apple.</span><span class="sxs-lookup"><span data-stu-id="07734-138">The assignment target for the Apple user initiated deployment profile.</span></span>|



## <a name="response"></a><span data-ttu-id="07734-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="07734-139">Response</span></span>
<span data-ttu-id="07734-140">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [апплинроллментпрофилеассигнмент](../resources/intune-enrollment-appleenrollmentprofileassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="07734-140">If successful, this method returns a `200 OK` response code and an updated [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07734-141">Пример</span><span class="sxs-lookup"><span data-stu-id="07734-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="07734-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="07734-142">Request</span></span>
<span data-ttu-id="07734-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="07734-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}/assignments/{appleEnrollmentProfileAssignmentId}
Content-type: application/json
Content-length: 327

{
  "@odata.type": "#microsoft.graph.appleEnrollmentProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```

### <a name="response"></a><span data-ttu-id="07734-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="07734-144">Response</span></span>
<span data-ttu-id="07734-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="07734-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 376

{
  "@odata.type": "#microsoft.graph.appleEnrollmentProfileAssignment",
  "id": "5b603771-3771-5b60-7137-605b7137605b",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```





