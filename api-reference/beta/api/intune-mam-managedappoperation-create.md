---
title: Создание объекта managedAppOperation
description: Создание объекта managedAppOperation.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 468be75739afbe33c5371352130d3e409e92e052
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142926"
---
# <a name="create-managedappoperation"></a><span data-ttu-id="9f165-103">Создание объекта managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="9f165-103">Create managedAppOperation</span></span>

> <span data-ttu-id="9f165-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f165-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f165-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9f165-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f165-106">Создание объекта [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="9f165-106">Create a new [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f165-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9f165-107">Prerequisites</span></span>
<span data-ttu-id="9f165-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9f165-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9f165-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f165-110">Permission type</span></span>|<span data-ttu-id="9f165-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f165-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f165-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f165-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9f165-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f165-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9f165-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f165-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f165-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f165-115">Not supported.</span></span>|
|<span data-ttu-id="9f165-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9f165-116">Application</span></span>|<span data-ttu-id="9f165-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f165-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f165-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f165-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
```

## <a name="request-headers"></a><span data-ttu-id="9f165-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9f165-119">Request headers</span></span>
|<span data-ttu-id="9f165-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9f165-120">Header</span></span>|<span data-ttu-id="9f165-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9f165-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f165-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9f165-122">Authorization</span></span>|<span data-ttu-id="9f165-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="9f165-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f165-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9f165-124">Accept</span></span>|<span data-ttu-id="9f165-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9f165-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f165-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9f165-126">Request body</span></span>
<span data-ttu-id="9f165-127">В теле запроса добавьте представление объекта managedAppOperation в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9f165-127">In the request body, supply a JSON representation for the managedAppOperation object.</span></span>

<span data-ttu-id="9f165-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта managedAppOperation.</span><span class="sxs-lookup"><span data-stu-id="9f165-128">The following table shows the properties that are required when you create the managedAppOperation.</span></span>

|<span data-ttu-id="9f165-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="9f165-129">Property</span></span>|<span data-ttu-id="9f165-130">Тип</span><span class="sxs-lookup"><span data-stu-id="9f165-130">Type</span></span>|<span data-ttu-id="9f165-131">Описание</span><span class="sxs-lookup"><span data-stu-id="9f165-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f165-132">displayName</span><span class="sxs-lookup"><span data-stu-id="9f165-132">displayName</span></span>|<span data-ttu-id="9f165-133">String</span><span class="sxs-lookup"><span data-stu-id="9f165-133">String</span></span>|<span data-ttu-id="9f165-134">Имя операции.</span><span class="sxs-lookup"><span data-stu-id="9f165-134">The operation name.</span></span>|
|<span data-ttu-id="9f165-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9f165-135">lastModifiedDateTime</span></span>|<span data-ttu-id="9f165-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f165-136">DateTimeOffset</span></span>|<span data-ttu-id="9f165-137">Время последнего изменения операции для приложения.</span><span class="sxs-lookup"><span data-stu-id="9f165-137">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="9f165-138">state</span><span class="sxs-lookup"><span data-stu-id="9f165-138">state</span></span>|<span data-ttu-id="9f165-139">String</span><span class="sxs-lookup"><span data-stu-id="9f165-139">String</span></span>|<span data-ttu-id="9f165-140">Текущее состояние операции</span><span class="sxs-lookup"><span data-stu-id="9f165-140">The current state of the operation</span></span>|
|<span data-ttu-id="9f165-141">id</span><span class="sxs-lookup"><span data-stu-id="9f165-141">id</span></span>|<span data-ttu-id="9f165-142">String</span><span class="sxs-lookup"><span data-stu-id="9f165-142">String</span></span>|<span data-ttu-id="9f165-143">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9f165-143">Key of the entity.</span></span>|
|<span data-ttu-id="9f165-144">version</span><span class="sxs-lookup"><span data-stu-id="9f165-144">version</span></span>|<span data-ttu-id="9f165-145">String</span><span class="sxs-lookup"><span data-stu-id="9f165-145">String</span></span>|<span data-ttu-id="9f165-146">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="9f165-146">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="9f165-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f165-147">Response</span></span>
<span data-ttu-id="9f165-148">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [managedAppOperation](../resources/intune-mam-managedappoperation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9f165-148">If successful, this method returns a `201 Created` response code and a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f165-149">Пример</span><span class="sxs-lookup"><span data-stu-id="9f165-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f165-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f165-150">Request</span></span>
<span data-ttu-id="9f165-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f165-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9f165-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="9f165-152">Response</span></span>
<span data-ttu-id="9f165-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9f165-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




