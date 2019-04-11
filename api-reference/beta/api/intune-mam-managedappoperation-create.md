---
title: Создание объекта managedAppOperation
description: Создание объекта managedAppOperation.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 994af667aadc990760d64c2f4334fc6d21eefcb9
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31797272"
---
# <a name="create-managedappoperation"></a><span data-ttu-id="b2839-103">Создание объекта managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="b2839-103">Create managedAppOperation</span></span>

> <span data-ttu-id="b2839-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2839-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2839-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b2839-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2839-106">Создание объекта [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="b2839-106">Create a new [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2839-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b2839-107">Prerequisites</span></span>
<span data-ttu-id="b2839-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2839-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2839-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b2839-110">Permission type</span></span>|<span data-ttu-id="b2839-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b2839-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2839-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b2839-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b2839-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2839-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b2839-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b2839-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2839-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2839-115">Not supported.</span></span>|
|<span data-ttu-id="b2839-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b2839-116">Application</span></span>|<span data-ttu-id="b2839-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2839-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2839-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b2839-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
```

## <a name="request-headers"></a><span data-ttu-id="b2839-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b2839-119">Request headers</span></span>
|<span data-ttu-id="b2839-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b2839-120">Header</span></span>|<span data-ttu-id="b2839-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b2839-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2839-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b2839-122">Authorization</span></span>|<span data-ttu-id="b2839-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b2839-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2839-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b2839-124">Accept</span></span>|<span data-ttu-id="b2839-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b2839-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2839-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b2839-126">Request body</span></span>
<span data-ttu-id="b2839-127">В теле запроса добавьте представление объекта managedAppOperation в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b2839-127">In the request body, supply a JSON representation for the managedAppOperation object.</span></span>

<span data-ttu-id="b2839-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта managedAppOperation.</span><span class="sxs-lookup"><span data-stu-id="b2839-128">The following table shows the properties that are required when you create the managedAppOperation.</span></span>

|<span data-ttu-id="b2839-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b2839-129">Property</span></span>|<span data-ttu-id="b2839-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b2839-130">Type</span></span>|<span data-ttu-id="b2839-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b2839-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2839-132">displayName</span><span class="sxs-lookup"><span data-stu-id="b2839-132">displayName</span></span>|<span data-ttu-id="b2839-133">String</span><span class="sxs-lookup"><span data-stu-id="b2839-133">String</span></span>|<span data-ttu-id="b2839-134">Имя операции.</span><span class="sxs-lookup"><span data-stu-id="b2839-134">The operation name.</span></span>|
|<span data-ttu-id="b2839-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b2839-135">lastModifiedDateTime</span></span>|<span data-ttu-id="b2839-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2839-136">DateTimeOffset</span></span>|<span data-ttu-id="b2839-137">Время последнего изменения операции для приложения.</span><span class="sxs-lookup"><span data-stu-id="b2839-137">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="b2839-138">state</span><span class="sxs-lookup"><span data-stu-id="b2839-138">state</span></span>|<span data-ttu-id="b2839-139">String</span><span class="sxs-lookup"><span data-stu-id="b2839-139">String</span></span>|<span data-ttu-id="b2839-140">Текущее состояние операции</span><span class="sxs-lookup"><span data-stu-id="b2839-140">The current state of the operation</span></span>|
|<span data-ttu-id="b2839-141">id</span><span class="sxs-lookup"><span data-stu-id="b2839-141">id</span></span>|<span data-ttu-id="b2839-142">Строка</span><span class="sxs-lookup"><span data-stu-id="b2839-142">String</span></span>|<span data-ttu-id="b2839-143">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b2839-143">Key of the entity.</span></span>|
|<span data-ttu-id="b2839-144">version</span><span class="sxs-lookup"><span data-stu-id="b2839-144">version</span></span>|<span data-ttu-id="b2839-145">Строка</span><span class="sxs-lookup"><span data-stu-id="b2839-145">String</span></span>|<span data-ttu-id="b2839-146">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="b2839-146">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="b2839-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2839-147">Response</span></span>
<span data-ttu-id="b2839-148">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [managedAppOperation](../resources/intune-mam-managedappoperation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b2839-148">If successful, this method returns a `201 Created` response code and a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2839-149">Пример</span><span class="sxs-lookup"><span data-stu-id="b2839-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2839-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="b2839-150">Request</span></span>
<span data-ttu-id="b2839-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b2839-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b2839-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2839-152">Response</span></span>
<span data-ttu-id="b2839-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b2839-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





