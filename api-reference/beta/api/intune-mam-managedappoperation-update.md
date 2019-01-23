---
title: Обновление объекта managedAppOperation
description: Обновление свойств объекта managedAppOperation.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 376d54159b2b2eba7ca84d29fecf947cc4561bcb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401280"
---
# <a name="update-managedappoperation"></a><span data-ttu-id="e8090-103">Обновление объекта managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="e8090-103">Update managedAppOperation</span></span>

> <span data-ttu-id="e8090-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e8090-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e8090-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8090-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e8090-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e8090-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8090-107">Обновление свойств объекта [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="e8090-107">Update the properties of a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e8090-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e8090-108">Prerequisites</span></span>
<span data-ttu-id="e8090-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e8090-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e8090-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e8090-111">Permission type</span></span>|<span data-ttu-id="e8090-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e8090-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8090-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e8090-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e8090-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8090-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e8090-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e8090-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8090-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8090-116">Not supported.</span></span>|
|<span data-ttu-id="e8090-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e8090-117">Application</span></span>|<span data-ttu-id="e8090-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8090-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8090-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e8090-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="e8090-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e8090-120">Request headers</span></span>
|<span data-ttu-id="e8090-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e8090-121">Header</span></span>|<span data-ttu-id="e8090-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e8090-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8090-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8090-123">Authorization</span></span>|<span data-ttu-id="e8090-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e8090-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8090-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e8090-125">Accept</span></span>|<span data-ttu-id="e8090-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e8090-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8090-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e8090-127">Request body</span></span>
<span data-ttu-id="e8090-128">В теле запроса добавьте представление объекта [managedAppOperation](../resources/intune-mam-managedappoperation.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e8090-128">In the request body, supply a JSON representation for the [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

<span data-ttu-id="e8090-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="e8090-129">The following table shows the properties that are required when you create the [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span></span>

|<span data-ttu-id="e8090-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e8090-130">Property</span></span>|<span data-ttu-id="e8090-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e8090-131">Type</span></span>|<span data-ttu-id="e8090-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e8090-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8090-133">displayName</span><span class="sxs-lookup"><span data-stu-id="e8090-133">displayName</span></span>|<span data-ttu-id="e8090-134">String</span><span class="sxs-lookup"><span data-stu-id="e8090-134">String</span></span>|<span data-ttu-id="e8090-135">Имя операции.</span><span class="sxs-lookup"><span data-stu-id="e8090-135">The operation name.</span></span>|
|<span data-ttu-id="e8090-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e8090-136">lastModifiedDateTime</span></span>|<span data-ttu-id="e8090-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8090-137">DateTimeOffset</span></span>|<span data-ttu-id="e8090-138">Время последнего изменения операции для приложения.</span><span class="sxs-lookup"><span data-stu-id="e8090-138">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="e8090-139">state</span><span class="sxs-lookup"><span data-stu-id="e8090-139">state</span></span>|<span data-ttu-id="e8090-140">String</span><span class="sxs-lookup"><span data-stu-id="e8090-140">String</span></span>|<span data-ttu-id="e8090-141">Текущее состояние операции</span><span class="sxs-lookup"><span data-stu-id="e8090-141">The current state of the operation</span></span>|
|<span data-ttu-id="e8090-142">id</span><span class="sxs-lookup"><span data-stu-id="e8090-142">id</span></span>|<span data-ttu-id="e8090-143">String</span><span class="sxs-lookup"><span data-stu-id="e8090-143">String</span></span>|<span data-ttu-id="e8090-144">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e8090-144">Key of the entity.</span></span>|
|<span data-ttu-id="e8090-145">version</span><span class="sxs-lookup"><span data-stu-id="e8090-145">version</span></span>|<span data-ttu-id="e8090-146">String</span><span class="sxs-lookup"><span data-stu-id="e8090-146">String</span></span>|<span data-ttu-id="e8090-147">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="e8090-147">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="e8090-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8090-148">Response</span></span>
<span data-ttu-id="e8090-149">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedAppOperation](../resources/intune-mam-managedappoperation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e8090-149">If successful, this method returns a `200 OK` response code and an updated [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8090-150">Пример</span><span class="sxs-lookup"><span data-stu-id="e8090-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8090-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8090-151">Request</span></span>
<span data-ttu-id="e8090-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e8090-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e8090-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8090-153">Response</span></span>
<span data-ttu-id="e8090-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e8090-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




