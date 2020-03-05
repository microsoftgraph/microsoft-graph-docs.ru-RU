---
title: Создание Интунебрандингпрофилеассигнмент
description: Создание нового объекта Интунебрандингпрофилеассигнмент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 10fb939fef6e8c88398ad627adcd0b33e0b49a2b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42457421"
---
# <a name="create-intunebrandingprofileassignment"></a><span data-ttu-id="49093-103">Создание Интунебрандингпрофилеассигнмент</span><span class="sxs-lookup"><span data-stu-id="49093-103">Create intuneBrandingProfileAssignment</span></span>

<span data-ttu-id="49093-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="49093-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="49093-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49093-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49093-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="49093-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49093-107">Создание нового объекта [интунебрандингпрофилеассигнмент](../resources/intune-wip-intunebrandingprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="49093-107">Create a new [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="49093-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="49093-108">Prerequisites</span></span>
<span data-ttu-id="49093-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49093-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49093-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49093-111">Permission type</span></span>|<span data-ttu-id="49093-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="49093-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49093-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49093-113">Delegated (work or school account)</span></span>|<span data-ttu-id="49093-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49093-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="49093-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49093-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49093-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49093-116">Not supported.</span></span>|
|<span data-ttu-id="49093-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="49093-117">Application</span></span>|<span data-ttu-id="49093-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49093-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="49093-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49093-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="49093-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="49093-120">Request headers</span></span>
|<span data-ttu-id="49093-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="49093-121">Header</span></span>|<span data-ttu-id="49093-122">Значение</span><span class="sxs-lookup"><span data-stu-id="49093-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49093-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="49093-123">Authorization</span></span>|<span data-ttu-id="49093-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="49093-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49093-125">Accept</span><span class="sxs-lookup"><span data-stu-id="49093-125">Accept</span></span>|<span data-ttu-id="49093-126">application/json</span><span class="sxs-lookup"><span data-stu-id="49093-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49093-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="49093-127">Request body</span></span>
<span data-ttu-id="49093-128">В тексте запроса добавьте представление объекта Интунебрандингпрофилеассигнмент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="49093-128">In the request body, supply a JSON representation for the intuneBrandingProfileAssignment object.</span></span>

<span data-ttu-id="49093-129">В следующей таблице приведены свойства, необходимые при создании Интунебрандингпрофилеассигнмент.</span><span class="sxs-lookup"><span data-stu-id="49093-129">The following table shows the properties that are required when you create the intuneBrandingProfileAssignment.</span></span>

|<span data-ttu-id="49093-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="49093-130">Property</span></span>|<span data-ttu-id="49093-131">Тип</span><span class="sxs-lookup"><span data-stu-id="49093-131">Type</span></span>|<span data-ttu-id="49093-132">Описание</span><span class="sxs-lookup"><span data-stu-id="49093-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49093-133">id</span><span class="sxs-lookup"><span data-stu-id="49093-133">id</span></span>|<span data-ttu-id="49093-134">String</span><span class="sxs-lookup"><span data-stu-id="49093-134">String</span></span>|<span data-ttu-id="49093-135">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="49093-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="49093-136">target</span><span class="sxs-lookup"><span data-stu-id="49093-136">target</span></span>|[<span data-ttu-id="49093-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="49093-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="49093-138">Цель назначения, которой назначен профиль фирменной символики.</span><span class="sxs-lookup"><span data-stu-id="49093-138">Assignment target that the branding profile is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="49093-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="49093-139">Response</span></span>
<span data-ttu-id="49093-140">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [интунебрандингпрофилеассигнмент](../resources/intune-wip-intunebrandingprofileassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="49093-140">If successful, this method returns a `201 Created` response code and a [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49093-141">Пример</span><span class="sxs-lookup"><span data-stu-id="49093-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="49093-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="49093-142">Request</span></span>
<span data-ttu-id="49093-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="49093-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments
Content-type: application/json
Content-length: 171

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="49093-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="49093-144">Response</span></span>
<span data-ttu-id="49093-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="49093-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





