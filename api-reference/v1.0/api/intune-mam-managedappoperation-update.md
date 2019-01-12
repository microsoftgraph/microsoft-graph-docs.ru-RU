---
title: Обновление объекта managedAppOperation
description: Обновление свойств объекта managedAppOperation.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5d0baf0b503edcde0bdc03329ec354a4d6e42a4c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980134"
---
# <a name="update-managedappoperation"></a><span data-ttu-id="836ed-103">Обновление объекта managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="836ed-103">Update managedAppOperation</span></span>

> <span data-ttu-id="836ed-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="836ed-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="836ed-105">Обновление свойств объекта [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="836ed-105">Update the properties of a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="836ed-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="836ed-106">Prerequisites</span></span>
<span data-ttu-id="836ed-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="836ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="836ed-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="836ed-109">Permission type</span></span>|<span data-ttu-id="836ed-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="836ed-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="836ed-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="836ed-111">Delegated (work or school account)</span></span>|<span data-ttu-id="836ed-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="836ed-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="836ed-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="836ed-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="836ed-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="836ed-114">Not supported.</span></span>|
|<span data-ttu-id="836ed-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="836ed-115">Application</span></span>|<span data-ttu-id="836ed-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="836ed-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="836ed-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="836ed-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="836ed-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="836ed-118">Request headers</span></span>
|<span data-ttu-id="836ed-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="836ed-119">Header</span></span>|<span data-ttu-id="836ed-120">Значение</span><span class="sxs-lookup"><span data-stu-id="836ed-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="836ed-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="836ed-121">Authorization</span></span>|<span data-ttu-id="836ed-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="836ed-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="836ed-123">Accept</span><span class="sxs-lookup"><span data-stu-id="836ed-123">Accept</span></span>|<span data-ttu-id="836ed-124">application/json</span><span class="sxs-lookup"><span data-stu-id="836ed-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="836ed-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="836ed-125">Request body</span></span>
<span data-ttu-id="836ed-126">В теле запроса добавьте представление объекта [managedAppOperation](../resources/intune-mam-managedappoperation.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="836ed-126">In the request body, supply a JSON representation for the [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

<span data-ttu-id="836ed-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="836ed-127">The following table shows the properties that are required when you create the [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span></span>

|<span data-ttu-id="836ed-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="836ed-128">Property</span></span>|<span data-ttu-id="836ed-129">Тип</span><span class="sxs-lookup"><span data-stu-id="836ed-129">Type</span></span>|<span data-ttu-id="836ed-130">Описание</span><span class="sxs-lookup"><span data-stu-id="836ed-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="836ed-131">displayName</span><span class="sxs-lookup"><span data-stu-id="836ed-131">displayName</span></span>|<span data-ttu-id="836ed-132">String</span><span class="sxs-lookup"><span data-stu-id="836ed-132">String</span></span>|<span data-ttu-id="836ed-133">Имя операции.</span><span class="sxs-lookup"><span data-stu-id="836ed-133">The operation name.</span></span>|
|<span data-ttu-id="836ed-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="836ed-134">lastModifiedDateTime</span></span>|<span data-ttu-id="836ed-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="836ed-135">DateTimeOffset</span></span>|<span data-ttu-id="836ed-136">Время последнего изменения операции для приложения.</span><span class="sxs-lookup"><span data-stu-id="836ed-136">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="836ed-137">state</span><span class="sxs-lookup"><span data-stu-id="836ed-137">state</span></span>|<span data-ttu-id="836ed-138">String</span><span class="sxs-lookup"><span data-stu-id="836ed-138">String</span></span>|<span data-ttu-id="836ed-139">Текущее состояние операции</span><span class="sxs-lookup"><span data-stu-id="836ed-139">The current state of the operation</span></span>|
|<span data-ttu-id="836ed-140">id</span><span class="sxs-lookup"><span data-stu-id="836ed-140">id</span></span>|<span data-ttu-id="836ed-141">Строка</span><span class="sxs-lookup"><span data-stu-id="836ed-141">String</span></span>|<span data-ttu-id="836ed-142">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="836ed-142">Key of the entity.</span></span>|
|<span data-ttu-id="836ed-143">version</span><span class="sxs-lookup"><span data-stu-id="836ed-143">version</span></span>|<span data-ttu-id="836ed-144">Строка</span><span class="sxs-lookup"><span data-stu-id="836ed-144">String</span></span>|<span data-ttu-id="836ed-145">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="836ed-145">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="836ed-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="836ed-146">Response</span></span>
<span data-ttu-id="836ed-147">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedAppOperation](../resources/intune-mam-managedappoperation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="836ed-147">If successful, this method returns a `200 OK` response code and an updated [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="836ed-148">Пример</span><span class="sxs-lookup"><span data-stu-id="836ed-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="836ed-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="836ed-149">Request</span></span>
<span data-ttu-id="836ed-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="836ed-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
Content-type: application/json
Content-length: 159

{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "Display Name value",
  "state": "State value",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="836ed-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="836ed-151">Response</span></span>
<span data-ttu-id="836ed-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="836ed-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



