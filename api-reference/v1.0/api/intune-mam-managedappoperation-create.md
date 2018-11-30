---
title: Создание объекта managedAppOperation
description: Создание объекта managedAppOperation.
ms.openlocfilehash: 083ecd75da542a80ce06213725db9594941504eb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027955"
---
# <a name="create-managedappoperation"></a><span data-ttu-id="ac342-103">Создание объекта managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="ac342-103">Create managedAppOperation</span></span>

> <span data-ttu-id="ac342-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ac342-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ac342-105">Создание объекта [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="ac342-105">Create a new [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ac342-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ac342-106">Prerequisites</span></span>
<span data-ttu-id="ac342-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac342-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac342-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ac342-109">Permission type</span></span>|<span data-ttu-id="ac342-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ac342-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ac342-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ac342-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ac342-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac342-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ac342-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ac342-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ac342-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac342-114">Not supported.</span></span>|
|<span data-ttu-id="ac342-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ac342-115">Application</span></span>|<span data-ttu-id="ac342-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac342-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ac342-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ac342-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
```

## <a name="request-headers"></a><span data-ttu-id="ac342-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ac342-118">Request headers</span></span>
|<span data-ttu-id="ac342-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ac342-119">Header</span></span>|<span data-ttu-id="ac342-120">Значение</span><span class="sxs-lookup"><span data-stu-id="ac342-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ac342-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac342-121">Authorization</span></span>|<span data-ttu-id="ac342-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ac342-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ac342-123">Accept</span><span class="sxs-lookup"><span data-stu-id="ac342-123">Accept</span></span>|<span data-ttu-id="ac342-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ac342-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ac342-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ac342-125">Request body</span></span>
<span data-ttu-id="ac342-126">В теле запроса добавьте представление объекта managedAppOperation в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ac342-126">In the request body, supply a JSON representation for the managedAppOperation object.</span></span>

<span data-ttu-id="ac342-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта managedAppOperation.</span><span class="sxs-lookup"><span data-stu-id="ac342-127">The following table shows the properties that are required when you create the managedAppOperation.</span></span>

|<span data-ttu-id="ac342-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="ac342-128">Property</span></span>|<span data-ttu-id="ac342-129">Тип</span><span class="sxs-lookup"><span data-stu-id="ac342-129">Type</span></span>|<span data-ttu-id="ac342-130">Описание</span><span class="sxs-lookup"><span data-stu-id="ac342-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac342-131">displayName</span><span class="sxs-lookup"><span data-stu-id="ac342-131">displayName</span></span>|<span data-ttu-id="ac342-132">String</span><span class="sxs-lookup"><span data-stu-id="ac342-132">String</span></span>|<span data-ttu-id="ac342-133">Имя операции.</span><span class="sxs-lookup"><span data-stu-id="ac342-133">The operation name.</span></span>|
|<span data-ttu-id="ac342-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ac342-134">lastModifiedDateTime</span></span>|<span data-ttu-id="ac342-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac342-135">DateTimeOffset</span></span>|<span data-ttu-id="ac342-136">Время последнего изменения операции для приложения.</span><span class="sxs-lookup"><span data-stu-id="ac342-136">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="ac342-137">state</span><span class="sxs-lookup"><span data-stu-id="ac342-137">state</span></span>|<span data-ttu-id="ac342-138">String</span><span class="sxs-lookup"><span data-stu-id="ac342-138">String</span></span>|<span data-ttu-id="ac342-139">Текущее состояние операции</span><span class="sxs-lookup"><span data-stu-id="ac342-139">The current state of the operation</span></span>|
|<span data-ttu-id="ac342-140">id</span><span class="sxs-lookup"><span data-stu-id="ac342-140">id</span></span>|<span data-ttu-id="ac342-141">String</span><span class="sxs-lookup"><span data-stu-id="ac342-141">String</span></span>|<span data-ttu-id="ac342-142">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ac342-142">Key of the entity.</span></span>|
|<span data-ttu-id="ac342-143">version</span><span class="sxs-lookup"><span data-stu-id="ac342-143">version</span></span>|<span data-ttu-id="ac342-144">String</span><span class="sxs-lookup"><span data-stu-id="ac342-144">String</span></span>|<span data-ttu-id="ac342-145">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="ac342-145">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="ac342-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac342-146">Response</span></span>
<span data-ttu-id="ac342-147">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [managedAppOperation](../resources/intune-mam-managedappoperation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ac342-147">If successful, this method returns a `201 Created` response code and a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac342-148">Пример</span><span class="sxs-lookup"><span data-stu-id="ac342-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="ac342-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="ac342-149">Request</span></span>
<span data-ttu-id="ac342-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ac342-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
Content-type: application/json
Content-length: 159

{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "Display Name value",
  "state": "State value",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="ac342-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="ac342-151">Response</span></span>
<span data-ttu-id="ac342-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="ac342-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



