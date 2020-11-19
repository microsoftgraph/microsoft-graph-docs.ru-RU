---
title: Обновление Интунебрандингпрофилеассигнмент
description: Обновление свойств объекта Интунебрандингпрофилеассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: df1dd4848ce77500cfa428dd5f9bb4ce4ad8d6f1
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49261526"
---
# <a name="update-intunebrandingprofileassignment"></a><span data-ttu-id="dcfcd-103">Обновление Интунебрандингпрофилеассигнмент</span><span class="sxs-lookup"><span data-stu-id="dcfcd-103">Update intuneBrandingProfileAssignment</span></span>

<span data-ttu-id="dcfcd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dcfcd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dcfcd-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dcfcd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dcfcd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dcfcd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dcfcd-107">Обновление свойств объекта [интунебрандингпрофилеассигнмент](../resources/intune-wip-intunebrandingprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="dcfcd-107">Update the properties of a [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dcfcd-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="dcfcd-108">Prerequisites</span></span>
<span data-ttu-id="dcfcd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dcfcd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dcfcd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dcfcd-111">Permission type</span></span>|<span data-ttu-id="dcfcd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dcfcd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dcfcd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dcfcd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dcfcd-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dcfcd-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="dcfcd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dcfcd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dcfcd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dcfcd-116">Not supported.</span></span>|
|<span data-ttu-id="dcfcd-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="dcfcd-117">Application</span></span>|<span data-ttu-id="dcfcd-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dcfcd-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dcfcd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dcfcd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments/{intuneBrandingProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="dcfcd-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="dcfcd-120">Request headers</span></span>
|<span data-ttu-id="dcfcd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dcfcd-121">Header</span></span>|<span data-ttu-id="dcfcd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="dcfcd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dcfcd-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dcfcd-123">Authorization</span></span>|<span data-ttu-id="dcfcd-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dcfcd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dcfcd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="dcfcd-125">Accept</span></span>|<span data-ttu-id="dcfcd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dcfcd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dcfcd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dcfcd-127">Request body</span></span>
<span data-ttu-id="dcfcd-128">В тексте запроса добавьте представление объекта [интунебрандингпрофилеассигнмент](../resources/intune-wip-intunebrandingprofileassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dcfcd-128">In the request body, supply a JSON representation for the [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object.</span></span>

<span data-ttu-id="dcfcd-129">В следующей таблице приведены свойства, необходимые при создании [интунебрандингпрофилеассигнмент](../resources/intune-wip-intunebrandingprofileassignment.md).</span><span class="sxs-lookup"><span data-stu-id="dcfcd-129">The following table shows the properties that are required when you create the [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md).</span></span>

|<span data-ttu-id="dcfcd-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="dcfcd-130">Property</span></span>|<span data-ttu-id="dcfcd-131">Тип</span><span class="sxs-lookup"><span data-stu-id="dcfcd-131">Type</span></span>|<span data-ttu-id="dcfcd-132">Описание</span><span class="sxs-lookup"><span data-stu-id="dcfcd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dcfcd-133">id</span><span class="sxs-lookup"><span data-stu-id="dcfcd-133">id</span></span>|<span data-ttu-id="dcfcd-134">String</span><span class="sxs-lookup"><span data-stu-id="dcfcd-134">String</span></span>|<span data-ttu-id="dcfcd-135">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="dcfcd-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="dcfcd-136">target</span><span class="sxs-lookup"><span data-stu-id="dcfcd-136">target</span></span>|[<span data-ttu-id="dcfcd-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="dcfcd-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="dcfcd-138">Цель назначения, которой назначен профиль фирменной символики.</span><span class="sxs-lookup"><span data-stu-id="dcfcd-138">Assignment target that the branding profile is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="dcfcd-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="dcfcd-139">Response</span></span>
<span data-ttu-id="dcfcd-140">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [интунебрандингпрофилеассигнмент](../resources/intune-wip-intunebrandingprofileassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dcfcd-140">If successful, this method returns a `200 OK` response code and an updated [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dcfcd-141">Пример</span><span class="sxs-lookup"><span data-stu-id="dcfcd-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="dcfcd-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="dcfcd-142">Request</span></span>
<span data-ttu-id="dcfcd-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dcfcd-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments/{intuneBrandingProfileAssignmentId}
Content-type: application/json
Content-length: 326

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```

### <a name="response"></a><span data-ttu-id="dcfcd-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="dcfcd-144">Response</span></span>
<span data-ttu-id="dcfcd-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dcfcd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 375

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
  "id": "ee38a117-a117-ee38-17a1-38ee17a138ee",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```




