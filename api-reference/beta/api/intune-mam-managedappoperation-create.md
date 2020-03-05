---
title: Создание объекта managedAppOperation
description: Создание объекта managedAppOperation.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e2ba1f5a28cadee8e55b352d99ef0b02fd9a531f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42463575"
---
# <a name="create-managedappoperation"></a><span data-ttu-id="83f50-103">Создание объекта managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="83f50-103">Create managedAppOperation</span></span>

<span data-ttu-id="83f50-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="83f50-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="83f50-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83f50-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83f50-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="83f50-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83f50-107">Создание объекта [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="83f50-107">Create a new [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="83f50-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="83f50-108">Prerequisites</span></span>
<span data-ttu-id="83f50-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83f50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83f50-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="83f50-111">Permission type</span></span>|<span data-ttu-id="83f50-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="83f50-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83f50-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="83f50-113">Delegated (work or school account)</span></span>|<span data-ttu-id="83f50-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83f50-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="83f50-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="83f50-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83f50-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83f50-116">Not supported.</span></span>|
|<span data-ttu-id="83f50-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="83f50-117">Application</span></span>|<span data-ttu-id="83f50-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83f50-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="83f50-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="83f50-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
```

## <a name="request-headers"></a><span data-ttu-id="83f50-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="83f50-120">Request headers</span></span>
|<span data-ttu-id="83f50-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="83f50-121">Header</span></span>|<span data-ttu-id="83f50-122">Значение</span><span class="sxs-lookup"><span data-stu-id="83f50-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83f50-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="83f50-123">Authorization</span></span>|<span data-ttu-id="83f50-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="83f50-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83f50-125">Accept</span><span class="sxs-lookup"><span data-stu-id="83f50-125">Accept</span></span>|<span data-ttu-id="83f50-126">application/json</span><span class="sxs-lookup"><span data-stu-id="83f50-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83f50-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="83f50-127">Request body</span></span>
<span data-ttu-id="83f50-128">В теле запроса добавьте представление объекта managedAppOperation в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="83f50-128">In the request body, supply a JSON representation for the managedAppOperation object.</span></span>

<span data-ttu-id="83f50-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта managedAppOperation.</span><span class="sxs-lookup"><span data-stu-id="83f50-129">The following table shows the properties that are required when you create the managedAppOperation.</span></span>

|<span data-ttu-id="83f50-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="83f50-130">Property</span></span>|<span data-ttu-id="83f50-131">Тип</span><span class="sxs-lookup"><span data-stu-id="83f50-131">Type</span></span>|<span data-ttu-id="83f50-132">Описание</span><span class="sxs-lookup"><span data-stu-id="83f50-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83f50-133">displayName</span><span class="sxs-lookup"><span data-stu-id="83f50-133">displayName</span></span>|<span data-ttu-id="83f50-134">Строка</span><span class="sxs-lookup"><span data-stu-id="83f50-134">String</span></span>|<span data-ttu-id="83f50-135">Имя операции.</span><span class="sxs-lookup"><span data-stu-id="83f50-135">The operation name.</span></span>|
|<span data-ttu-id="83f50-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="83f50-136">lastModifiedDateTime</span></span>|<span data-ttu-id="83f50-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83f50-137">DateTimeOffset</span></span>|<span data-ttu-id="83f50-138">Время последнего изменения операции для приложения.</span><span class="sxs-lookup"><span data-stu-id="83f50-138">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="83f50-139">state</span><span class="sxs-lookup"><span data-stu-id="83f50-139">state</span></span>|<span data-ttu-id="83f50-140">String</span><span class="sxs-lookup"><span data-stu-id="83f50-140">String</span></span>|<span data-ttu-id="83f50-141">Текущее состояние операции</span><span class="sxs-lookup"><span data-stu-id="83f50-141">The current state of the operation</span></span>|
|<span data-ttu-id="83f50-142">id</span><span class="sxs-lookup"><span data-stu-id="83f50-142">id</span></span>|<span data-ttu-id="83f50-143">String</span><span class="sxs-lookup"><span data-stu-id="83f50-143">String</span></span>|<span data-ttu-id="83f50-144">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="83f50-144">Key of the entity.</span></span>|
|<span data-ttu-id="83f50-145">version</span><span class="sxs-lookup"><span data-stu-id="83f50-145">version</span></span>|<span data-ttu-id="83f50-146">String</span><span class="sxs-lookup"><span data-stu-id="83f50-146">String</span></span>|<span data-ttu-id="83f50-147">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="83f50-147">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="83f50-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="83f50-148">Response</span></span>
<span data-ttu-id="83f50-149">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [managedAppOperation](../resources/intune-mam-managedappoperation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="83f50-149">If successful, this method returns a `201 Created` response code and a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83f50-150">Пример</span><span class="sxs-lookup"><span data-stu-id="83f50-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="83f50-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="83f50-151">Request</span></span>
<span data-ttu-id="83f50-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="83f50-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="83f50-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="83f50-153">Response</span></span>
<span data-ttu-id="83f50-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="83f50-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





