---
title: Обновление объекта managedAppOperation
description: Обновление свойств объекта managedAppOperation.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6eec0b5068b96330a81ea4d1d305cd7cc5f9e6fe
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30985202"
---
# <a name="update-managedappoperation"></a><span data-ttu-id="57866-103">Обновление объекта managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="57866-103">Update managedAppOperation</span></span>

> <span data-ttu-id="57866-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57866-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57866-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="57866-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57866-106">Обновление свойств объекта [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="57866-106">Update the properties of a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="57866-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="57866-107">Prerequisites</span></span>
<span data-ttu-id="57866-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57866-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57866-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="57866-110">Permission type</span></span>|<span data-ttu-id="57866-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="57866-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57866-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="57866-112">Delegated (work or school account)</span></span>|<span data-ttu-id="57866-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57866-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="57866-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="57866-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57866-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57866-115">Not supported.</span></span>|
|<span data-ttu-id="57866-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="57866-116">Application</span></span>|<span data-ttu-id="57866-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57866-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="57866-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="57866-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="57866-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="57866-119">Request headers</span></span>
|<span data-ttu-id="57866-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="57866-120">Header</span></span>|<span data-ttu-id="57866-121">Значение</span><span class="sxs-lookup"><span data-stu-id="57866-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57866-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="57866-122">Authorization</span></span>|<span data-ttu-id="57866-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="57866-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="57866-124">Accept</span><span class="sxs-lookup"><span data-stu-id="57866-124">Accept</span></span>|<span data-ttu-id="57866-125">application/json</span><span class="sxs-lookup"><span data-stu-id="57866-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57866-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="57866-126">Request body</span></span>
<span data-ttu-id="57866-127">В теле запроса добавьте представление объекта [managedAppOperation](../resources/intune-mam-managedappoperation.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="57866-127">In the request body, supply a JSON representation for the [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

<span data-ttu-id="57866-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="57866-128">The following table shows the properties that are required when you create the [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span></span>

|<span data-ttu-id="57866-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="57866-129">Property</span></span>|<span data-ttu-id="57866-130">Тип</span><span class="sxs-lookup"><span data-stu-id="57866-130">Type</span></span>|<span data-ttu-id="57866-131">Описание</span><span class="sxs-lookup"><span data-stu-id="57866-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57866-132">displayName</span><span class="sxs-lookup"><span data-stu-id="57866-132">displayName</span></span>|<span data-ttu-id="57866-133">String</span><span class="sxs-lookup"><span data-stu-id="57866-133">String</span></span>|<span data-ttu-id="57866-134">Имя операции.</span><span class="sxs-lookup"><span data-stu-id="57866-134">The operation name.</span></span>|
|<span data-ttu-id="57866-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="57866-135">lastModifiedDateTime</span></span>|<span data-ttu-id="57866-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57866-136">DateTimeOffset</span></span>|<span data-ttu-id="57866-137">Время последнего изменения операции для приложения.</span><span class="sxs-lookup"><span data-stu-id="57866-137">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="57866-138">state</span><span class="sxs-lookup"><span data-stu-id="57866-138">state</span></span>|<span data-ttu-id="57866-139">String</span><span class="sxs-lookup"><span data-stu-id="57866-139">String</span></span>|<span data-ttu-id="57866-140">Текущее состояние операции</span><span class="sxs-lookup"><span data-stu-id="57866-140">The current state of the operation</span></span>|
|<span data-ttu-id="57866-141">id</span><span class="sxs-lookup"><span data-stu-id="57866-141">id</span></span>|<span data-ttu-id="57866-142">Строка</span><span class="sxs-lookup"><span data-stu-id="57866-142">String</span></span>|<span data-ttu-id="57866-143">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="57866-143">Key of the entity.</span></span>|
|<span data-ttu-id="57866-144">version</span><span class="sxs-lookup"><span data-stu-id="57866-144">version</span></span>|<span data-ttu-id="57866-145">Строка</span><span class="sxs-lookup"><span data-stu-id="57866-145">String</span></span>|<span data-ttu-id="57866-146">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="57866-146">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="57866-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="57866-147">Response</span></span>
<span data-ttu-id="57866-148">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedAppOperation](../resources/intune-mam-managedappoperation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="57866-148">If successful, this method returns a `200 OK` response code and an updated [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57866-149">Пример</span><span class="sxs-lookup"><span data-stu-id="57866-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="57866-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="57866-150">Request</span></span>
<span data-ttu-id="57866-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="57866-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="57866-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="57866-152">Response</span></span>
<span data-ttu-id="57866-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="57866-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




