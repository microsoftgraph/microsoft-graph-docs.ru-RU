---
title: Создание windowsQualityUpdateProfileAssignment
description: Создайте новый объект WindowsQualityUpdateProfileAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b4c1c7feb40af06d8baefcfbc7642c828114e208
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51156172"
---
# <a name="create-windowsqualityupdateprofileassignment"></a><span data-ttu-id="d385c-103">Создание windowsQualityUpdateProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="d385c-103">Create windowsQualityUpdateProfileAssignment</span></span>

<span data-ttu-id="d385c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d385c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d385c-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d385c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d385c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d385c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d385c-107">Создайте [новый объект WindowsQualityUpdateProfileAssignment.](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md)</span><span class="sxs-lookup"><span data-stu-id="d385c-107">Create a new [windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d385c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d385c-108">Prerequisites</span></span>
<span data-ttu-id="d385c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d385c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d385c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d385c-111">Permission type</span></span>|<span data-ttu-id="d385c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d385c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d385c-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d385c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d385c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d385c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d385c-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d385c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d385c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d385c-116">Not supported.</span></span>|
|<span data-ttu-id="d385c-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="d385c-117">Application</span></span>|<span data-ttu-id="d385c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d385c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d385c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d385c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsQualityUpdateProfiles/{windowsQualityUpdateProfileId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="d385c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d385c-120">Request headers</span></span>
|<span data-ttu-id="d385c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d385c-121">Header</span></span>|<span data-ttu-id="d385c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d385c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d385c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d385c-123">Authorization</span></span>|<span data-ttu-id="d385c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d385c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d385c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d385c-125">Accept</span></span>|<span data-ttu-id="d385c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d385c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d385c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d385c-127">Request body</span></span>
<span data-ttu-id="d385c-128">В теле запроса поставляем представление JSON для объекта WindowsQualityUpdateProfileAssignment.</span><span class="sxs-lookup"><span data-stu-id="d385c-128">In the request body, supply a JSON representation for the windowsQualityUpdateProfileAssignment object.</span></span>

<span data-ttu-id="d385c-129">В следующей таблице показаны свойства, необходимые при создании windowsQualityUpdateProfileAssignment.</span><span class="sxs-lookup"><span data-stu-id="d385c-129">The following table shows the properties that are required when you create the windowsQualityUpdateProfileAssignment.</span></span>

|<span data-ttu-id="d385c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d385c-130">Property</span></span>|<span data-ttu-id="d385c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d385c-131">Type</span></span>|<span data-ttu-id="d385c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d385c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d385c-133">id</span><span class="sxs-lookup"><span data-stu-id="d385c-133">id</span></span>|<span data-ttu-id="d385c-134">Строка</span><span class="sxs-lookup"><span data-stu-id="d385c-134">String</span></span>|<span data-ttu-id="d385c-135">Идентификатор сущности</span><span class="sxs-lookup"><span data-stu-id="d385c-135">The Identifier of the entity</span></span>|
|<span data-ttu-id="d385c-136">target</span><span class="sxs-lookup"><span data-stu-id="d385c-136">target</span></span>|[<span data-ttu-id="d385c-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d385c-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="d385c-138">Цель назначения, назначенная профилем обновления функций.</span><span class="sxs-lookup"><span data-stu-id="d385c-138">The assignment target that the feature update profile is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="d385c-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="d385c-139">Response</span></span>
<span data-ttu-id="d385c-140">В случае успешного выполнения этот метод возвращает код отклика и `201 Created` [объект windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d385c-140">If successful, this method returns a `201 Created` response code and a [windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d385c-141">Пример</span><span class="sxs-lookup"><span data-stu-id="d385c-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="d385c-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="d385c-142">Request</span></span>
<span data-ttu-id="d385c-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d385c-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsQualityUpdateProfiles/{windowsQualityUpdateProfileId}/assignments
Content-type: application/json
Content-length: 344

{
  "@odata.type": "#microsoft.graph.windowsQualityUpdateProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```

### <a name="response"></a><span data-ttu-id="d385c-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="d385c-144">Response</span></span>
<span data-ttu-id="d385c-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d385c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 393

{
  "@odata.type": "#microsoft.graph.windowsQualityUpdateProfileAssignment",
  "id": "0c3a8422-8422-0c3a-2284-3a0c22843a0c",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```




