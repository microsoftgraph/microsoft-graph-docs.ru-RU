---
title: Создание объекта managedAppOperation
description: Создание объекта managedAppOperation.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 84a954832fb709e0431535653b9e6d175624364c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42803612"
---
# <a name="create-managedappoperation"></a><span data-ttu-id="0d269-103">Создание объекта managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="0d269-103">Create managedAppOperation</span></span>

> <span data-ttu-id="0d269-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d269-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0d269-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0d269-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d269-106">Создание объекта [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="0d269-106">Create a new [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0d269-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0d269-107">Prerequisites</span></span>
<span data-ttu-id="0d269-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d269-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d269-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0d269-110">Permission type</span></span>|<span data-ttu-id="0d269-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0d269-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d269-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0d269-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0d269-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d269-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0d269-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0d269-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d269-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d269-115">Not supported.</span></span>|
|<span data-ttu-id="0d269-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="0d269-116">Application</span></span>|<span data-ttu-id="0d269-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d269-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d269-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0d269-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
```

## <a name="request-headers"></a><span data-ttu-id="0d269-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0d269-119">Request headers</span></span>
|<span data-ttu-id="0d269-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0d269-120">Header</span></span>|<span data-ttu-id="0d269-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0d269-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d269-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d269-122">Authorization</span></span>|<span data-ttu-id="0d269-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0d269-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d269-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0d269-124">Accept</span></span>|<span data-ttu-id="0d269-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0d269-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d269-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0d269-126">Request body</span></span>
<span data-ttu-id="0d269-127">В теле запроса добавьте представление объекта managedAppOperation в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0d269-127">In the request body, supply a JSON representation for the managedAppOperation object.</span></span>

<span data-ttu-id="0d269-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта managedAppOperation.</span><span class="sxs-lookup"><span data-stu-id="0d269-128">The following table shows the properties that are required when you create the managedAppOperation.</span></span>

|<span data-ttu-id="0d269-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="0d269-129">Property</span></span>|<span data-ttu-id="0d269-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0d269-130">Type</span></span>|<span data-ttu-id="0d269-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0d269-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d269-132">displayName</span><span class="sxs-lookup"><span data-stu-id="0d269-132">displayName</span></span>|<span data-ttu-id="0d269-133">Строка</span><span class="sxs-lookup"><span data-stu-id="0d269-133">String</span></span>|<span data-ttu-id="0d269-134">Имя операции.</span><span class="sxs-lookup"><span data-stu-id="0d269-134">The operation name.</span></span>|
|<span data-ttu-id="0d269-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0d269-135">lastModifiedDateTime</span></span>|<span data-ttu-id="0d269-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d269-136">DateTimeOffset</span></span>|<span data-ttu-id="0d269-137">Время последнего изменения операции для приложения.</span><span class="sxs-lookup"><span data-stu-id="0d269-137">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="0d269-138">state</span><span class="sxs-lookup"><span data-stu-id="0d269-138">state</span></span>|<span data-ttu-id="0d269-139">String</span><span class="sxs-lookup"><span data-stu-id="0d269-139">String</span></span>|<span data-ttu-id="0d269-140">Текущее состояние операции</span><span class="sxs-lookup"><span data-stu-id="0d269-140">The current state of the operation</span></span>|
|<span data-ttu-id="0d269-141">id</span><span class="sxs-lookup"><span data-stu-id="0d269-141">id</span></span>|<span data-ttu-id="0d269-142">String</span><span class="sxs-lookup"><span data-stu-id="0d269-142">String</span></span>|<span data-ttu-id="0d269-143">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0d269-143">Key of the entity.</span></span>|
|<span data-ttu-id="0d269-144">version</span><span class="sxs-lookup"><span data-stu-id="0d269-144">version</span></span>|<span data-ttu-id="0d269-145">String</span><span class="sxs-lookup"><span data-stu-id="0d269-145">String</span></span>|<span data-ttu-id="0d269-146">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="0d269-146">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="0d269-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d269-147">Response</span></span>
<span data-ttu-id="0d269-148">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [managedAppOperation](../resources/intune-mam-managedappoperation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0d269-148">If successful, this method returns a `201 Created` response code and a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d269-149">Пример</span><span class="sxs-lookup"><span data-stu-id="0d269-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="0d269-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d269-150">Request</span></span>
<span data-ttu-id="0d269-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0d269-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0d269-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d269-152">Response</span></span>
<span data-ttu-id="0d269-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0d269-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




