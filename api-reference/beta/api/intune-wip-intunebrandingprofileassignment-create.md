---
title: Создание Интунебрандингпрофилеассигнмент
description: Создание нового объекта Интунебрандингпрофилеассигнмент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e0223a709a2b5be7a4d92de5ff3b27a807a389be
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35979220"
---
# <a name="create-intunebrandingprofileassignment"></a><span data-ttu-id="ebe64-103">Создание Интунебрандингпрофилеассигнмент</span><span class="sxs-lookup"><span data-stu-id="ebe64-103">Create intuneBrandingProfileAssignment</span></span>

> <span data-ttu-id="ebe64-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ebe64-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ebe64-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ebe64-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebe64-106">Создание нового объекта [интунебрандингпрофилеассигнмент](../resources/intune-wip-intunebrandingprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="ebe64-106">Create a new [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ebe64-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ebe64-107">Prerequisites</span></span>
<span data-ttu-id="ebe64-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ebe64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebe64-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ebe64-110">Permission type</span></span>|<span data-ttu-id="ebe64-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ebe64-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ebe64-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ebe64-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ebe64-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebe64-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ebe64-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ebe64-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ebe64-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ebe64-115">Not supported.</span></span>|
|<span data-ttu-id="ebe64-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ebe64-116">Application</span></span>|<span data-ttu-id="ebe64-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ebe64-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ebe64-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ebe64-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="ebe64-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ebe64-119">Request headers</span></span>
|<span data-ttu-id="ebe64-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ebe64-120">Header</span></span>|<span data-ttu-id="ebe64-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ebe64-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ebe64-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ebe64-122">Authorization</span></span>|<span data-ttu-id="ebe64-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ebe64-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ebe64-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ebe64-124">Accept</span></span>|<span data-ttu-id="ebe64-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ebe64-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ebe64-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ebe64-126">Request body</span></span>
<span data-ttu-id="ebe64-127">В тексте запроса добавьте представление объекта Интунебрандингпрофилеассигнмент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ebe64-127">In the request body, supply a JSON representation for the intuneBrandingProfileAssignment object.</span></span>

<span data-ttu-id="ebe64-128">В следующей таблице приведены свойства, необходимые при создании Интунебрандингпрофилеассигнмент.</span><span class="sxs-lookup"><span data-stu-id="ebe64-128">The following table shows the properties that are required when you create the intuneBrandingProfileAssignment.</span></span>

|<span data-ttu-id="ebe64-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ebe64-129">Property</span></span>|<span data-ttu-id="ebe64-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ebe64-130">Type</span></span>|<span data-ttu-id="ebe64-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ebe64-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebe64-132">id</span><span class="sxs-lookup"><span data-stu-id="ebe64-132">id</span></span>|<span data-ttu-id="ebe64-133">String</span><span class="sxs-lookup"><span data-stu-id="ebe64-133">String</span></span>|<span data-ttu-id="ebe64-134">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="ebe64-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="ebe64-135">target</span><span class="sxs-lookup"><span data-stu-id="ebe64-135">target</span></span>|[<span data-ttu-id="ebe64-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ebe64-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="ebe64-137">Цель назначения, которой назначен профиль фирменной символики.</span><span class="sxs-lookup"><span data-stu-id="ebe64-137">Assignment target that the branding profile is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="ebe64-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="ebe64-138">Response</span></span>
<span data-ttu-id="ebe64-139">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [интунебрандингпрофилеассигнмент](../resources/intune-wip-intunebrandingprofileassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ebe64-139">If successful, this method returns a `201 Created` response code and a [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ebe64-140">Пример</span><span class="sxs-lookup"><span data-stu-id="ebe64-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="ebe64-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="ebe64-141">Request</span></span>
<span data-ttu-id="ebe64-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ebe64-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ebe64-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="ebe64-143">Response</span></span>
<span data-ttu-id="ebe64-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ebe64-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





