---
title: Обновление Интунебрандингпрофилеассигнмент
description: Обновление свойств объекта Интунебрандингпрофилеассигнмент.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8aecac4625d1fb92ea3f664b1e7a813fd096dce6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30139587"
---
# <a name="update-intunebrandingprofileassignment"></a><span data-ttu-id="3f2d0-103">Обновление Интунебрандингпрофилеассигнмент</span><span class="sxs-lookup"><span data-stu-id="3f2d0-103">Update intuneBrandingProfileAssignment</span></span>

> <span data-ttu-id="3f2d0-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f2d0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f2d0-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3f2d0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f2d0-106">Обновление свойств объекта [интунебрандингпрофилеассигнмент](../resources/intune-wip-intunebrandingprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="3f2d0-106">Update the properties of a [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3f2d0-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3f2d0-107">Prerequisites</span></span>
<span data-ttu-id="3f2d0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3f2d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3f2d0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3f2d0-110">Permission type</span></span>|<span data-ttu-id="3f2d0-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3f2d0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3f2d0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3f2d0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3f2d0-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f2d0-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3f2d0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3f2d0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3f2d0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f2d0-115">Not supported.</span></span>|
|<span data-ttu-id="3f2d0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3f2d0-116">Application</span></span>|<span data-ttu-id="3f2d0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f2d0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3f2d0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3f2d0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments/{intuneBrandingProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="3f2d0-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3f2d0-119">Request headers</span></span>
|<span data-ttu-id="3f2d0-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3f2d0-120">Header</span></span>|<span data-ttu-id="3f2d0-121">Значение</span><span class="sxs-lookup"><span data-stu-id="3f2d0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3f2d0-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3f2d0-122">Authorization</span></span>|<span data-ttu-id="3f2d0-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3f2d0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3f2d0-124">Accept</span><span class="sxs-lookup"><span data-stu-id="3f2d0-124">Accept</span></span>|<span data-ttu-id="3f2d0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3f2d0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f2d0-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3f2d0-126">Request body</span></span>
<span data-ttu-id="3f2d0-127">В тексте запроса добавьте представление объекта [Интунебрандингпрофилеассигнмент](../resources/intune-wip-intunebrandingprofileassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3f2d0-127">In the request body, supply a JSON representation for the [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object.</span></span>

<span data-ttu-id="3f2d0-128">В следующей таблице приведены свойства, необходимые при создании [интунебрандингпрофилеассигнмент](../resources/intune-wip-intunebrandingprofileassignment.md).</span><span class="sxs-lookup"><span data-stu-id="3f2d0-128">The following table shows the properties that are required when you create the [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md).</span></span>

|<span data-ttu-id="3f2d0-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="3f2d0-129">Property</span></span>|<span data-ttu-id="3f2d0-130">Тип</span><span class="sxs-lookup"><span data-stu-id="3f2d0-130">Type</span></span>|<span data-ttu-id="3f2d0-131">Описание</span><span class="sxs-lookup"><span data-stu-id="3f2d0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f2d0-132">id</span><span class="sxs-lookup"><span data-stu-id="3f2d0-132">id</span></span>|<span data-ttu-id="3f2d0-133">String</span><span class="sxs-lookup"><span data-stu-id="3f2d0-133">String</span></span>|<span data-ttu-id="3f2d0-134">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="3f2d0-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="3f2d0-135">target</span><span class="sxs-lookup"><span data-stu-id="3f2d0-135">target</span></span>|[<span data-ttu-id="3f2d0-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="3f2d0-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="3f2d0-137">Цель назначения, которой назначен профиль фирменной символики.</span><span class="sxs-lookup"><span data-stu-id="3f2d0-137">Assignment target that the branding profile is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="3f2d0-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f2d0-138">Response</span></span>
<span data-ttu-id="3f2d0-139">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [интунебрандингпрофилеассигнмент](../resources/intune-wip-intunebrandingprofileassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3f2d0-139">If successful, this method returns a `200 OK` response code and an updated [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f2d0-140">Пример</span><span class="sxs-lookup"><span data-stu-id="3f2d0-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="3f2d0-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="3f2d0-141">Request</span></span>
<span data-ttu-id="3f2d0-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3f2d0-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3f2d0-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f2d0-143">Response</span></span>
<span data-ttu-id="3f2d0-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3f2d0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




