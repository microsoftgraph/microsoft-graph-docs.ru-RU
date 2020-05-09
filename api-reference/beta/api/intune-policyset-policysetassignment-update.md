---
title: Обновление Полицисетассигнмент
description: Обновление свойств объекта Полицисетассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d5d7a90f10cdc74490534f19469714033c39b3fe
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178299"
---
# <a name="update-policysetassignment"></a><span data-ttu-id="71d25-103">Обновление Полицисетассигнмент</span><span class="sxs-lookup"><span data-stu-id="71d25-103">Update policySetAssignment</span></span>

<span data-ttu-id="71d25-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71d25-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="71d25-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71d25-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71d25-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="71d25-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71d25-107">Обновление свойств объекта [полицисетассигнмент](../resources/intune-policyset-policysetassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="71d25-107">Update the properties of a [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="71d25-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="71d25-108">Prerequisites</span></span>
<span data-ttu-id="71d25-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71d25-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71d25-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71d25-111">Permission type</span></span>|<span data-ttu-id="71d25-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="71d25-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71d25-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71d25-113">Delegated (work or school account)</span></span>|<span data-ttu-id="71d25-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71d25-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="71d25-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71d25-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71d25-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71d25-116">Not supported.</span></span>|
|<span data-ttu-id="71d25-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="71d25-117">Application</span></span>|<span data-ttu-id="71d25-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71d25-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="71d25-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71d25-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/policySets/{policySetId}/assignments/{policySetAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="71d25-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="71d25-120">Request headers</span></span>
|<span data-ttu-id="71d25-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="71d25-121">Header</span></span>|<span data-ttu-id="71d25-122">Значение</span><span class="sxs-lookup"><span data-stu-id="71d25-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71d25-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="71d25-123">Authorization</span></span>|<span data-ttu-id="71d25-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="71d25-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71d25-125">Accept</span><span class="sxs-lookup"><span data-stu-id="71d25-125">Accept</span></span>|<span data-ttu-id="71d25-126">application/json</span><span class="sxs-lookup"><span data-stu-id="71d25-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71d25-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="71d25-127">Request body</span></span>
<span data-ttu-id="71d25-128">В тексте запроса добавьте представление объекта [полицисетассигнмент](../resources/intune-policyset-policysetassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="71d25-128">In the request body, supply a JSON representation for the [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object.</span></span>

<span data-ttu-id="71d25-129">В следующей таблице приведены свойства, необходимые при создании [полицисетассигнмент](../resources/intune-policyset-policysetassignment.md).</span><span class="sxs-lookup"><span data-stu-id="71d25-129">The following table shows the properties that are required when you create the [policySetAssignment](../resources/intune-policyset-policysetassignment.md).</span></span>

|<span data-ttu-id="71d25-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="71d25-130">Property</span></span>|<span data-ttu-id="71d25-131">Тип</span><span class="sxs-lookup"><span data-stu-id="71d25-131">Type</span></span>|<span data-ttu-id="71d25-132">Описание</span><span class="sxs-lookup"><span data-stu-id="71d25-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71d25-133">id</span><span class="sxs-lookup"><span data-stu-id="71d25-133">id</span></span>|<span data-ttu-id="71d25-134">Строка</span><span class="sxs-lookup"><span data-stu-id="71d25-134">String</span></span>|<span data-ttu-id="71d25-135">Ключ Полицисетассигнмент.</span><span class="sxs-lookup"><span data-stu-id="71d25-135">Key of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="71d25-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="71d25-136">lastModifiedDateTime</span></span>|<span data-ttu-id="71d25-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71d25-137">DateTimeOffset</span></span>|<span data-ttu-id="71d25-138">Время последнего изменения Полицисетассигнмент.</span><span class="sxs-lookup"><span data-stu-id="71d25-138">Last modified time of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="71d25-139">target</span><span class="sxs-lookup"><span data-stu-id="71d25-139">target</span></span>|[<span data-ttu-id="71d25-140">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="71d25-140">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="71d25-141">Целевая группа Полицисетассигнмент</span><span class="sxs-lookup"><span data-stu-id="71d25-141">The target group of PolicySetAssignment</span></span>|



## <a name="response"></a><span data-ttu-id="71d25-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="71d25-142">Response</span></span>
<span data-ttu-id="71d25-143">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [полицисетассигнмент](../resources/intune-policyset-policysetassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="71d25-143">If successful, this method returns a `200 OK` response code and an updated [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71d25-144">Пример</span><span class="sxs-lookup"><span data-stu-id="71d25-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="71d25-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="71d25-145">Request</span></span>
<span data-ttu-id="71d25-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="71d25-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/assignments/{policySetAssignmentId}
Content-type: application/json
Content-length: 147

{
  "@odata.type": "#microsoft.graph.policySetAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="71d25-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="71d25-147">Response</span></span>
<span data-ttu-id="71d25-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="71d25-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 260

{
  "@odata.type": "#microsoft.graph.policySetAssignment",
  "id": "0a8e7d40-7d40-0a8e-407d-8e0a407d8e0a",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
  }
}
```



