---
title: Создание Полицисетассигнмент
description: Создание нового объекта Полицисетассигнмент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e9827b9222ba4b02457cc40486f8fad3357baca6
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37192645"
---
# <a name="create-policysetassignment"></a><span data-ttu-id="69f06-103">Создание Полицисетассигнмент</span><span class="sxs-lookup"><span data-stu-id="69f06-103">Create policySetAssignment</span></span>

> <span data-ttu-id="69f06-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69f06-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69f06-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="69f06-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69f06-106">Создание нового объекта [полицисетассигнмент](../resources/intune-policyset-policysetassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="69f06-106">Create a new [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="69f06-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="69f06-107">Prerequisites</span></span>
<span data-ttu-id="69f06-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69f06-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69f06-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="69f06-110">Permission type</span></span>|<span data-ttu-id="69f06-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="69f06-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69f06-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="69f06-112">Delegated (work or school account)</span></span>|<span data-ttu-id="69f06-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69f06-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="69f06-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="69f06-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69f06-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69f06-115">Not supported.</span></span>|
|<span data-ttu-id="69f06-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="69f06-116">Application</span></span>|<span data-ttu-id="69f06-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69f06-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="69f06-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="69f06-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="69f06-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="69f06-119">Request headers</span></span>
|<span data-ttu-id="69f06-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="69f06-120">Header</span></span>|<span data-ttu-id="69f06-121">Значение</span><span class="sxs-lookup"><span data-stu-id="69f06-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69f06-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="69f06-122">Authorization</span></span>|<span data-ttu-id="69f06-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="69f06-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69f06-124">Accept</span><span class="sxs-lookup"><span data-stu-id="69f06-124">Accept</span></span>|<span data-ttu-id="69f06-125">application/json</span><span class="sxs-lookup"><span data-stu-id="69f06-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69f06-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="69f06-126">Request body</span></span>
<span data-ttu-id="69f06-127">В тексте запроса добавьте представление объекта Полицисетассигнмент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="69f06-127">In the request body, supply a JSON representation for the policySetAssignment object.</span></span>

<span data-ttu-id="69f06-128">В следующей таблице приведены свойства, необходимые при создании Полицисетассигнмент.</span><span class="sxs-lookup"><span data-stu-id="69f06-128">The following table shows the properties that are required when you create the policySetAssignment.</span></span>

|<span data-ttu-id="69f06-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="69f06-129">Property</span></span>|<span data-ttu-id="69f06-130">Тип</span><span class="sxs-lookup"><span data-stu-id="69f06-130">Type</span></span>|<span data-ttu-id="69f06-131">Описание</span><span class="sxs-lookup"><span data-stu-id="69f06-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69f06-132">id</span><span class="sxs-lookup"><span data-stu-id="69f06-132">id</span></span>|<span data-ttu-id="69f06-133">String</span><span class="sxs-lookup"><span data-stu-id="69f06-133">String</span></span>|<span data-ttu-id="69f06-134">Ключ Полицисетассигнмент.</span><span class="sxs-lookup"><span data-stu-id="69f06-134">Key of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="69f06-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="69f06-135">lastModifiedDateTime</span></span>|<span data-ttu-id="69f06-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69f06-136">DateTimeOffset</span></span>|<span data-ttu-id="69f06-137">Время последнего изменения Полицисетассигнмент.</span><span class="sxs-lookup"><span data-stu-id="69f06-137">Last modified time of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="69f06-138">target</span><span class="sxs-lookup"><span data-stu-id="69f06-138">target</span></span>|[<span data-ttu-id="69f06-139">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="69f06-139">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="69f06-140">Целевая группа Полицисетассигнмент</span><span class="sxs-lookup"><span data-stu-id="69f06-140">The target group of PolicySetAssignment</span></span>|



## <a name="response"></a><span data-ttu-id="69f06-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="69f06-141">Response</span></span>
<span data-ttu-id="69f06-142">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [полицисетассигнмент](../resources/intune-policyset-policysetassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="69f06-142">If successful, this method returns a `201 Created` response code and a [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69f06-143">Пример</span><span class="sxs-lookup"><span data-stu-id="69f06-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="69f06-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="69f06-144">Request</span></span>
<span data-ttu-id="69f06-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="69f06-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/assignments
Content-type: application/json
Content-length: 159

{
  "@odata.type": "#microsoft.graph.policySetAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="69f06-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="69f06-146">Response</span></span>
<span data-ttu-id="69f06-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="69f06-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 272

{
  "@odata.type": "#microsoft.graph.policySetAssignment",
  "id": "0a8e7d40-7d40-0a8e-407d-8e0a407d8e0a",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




