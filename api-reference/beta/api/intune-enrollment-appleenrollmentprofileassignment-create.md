---
title: Создание Апплинроллментпрофилеассигнмент
description: Создание нового объекта Апплинроллментпрофилеассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: db6b389b4ac7169cf65a8293634c087543de4da4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48040772"
---
# <a name="create-appleenrollmentprofileassignment"></a><span data-ttu-id="a0e61-103">Создание Апплинроллментпрофилеассигнмент</span><span class="sxs-lookup"><span data-stu-id="a0e61-103">Create appleEnrollmentProfileAssignment</span></span>

<span data-ttu-id="a0e61-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0e61-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a0e61-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0e61-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a0e61-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a0e61-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0e61-107">Создание нового объекта [апплинроллментпрофилеассигнмент](../resources/intune-enrollment-appleenrollmentprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="a0e61-107">Create a new [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a0e61-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a0e61-108">Prerequisites</span></span>
<span data-ttu-id="a0e61-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0e61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0e61-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a0e61-111">Permission type</span></span>|<span data-ttu-id="a0e61-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a0e61-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0e61-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a0e61-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a0e61-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0e61-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a0e61-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a0e61-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0e61-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0e61-116">Not supported.</span></span>|
|<span data-ttu-id="a0e61-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a0e61-117">Application</span></span>|<span data-ttu-id="a0e61-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0e61-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0e61-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a0e61-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="a0e61-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a0e61-120">Request headers</span></span>
|<span data-ttu-id="a0e61-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a0e61-121">Header</span></span>|<span data-ttu-id="a0e61-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a0e61-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0e61-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a0e61-123">Authorization</span></span>|<span data-ttu-id="a0e61-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a0e61-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0e61-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a0e61-125">Accept</span></span>|<span data-ttu-id="a0e61-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a0e61-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0e61-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a0e61-127">Request body</span></span>
<span data-ttu-id="a0e61-128">В тексте запроса добавьте представление объекта Апплинроллментпрофилеассигнмент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a0e61-128">In the request body, supply a JSON representation for the appleEnrollmentProfileAssignment object.</span></span>

<span data-ttu-id="a0e61-129">В следующей таблице приведены свойства, необходимые при создании Апплинроллментпрофилеассигнмент.</span><span class="sxs-lookup"><span data-stu-id="a0e61-129">The following table shows the properties that are required when you create the appleEnrollmentProfileAssignment.</span></span>

|<span data-ttu-id="a0e61-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a0e61-130">Property</span></span>|<span data-ttu-id="a0e61-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a0e61-131">Type</span></span>|<span data-ttu-id="a0e61-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a0e61-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0e61-133">id</span><span class="sxs-lookup"><span data-stu-id="a0e61-133">id</span></span>|<span data-ttu-id="a0e61-134">Строка</span><span class="sxs-lookup"><span data-stu-id="a0e61-134">String</span></span>|<span data-ttu-id="a0e61-135">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="a0e61-135">The key of the assignment.</span></span>|
|<span data-ttu-id="a0e61-136">target</span><span class="sxs-lookup"><span data-stu-id="a0e61-136">target</span></span>|[<span data-ttu-id="a0e61-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a0e61-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="a0e61-138">Цель назначения для профиля развертывания, инициированного пользователем Apple.</span><span class="sxs-lookup"><span data-stu-id="a0e61-138">The assignment target for the Apple user initiated deployment profile.</span></span>|



## <a name="response"></a><span data-ttu-id="a0e61-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0e61-139">Response</span></span>
<span data-ttu-id="a0e61-140">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [апплинроллментпрофилеассигнмент](../resources/intune-enrollment-appleenrollmentprofileassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a0e61-140">If successful, this method returns a `201 Created` response code and a [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0e61-141">Пример</span><span class="sxs-lookup"><span data-stu-id="a0e61-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0e61-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="a0e61-142">Request</span></span>
<span data-ttu-id="a0e61-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a0e61-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}/assignments
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

### <a name="response"></a><span data-ttu-id="a0e61-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0e61-144">Response</span></span>
<span data-ttu-id="a0e61-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a0e61-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






