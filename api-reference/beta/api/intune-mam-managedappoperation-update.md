---
title: Обновление объекта managedAppOperation
description: Обновление свойств объекта managedAppOperation.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a45946b63c913bd06a696a706ffaab7a32e65fac
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47986380"
---
# <a name="update-managedappoperation"></a><span data-ttu-id="ef14f-103">Обновление объекта managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="ef14f-103">Update managedAppOperation</span></span>

<span data-ttu-id="ef14f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef14f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ef14f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef14f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ef14f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ef14f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef14f-107">Обновление свойств объекта [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="ef14f-107">Update the properties of a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ef14f-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ef14f-108">Prerequisites</span></span>
<span data-ttu-id="ef14f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef14f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef14f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ef14f-111">Permission type</span></span>|<span data-ttu-id="ef14f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ef14f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef14f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ef14f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ef14f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef14f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ef14f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ef14f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef14f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef14f-116">Not supported.</span></span>|
|<span data-ttu-id="ef14f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ef14f-117">Application</span></span>|<span data-ttu-id="ef14f-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef14f-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef14f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ef14f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="ef14f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ef14f-120">Request headers</span></span>
|<span data-ttu-id="ef14f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ef14f-121">Header</span></span>|<span data-ttu-id="ef14f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ef14f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef14f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef14f-123">Authorization</span></span>|<span data-ttu-id="ef14f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ef14f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef14f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ef14f-125">Accept</span></span>|<span data-ttu-id="ef14f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ef14f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef14f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ef14f-127">Request body</span></span>
<span data-ttu-id="ef14f-128">В теле запроса добавьте представление объекта [managedAppOperation](../resources/intune-mam-managedappoperation.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ef14f-128">In the request body, supply a JSON representation for the [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

<span data-ttu-id="ef14f-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="ef14f-129">The following table shows the properties that are required when you create the [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span></span>

|<span data-ttu-id="ef14f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ef14f-130">Property</span></span>|<span data-ttu-id="ef14f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ef14f-131">Type</span></span>|<span data-ttu-id="ef14f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ef14f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef14f-133">displayName</span><span class="sxs-lookup"><span data-stu-id="ef14f-133">displayName</span></span>|<span data-ttu-id="ef14f-134">String</span><span class="sxs-lookup"><span data-stu-id="ef14f-134">String</span></span>|<span data-ttu-id="ef14f-135">Имя операции.</span><span class="sxs-lookup"><span data-stu-id="ef14f-135">The operation name.</span></span>|
|<span data-ttu-id="ef14f-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ef14f-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ef14f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef14f-137">DateTimeOffset</span></span>|<span data-ttu-id="ef14f-138">Время последнего изменения операции для приложения.</span><span class="sxs-lookup"><span data-stu-id="ef14f-138">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="ef14f-139">state</span><span class="sxs-lookup"><span data-stu-id="ef14f-139">state</span></span>|<span data-ttu-id="ef14f-140">String</span><span class="sxs-lookup"><span data-stu-id="ef14f-140">String</span></span>|<span data-ttu-id="ef14f-141">Текущее состояние операции</span><span class="sxs-lookup"><span data-stu-id="ef14f-141">The current state of the operation</span></span>|
|<span data-ttu-id="ef14f-142">id</span><span class="sxs-lookup"><span data-stu-id="ef14f-142">id</span></span>|<span data-ttu-id="ef14f-143">String</span><span class="sxs-lookup"><span data-stu-id="ef14f-143">String</span></span>|<span data-ttu-id="ef14f-144">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ef14f-144">Key of the entity.</span></span>|
|<span data-ttu-id="ef14f-145">version</span><span class="sxs-lookup"><span data-stu-id="ef14f-145">version</span></span>|<span data-ttu-id="ef14f-146">String</span><span class="sxs-lookup"><span data-stu-id="ef14f-146">String</span></span>|<span data-ttu-id="ef14f-147">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="ef14f-147">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="ef14f-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef14f-148">Response</span></span>
<span data-ttu-id="ef14f-149">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedAppOperation](../resources/intune-mam-managedappoperation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ef14f-149">If successful, this method returns a `200 OK` response code and an updated [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef14f-150">Пример</span><span class="sxs-lookup"><span data-stu-id="ef14f-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="ef14f-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef14f-151">Request</span></span>
<span data-ttu-id="ef14f-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ef14f-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
Content-type: application/json
Content-length: 159

{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "Display Name value",
  "state": "State value",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="ef14f-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef14f-153">Response</span></span>
<span data-ttu-id="ef14f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ef14f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 272

{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "state": "State value",
  "id": "f2867b06-7b06-f286-067b-86f2067b86f2",
  "version": "Version value"
}
```






