---
title: Обновление объекта termsAndConditionsAssignment
description: Удаление свойств объекта termsAndConditionsAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c4de7d4c55d0fc92e7439843f295a08f2ab04515
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37170436"
---
# <a name="update-termsandconditionsassignment"></a><span data-ttu-id="14388-103">Обновление объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="14388-103">Update termsAndConditionsAssignment</span></span>

> <span data-ttu-id="14388-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14388-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14388-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="14388-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14388-106">Удаление свойств объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="14388-106">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="14388-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="14388-107">Prerequisites</span></span>
<span data-ttu-id="14388-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14388-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14388-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="14388-110">Permission type</span></span>|<span data-ttu-id="14388-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="14388-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14388-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="14388-112">Delegated (work or school account)</span></span>|<span data-ttu-id="14388-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14388-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="14388-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="14388-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14388-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14388-115">Not supported.</span></span>|
|<span data-ttu-id="14388-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="14388-116">Application</span></span>|<span data-ttu-id="14388-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14388-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="14388-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="14388-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="14388-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="14388-119">Request headers</span></span>
|<span data-ttu-id="14388-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="14388-120">Header</span></span>|<span data-ttu-id="14388-121">Значение</span><span class="sxs-lookup"><span data-stu-id="14388-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14388-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="14388-122">Authorization</span></span>|<span data-ttu-id="14388-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="14388-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14388-124">Accept</span><span class="sxs-lookup"><span data-stu-id="14388-124">Accept</span></span>|<span data-ttu-id="14388-125">application/json</span><span class="sxs-lookup"><span data-stu-id="14388-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14388-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="14388-126">Request body</span></span>
<span data-ttu-id="14388-127">В тексте запроса добавьте представление объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="14388-127">In the request body, supply a JSON representation for the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

<span data-ttu-id="14388-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="14388-128">The following table shows the properties that are required when you create the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>

|<span data-ttu-id="14388-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="14388-129">Property</span></span>|<span data-ttu-id="14388-130">Тип</span><span class="sxs-lookup"><span data-stu-id="14388-130">Type</span></span>|<span data-ttu-id="14388-131">Описание</span><span class="sxs-lookup"><span data-stu-id="14388-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14388-132">id</span><span class="sxs-lookup"><span data-stu-id="14388-132">id</span></span>|<span data-ttu-id="14388-133">String</span><span class="sxs-lookup"><span data-stu-id="14388-133">String</span></span>|<span data-ttu-id="14388-134">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="14388-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="14388-135">target</span><span class="sxs-lookup"><span data-stu-id="14388-135">target</span></span>|[<span data-ttu-id="14388-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="14388-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="14388-137">Объект, для которого назначается политика соблюдения условий.</span><span class="sxs-lookup"><span data-stu-id="14388-137">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="14388-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="14388-138">Response</span></span>
<span data-ttu-id="14388-139">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="14388-139">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14388-140">Пример</span><span class="sxs-lookup"><span data-stu-id="14388-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="14388-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="14388-141">Request</span></span>
<span data-ttu-id="14388-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="14388-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
Content-type: application/json
Content-length: 168

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="14388-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="14388-143">Response</span></span>
<span data-ttu-id="14388-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="14388-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 217

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "id": "64c1a196-a196-64c1-96a1-c16496a1c164",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




