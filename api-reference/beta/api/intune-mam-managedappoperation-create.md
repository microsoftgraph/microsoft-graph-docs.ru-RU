---
title: Создание объекта managedAppOperation
description: Создание объекта managedAppOperation.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4f3ec846571e5c98cd3d99ddd279028475b2a6eb
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43455956"
---
# <a name="create-managedappoperation"></a><span data-ttu-id="211aa-103">Создание объекта managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="211aa-103">Create managedAppOperation</span></span>

<span data-ttu-id="211aa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="211aa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="211aa-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="211aa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="211aa-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="211aa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="211aa-107">Создание объекта [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="211aa-107">Create a new [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="211aa-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="211aa-108">Prerequisites</span></span>
<span data-ttu-id="211aa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="211aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="211aa-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="211aa-111">Permission type</span></span>|<span data-ttu-id="211aa-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="211aa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="211aa-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="211aa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="211aa-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="211aa-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="211aa-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="211aa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="211aa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="211aa-116">Not supported.</span></span>|
|<span data-ttu-id="211aa-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="211aa-117">Application</span></span>|<span data-ttu-id="211aa-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="211aa-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="211aa-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="211aa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
```

## <a name="request-headers"></a><span data-ttu-id="211aa-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="211aa-120">Request headers</span></span>
|<span data-ttu-id="211aa-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="211aa-121">Header</span></span>|<span data-ttu-id="211aa-122">Значение</span><span class="sxs-lookup"><span data-stu-id="211aa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="211aa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="211aa-123">Authorization</span></span>|<span data-ttu-id="211aa-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="211aa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="211aa-125">Accept</span><span class="sxs-lookup"><span data-stu-id="211aa-125">Accept</span></span>|<span data-ttu-id="211aa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="211aa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="211aa-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="211aa-127">Request body</span></span>
<span data-ttu-id="211aa-128">В теле запроса добавьте представление объекта managedAppOperation в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="211aa-128">In the request body, supply a JSON representation for the managedAppOperation object.</span></span>

<span data-ttu-id="211aa-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта managedAppOperation.</span><span class="sxs-lookup"><span data-stu-id="211aa-129">The following table shows the properties that are required when you create the managedAppOperation.</span></span>

|<span data-ttu-id="211aa-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="211aa-130">Property</span></span>|<span data-ttu-id="211aa-131">Тип</span><span class="sxs-lookup"><span data-stu-id="211aa-131">Type</span></span>|<span data-ttu-id="211aa-132">Описание</span><span class="sxs-lookup"><span data-stu-id="211aa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="211aa-133">displayName</span><span class="sxs-lookup"><span data-stu-id="211aa-133">displayName</span></span>|<span data-ttu-id="211aa-134">Строка</span><span class="sxs-lookup"><span data-stu-id="211aa-134">String</span></span>|<span data-ttu-id="211aa-135">Имя операции.</span><span class="sxs-lookup"><span data-stu-id="211aa-135">The operation name.</span></span>|
|<span data-ttu-id="211aa-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="211aa-136">lastModifiedDateTime</span></span>|<span data-ttu-id="211aa-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="211aa-137">DateTimeOffset</span></span>|<span data-ttu-id="211aa-138">Время последнего изменения операции для приложения.</span><span class="sxs-lookup"><span data-stu-id="211aa-138">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="211aa-139">state</span><span class="sxs-lookup"><span data-stu-id="211aa-139">state</span></span>|<span data-ttu-id="211aa-140">String</span><span class="sxs-lookup"><span data-stu-id="211aa-140">String</span></span>|<span data-ttu-id="211aa-141">Текущее состояние операции</span><span class="sxs-lookup"><span data-stu-id="211aa-141">The current state of the operation</span></span>|
|<span data-ttu-id="211aa-142">id</span><span class="sxs-lookup"><span data-stu-id="211aa-142">id</span></span>|<span data-ttu-id="211aa-143">String</span><span class="sxs-lookup"><span data-stu-id="211aa-143">String</span></span>|<span data-ttu-id="211aa-144">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="211aa-144">Key of the entity.</span></span>|
|<span data-ttu-id="211aa-145">version</span><span class="sxs-lookup"><span data-stu-id="211aa-145">version</span></span>|<span data-ttu-id="211aa-146">String</span><span class="sxs-lookup"><span data-stu-id="211aa-146">String</span></span>|<span data-ttu-id="211aa-147">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="211aa-147">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="211aa-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="211aa-148">Response</span></span>
<span data-ttu-id="211aa-149">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [managedAppOperation](../resources/intune-mam-managedappoperation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="211aa-149">If successful, this method returns a `201 Created` response code and a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="211aa-150">Пример</span><span class="sxs-lookup"><span data-stu-id="211aa-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="211aa-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="211aa-151">Request</span></span>
<span data-ttu-id="211aa-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="211aa-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
Content-type: application/json
Content-length: 159

{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "Display Name value",
  "state": "State value",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="211aa-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="211aa-153">Response</span></span>
<span data-ttu-id="211aa-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="211aa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



