---
title: Создание Интунебрандингпрофилеассигнмент
description: Создание нового объекта Интунебрандингпрофилеассигнмент.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d7f8336edf5bffd8708c5a5149066faed4ab3e21
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157913"
---
# <a name="create-intunebrandingprofileassignment"></a><span data-ttu-id="8cff4-103">Создание Интунебрандингпрофилеассигнмент</span><span class="sxs-lookup"><span data-stu-id="8cff4-103">Create intuneBrandingProfileAssignment</span></span>

> <span data-ttu-id="8cff4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8cff4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8cff4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8cff4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8cff4-106">Создание нового объекта [интунебрандингпрофилеассигнмент](../resources/intune-wip-intunebrandingprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="8cff4-106">Create a new [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8cff4-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8cff4-107">Prerequisites</span></span>
<span data-ttu-id="8cff4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="8cff4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8cff4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8cff4-110">Permission type</span></span>|<span data-ttu-id="8cff4-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8cff4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8cff4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8cff4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8cff4-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cff4-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8cff4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8cff4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8cff4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8cff4-115">Not supported.</span></span>|
|<span data-ttu-id="8cff4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8cff4-116">Application</span></span>|<span data-ttu-id="8cff4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8cff4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8cff4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8cff4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="8cff4-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8cff4-119">Request headers</span></span>
|<span data-ttu-id="8cff4-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8cff4-120">Header</span></span>|<span data-ttu-id="8cff4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8cff4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8cff4-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8cff4-122">Authorization</span></span>|<span data-ttu-id="8cff4-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8cff4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8cff4-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8cff4-124">Accept</span></span>|<span data-ttu-id="8cff4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8cff4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8cff4-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8cff4-126">Request body</span></span>
<span data-ttu-id="8cff4-127">В тексте запроса добавьте представление объекта Интунебрандингпрофилеассигнмент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8cff4-127">In the request body, supply a JSON representation for the intuneBrandingProfileAssignment object.</span></span>

<span data-ttu-id="8cff4-128">В следующей таблице приведены свойства, необходимые при создании Интунебрандингпрофилеассигнмент.</span><span class="sxs-lookup"><span data-stu-id="8cff4-128">The following table shows the properties that are required when you create the intuneBrandingProfileAssignment.</span></span>

|<span data-ttu-id="8cff4-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="8cff4-129">Property</span></span>|<span data-ttu-id="8cff4-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8cff4-130">Type</span></span>|<span data-ttu-id="8cff4-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8cff4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8cff4-132">id</span><span class="sxs-lookup"><span data-stu-id="8cff4-132">id</span></span>|<span data-ttu-id="8cff4-133">String</span><span class="sxs-lookup"><span data-stu-id="8cff4-133">String</span></span>|<span data-ttu-id="8cff4-134">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="8cff4-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="8cff4-135">target</span><span class="sxs-lookup"><span data-stu-id="8cff4-135">target</span></span>|[<span data-ttu-id="8cff4-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="8cff4-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="8cff4-137">Цель назначения, которой назначен профиль фирменной символики.</span><span class="sxs-lookup"><span data-stu-id="8cff4-137">Assignment target that the branding profile is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="8cff4-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="8cff4-138">Response</span></span>
<span data-ttu-id="8cff4-139">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [интунебрандингпрофилеассигнмент](../resources/intune-wip-intunebrandingprofileassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8cff4-139">If successful, this method returns a `201 Created` response code and a [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8cff4-140">Пример</span><span class="sxs-lookup"><span data-stu-id="8cff4-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="8cff4-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="8cff4-141">Request</span></span>
<span data-ttu-id="8cff4-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8cff4-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8cff4-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="8cff4-143">Response</span></span>
<span data-ttu-id="8cff4-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8cff4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




