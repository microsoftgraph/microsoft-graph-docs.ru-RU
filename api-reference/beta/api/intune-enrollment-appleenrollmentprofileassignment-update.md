---
title: Обновление Апплинроллментпрофилеассигнмент
description: Обновление свойств объекта Апплинроллментпрофилеассигнмент.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 66af75684e8f6cbb761ed70262e52cadb719fc76
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42813504"
---
# <a name="update-appleenrollmentprofileassignment"></a><span data-ttu-id="51580-103">Обновление Апплинроллментпрофилеассигнмент</span><span class="sxs-lookup"><span data-stu-id="51580-103">Update appleEnrollmentProfileAssignment</span></span>

> <span data-ttu-id="51580-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51580-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="51580-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="51580-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51580-106">Обновление свойств объекта [апплинроллментпрофилеассигнмент](../resources/intune-enrollment-appleenrollmentprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="51580-106">Update the properties of a [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51580-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="51580-107">Prerequisites</span></span>
<span data-ttu-id="51580-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51580-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51580-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51580-110">Permission type</span></span>|<span data-ttu-id="51580-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="51580-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51580-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51580-112">Delegated (work or school account)</span></span>|<span data-ttu-id="51580-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51580-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="51580-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51580-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51580-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51580-115">Not supported.</span></span>|
|<span data-ttu-id="51580-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="51580-116">Application</span></span>|<span data-ttu-id="51580-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51580-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="51580-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51580-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}/assignments/{appleEnrollmentProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="51580-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="51580-119">Request headers</span></span>
|<span data-ttu-id="51580-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="51580-120">Header</span></span>|<span data-ttu-id="51580-121">Значение</span><span class="sxs-lookup"><span data-stu-id="51580-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51580-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="51580-122">Authorization</span></span>|<span data-ttu-id="51580-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="51580-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51580-124">Accept</span><span class="sxs-lookup"><span data-stu-id="51580-124">Accept</span></span>|<span data-ttu-id="51580-125">application/json</span><span class="sxs-lookup"><span data-stu-id="51580-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51580-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="51580-126">Request body</span></span>
<span data-ttu-id="51580-127">В тексте запроса добавьте представление объекта [апплинроллментпрофилеассигнмент](../resources/intune-enrollment-appleenrollmentprofileassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="51580-127">In the request body, supply a JSON representation for the [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) object.</span></span>

<span data-ttu-id="51580-128">В следующей таблице приведены свойства, необходимые при создании [апплинроллментпрофилеассигнмент](../resources/intune-enrollment-appleenrollmentprofileassignment.md).</span><span class="sxs-lookup"><span data-stu-id="51580-128">The following table shows the properties that are required when you create the [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md).</span></span>

|<span data-ttu-id="51580-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="51580-129">Property</span></span>|<span data-ttu-id="51580-130">Тип</span><span class="sxs-lookup"><span data-stu-id="51580-130">Type</span></span>|<span data-ttu-id="51580-131">Описание</span><span class="sxs-lookup"><span data-stu-id="51580-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51580-132">id</span><span class="sxs-lookup"><span data-stu-id="51580-132">id</span></span>|<span data-ttu-id="51580-133">String</span><span class="sxs-lookup"><span data-stu-id="51580-133">String</span></span>|<span data-ttu-id="51580-134">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="51580-134">The key of the assignment.</span></span>|
|<span data-ttu-id="51580-135">target</span><span class="sxs-lookup"><span data-stu-id="51580-135">target</span></span>|[<span data-ttu-id="51580-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="51580-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="51580-137">Цель назначения для профиля развертывания, инициированного пользователем Apple.</span><span class="sxs-lookup"><span data-stu-id="51580-137">The assignment target for the Apple user initiated deployment profile.</span></span>|



## <a name="response"></a><span data-ttu-id="51580-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="51580-138">Response</span></span>
<span data-ttu-id="51580-139">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [апплинроллментпрофилеассигнмент](../resources/intune-enrollment-appleenrollmentprofileassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="51580-139">If successful, this method returns a `200 OK` response code and an updated [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51580-140">Пример</span><span class="sxs-lookup"><span data-stu-id="51580-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="51580-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="51580-141">Request</span></span>
<span data-ttu-id="51580-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51580-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}/assignments/{appleEnrollmentProfileAssignmentId}
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.appleEnrollmentProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="51580-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="51580-143">Response</span></span>
<span data-ttu-id="51580-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="51580-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.appleEnrollmentProfileAssignment",
  "id": "5b603771-3771-5b60-7137-605b7137605b",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




