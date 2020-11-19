---
title: Создание объекта managedAppOperation
description: Создание объекта managedAppOperation.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5238b4e5e1c796893e930929b2edc788ad7a134a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49277724"
---
# <a name="create-managedappoperation"></a><span data-ttu-id="edfaf-103">Создание объекта managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="edfaf-103">Create managedAppOperation</span></span>

<span data-ttu-id="edfaf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="edfaf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="edfaf-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="edfaf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="edfaf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="edfaf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="edfaf-107">Создание объекта [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="edfaf-107">Create a new [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="edfaf-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="edfaf-108">Prerequisites</span></span>
<span data-ttu-id="edfaf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="edfaf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="edfaf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="edfaf-111">Permission type</span></span>|<span data-ttu-id="edfaf-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="edfaf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="edfaf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="edfaf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="edfaf-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="edfaf-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="edfaf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="edfaf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="edfaf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="edfaf-116">Not supported.</span></span>|
|<span data-ttu-id="edfaf-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="edfaf-117">Application</span></span>|<span data-ttu-id="edfaf-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="edfaf-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="edfaf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="edfaf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
```

## <a name="request-headers"></a><span data-ttu-id="edfaf-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="edfaf-120">Request headers</span></span>
|<span data-ttu-id="edfaf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="edfaf-121">Header</span></span>|<span data-ttu-id="edfaf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="edfaf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="edfaf-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="edfaf-123">Authorization</span></span>|<span data-ttu-id="edfaf-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="edfaf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="edfaf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="edfaf-125">Accept</span></span>|<span data-ttu-id="edfaf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="edfaf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="edfaf-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="edfaf-127">Request body</span></span>
<span data-ttu-id="edfaf-128">В теле запроса добавьте представление объекта managedAppOperation в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="edfaf-128">In the request body, supply a JSON representation for the managedAppOperation object.</span></span>

<span data-ttu-id="edfaf-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта managedAppOperation.</span><span class="sxs-lookup"><span data-stu-id="edfaf-129">The following table shows the properties that are required when you create the managedAppOperation.</span></span>

|<span data-ttu-id="edfaf-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="edfaf-130">Property</span></span>|<span data-ttu-id="edfaf-131">Тип</span><span class="sxs-lookup"><span data-stu-id="edfaf-131">Type</span></span>|<span data-ttu-id="edfaf-132">Описание</span><span class="sxs-lookup"><span data-stu-id="edfaf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="edfaf-133">displayName</span><span class="sxs-lookup"><span data-stu-id="edfaf-133">displayName</span></span>|<span data-ttu-id="edfaf-134">String</span><span class="sxs-lookup"><span data-stu-id="edfaf-134">String</span></span>|<span data-ttu-id="edfaf-135">Имя операции.</span><span class="sxs-lookup"><span data-stu-id="edfaf-135">The operation name.</span></span>|
|<span data-ttu-id="edfaf-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="edfaf-136">lastModifiedDateTime</span></span>|<span data-ttu-id="edfaf-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="edfaf-137">DateTimeOffset</span></span>|<span data-ttu-id="edfaf-138">Время последнего изменения операции для приложения.</span><span class="sxs-lookup"><span data-stu-id="edfaf-138">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="edfaf-139">state</span><span class="sxs-lookup"><span data-stu-id="edfaf-139">state</span></span>|<span data-ttu-id="edfaf-140">String</span><span class="sxs-lookup"><span data-stu-id="edfaf-140">String</span></span>|<span data-ttu-id="edfaf-141">Текущее состояние операции</span><span class="sxs-lookup"><span data-stu-id="edfaf-141">The current state of the operation</span></span>|
|<span data-ttu-id="edfaf-142">id</span><span class="sxs-lookup"><span data-stu-id="edfaf-142">id</span></span>|<span data-ttu-id="edfaf-143">String</span><span class="sxs-lookup"><span data-stu-id="edfaf-143">String</span></span>|<span data-ttu-id="edfaf-144">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="edfaf-144">Key of the entity.</span></span>|
|<span data-ttu-id="edfaf-145">version</span><span class="sxs-lookup"><span data-stu-id="edfaf-145">version</span></span>|<span data-ttu-id="edfaf-146">String</span><span class="sxs-lookup"><span data-stu-id="edfaf-146">String</span></span>|<span data-ttu-id="edfaf-147">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="edfaf-147">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="edfaf-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="edfaf-148">Response</span></span>
<span data-ttu-id="edfaf-149">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [managedAppOperation](../resources/intune-mam-managedappoperation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="edfaf-149">If successful, this method returns a `201 Created` response code and a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="edfaf-150">Пример</span><span class="sxs-lookup"><span data-stu-id="edfaf-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="edfaf-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="edfaf-151">Request</span></span>
<span data-ttu-id="edfaf-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="edfaf-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="edfaf-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="edfaf-153">Response</span></span>
<span data-ttu-id="edfaf-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="edfaf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




