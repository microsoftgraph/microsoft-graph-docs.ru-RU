---
title: Обновление объекта mobileAppAssignment
description: Обновление свойств объекта mobileAppAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 245e18d690c17378ffb0218ae817a5973f922e88
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32489928"
---
# <a name="update-mobileappassignment"></a><span data-ttu-id="a18cb-103">Обновление объекта mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="a18cb-103">Update mobileAppAssignment</span></span>

> <span data-ttu-id="a18cb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a18cb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a18cb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a18cb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a18cb-106">Обновление свойств объекта [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a18cb-106">Update the properties of a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a18cb-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a18cb-107">Prerequisites</span></span>
<span data-ttu-id="a18cb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a18cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a18cb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a18cb-110">Permission type</span></span>|<span data-ttu-id="a18cb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a18cb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a18cb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a18cb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a18cb-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a18cb-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a18cb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a18cb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a18cb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a18cb-115">Not supported.</span></span>|
|<span data-ttu-id="a18cb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a18cb-116">Application</span></span>|<span data-ttu-id="a18cb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a18cb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a18cb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a18cb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="a18cb-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a18cb-119">Request headers</span></span>
|<span data-ttu-id="a18cb-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a18cb-120">Header</span></span>|<span data-ttu-id="a18cb-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a18cb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a18cb-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a18cb-122">Authorization</span></span>|<span data-ttu-id="a18cb-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a18cb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a18cb-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a18cb-124">Accept</span></span>|<span data-ttu-id="a18cb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a18cb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a18cb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a18cb-126">Request body</span></span>
<span data-ttu-id="a18cb-127">В тексте запроса добавьте представление объекта [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a18cb-127">In the request body, supply a JSON representation for the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

<span data-ttu-id="a18cb-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a18cb-128">The following table shows the properties that are required when you create the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span></span>

|<span data-ttu-id="a18cb-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a18cb-129">Property</span></span>|<span data-ttu-id="a18cb-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a18cb-130">Type</span></span>|<span data-ttu-id="a18cb-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a18cb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a18cb-132">id</span><span class="sxs-lookup"><span data-stu-id="a18cb-132">id</span></span>|<span data-ttu-id="a18cb-133">String</span><span class="sxs-lookup"><span data-stu-id="a18cb-133">String</span></span>|<span data-ttu-id="a18cb-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a18cb-134">Key of the entity.</span></span>|
|<span data-ttu-id="a18cb-135">intent</span><span class="sxs-lookup"><span data-stu-id="a18cb-135">intent</span></span>|[<span data-ttu-id="a18cb-136">installIntent</span><span class="sxs-lookup"><span data-stu-id="a18cb-136">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="a18cb-137">Цель установки, определенная администратором. Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="a18cb-137">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="a18cb-138">target</span><span class="sxs-lookup"><span data-stu-id="a18cb-138">target</span></span>|[<span data-ttu-id="a18cb-139">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a18cb-139">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="a18cb-140">Целевое назначение группы, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="a18cb-140">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="a18cb-141">settings</span><span class="sxs-lookup"><span data-stu-id="a18cb-141">settings</span></span>|[<span data-ttu-id="a18cb-142">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="a18cb-142">mobileAppAssignmentSettings</span></span>](../resources/intune-apps-mobileappassignmentsettings.md)|<span data-ttu-id="a18cb-143">Параметры целевого назначения, определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="a18cb-143">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="a18cb-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="a18cb-144">Response</span></span>
<span data-ttu-id="a18cb-145">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a18cb-145">If successful, this method returns a `200 OK` response code and an updated [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a18cb-146">Пример</span><span class="sxs-lookup"><span data-stu-id="a18cb-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="a18cb-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="a18cb-147">Request</span></span>
<span data-ttu-id="a18cb-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a18cb-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
Content-type: application/json
Content-length: 273

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```

### <a name="response"></a><span data-ttu-id="a18cb-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="a18cb-149">Response</span></span>
<span data-ttu-id="a18cb-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a18cb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 322

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "id": "591620b7-20b7-5916-b720-1659b7201659",
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```





