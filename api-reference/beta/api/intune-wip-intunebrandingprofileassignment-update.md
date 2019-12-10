---
title: Обновление Интунебрандингпрофилеассигнмент
description: Обновление свойств объекта Интунебрандингпрофилеассигнмент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bfe7f131346c2c272905aafe36444e9b5429709e
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39938224"
---
# <a name="update-intunebrandingprofileassignment"></a><span data-ttu-id="e0b8c-103">Обновление Интунебрандингпрофилеассигнмент</span><span class="sxs-lookup"><span data-stu-id="e0b8c-103">Update intuneBrandingProfileAssignment</span></span>

> <span data-ttu-id="e0b8c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0b8c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e0b8c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e0b8c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0b8c-106">Обновление свойств объекта [интунебрандингпрофилеассигнмент](../resources/intune-wip-intunebrandingprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="e0b8c-106">Update the properties of a [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e0b8c-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e0b8c-107">Prerequisites</span></span>
<span data-ttu-id="e0b8c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0b8c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0b8c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e0b8c-110">Permission type</span></span>|<span data-ttu-id="e0b8c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e0b8c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0b8c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e0b8c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e0b8c-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0b8c-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e0b8c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e0b8c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0b8c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0b8c-115">Not supported.</span></span>|
|<span data-ttu-id="e0b8c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e0b8c-116">Application</span></span>|<span data-ttu-id="e0b8c-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0b8c-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0b8c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e0b8c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments/{intuneBrandingProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="e0b8c-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e0b8c-119">Request headers</span></span>
|<span data-ttu-id="e0b8c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e0b8c-120">Header</span></span>|<span data-ttu-id="e0b8c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e0b8c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0b8c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e0b8c-122">Authorization</span></span>|<span data-ttu-id="e0b8c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e0b8c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0b8c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e0b8c-124">Accept</span></span>|<span data-ttu-id="e0b8c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e0b8c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0b8c-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e0b8c-126">Request body</span></span>
<span data-ttu-id="e0b8c-127">В тексте запроса добавьте представление объекта [интунебрандингпрофилеассигнмент](../resources/intune-wip-intunebrandingprofileassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e0b8c-127">In the request body, supply a JSON representation for the [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object.</span></span>

<span data-ttu-id="e0b8c-128">В следующей таблице приведены свойства, необходимые при создании [интунебрандингпрофилеассигнмент](../resources/intune-wip-intunebrandingprofileassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e0b8c-128">The following table shows the properties that are required when you create the [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md).</span></span>

|<span data-ttu-id="e0b8c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e0b8c-129">Property</span></span>|<span data-ttu-id="e0b8c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e0b8c-130">Type</span></span>|<span data-ttu-id="e0b8c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e0b8c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0b8c-132">id</span><span class="sxs-lookup"><span data-stu-id="e0b8c-132">id</span></span>|<span data-ttu-id="e0b8c-133">Строка</span><span class="sxs-lookup"><span data-stu-id="e0b8c-133">String</span></span>|<span data-ttu-id="e0b8c-134">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="e0b8c-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="e0b8c-135">target</span><span class="sxs-lookup"><span data-stu-id="e0b8c-135">target</span></span>|[<span data-ttu-id="e0b8c-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e0b8c-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="e0b8c-137">Цель назначения, которой назначен профиль фирменной символики.</span><span class="sxs-lookup"><span data-stu-id="e0b8c-137">Assignment target that the branding profile is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="e0b8c-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="e0b8c-138">Response</span></span>
<span data-ttu-id="e0b8c-139">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [интунебрандингпрофилеассигнмент](../resources/intune-wip-intunebrandingprofileassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e0b8c-139">If successful, this method returns a `200 OK` response code and an updated [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0b8c-140">Пример</span><span class="sxs-lookup"><span data-stu-id="e0b8c-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="e0b8c-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="e0b8c-141">Request</span></span>
<span data-ttu-id="e0b8c-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e0b8c-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments/{intuneBrandingProfileAssignmentId}
Content-type: application/json
Content-length: 171

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="e0b8c-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0b8c-143">Response</span></span>
<span data-ttu-id="e0b8c-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e0b8c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 220

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
  "id": "ee38a117-a117-ee38-17a1-38ee17a138ee",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





