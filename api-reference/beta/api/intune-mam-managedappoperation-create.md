---
title: Создание объекта managedAppOperation
description: Создание объекта managedAppOperation.
ms.openlocfilehash: ac6a6933a7cceac298e2cbd1c59d3cb1ec4aaade
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078378"
---
# <a name="create-managedappoperation"></a><span data-ttu-id="bea87-103">Создание объекта managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="bea87-103">Create managedAppOperation</span></span>

> <span data-ttu-id="bea87-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bea87-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bea87-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bea87-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bea87-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="bea87-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bea87-107">Создание объекта [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="bea87-107">Create a new [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bea87-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="bea87-108">Prerequisites</span></span>
<span data-ttu-id="bea87-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bea87-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bea87-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bea87-111">Permission type</span></span>|<span data-ttu-id="bea87-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bea87-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bea87-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bea87-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bea87-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bea87-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bea87-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bea87-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bea87-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bea87-116">Not supported.</span></span>|
|<span data-ttu-id="bea87-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bea87-117">Application</span></span>|<span data-ttu-id="bea87-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bea87-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bea87-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bea87-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
```

## <a name="request-headers"></a><span data-ttu-id="bea87-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bea87-120">Request headers</span></span>
|<span data-ttu-id="bea87-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bea87-121">Header</span></span>|<span data-ttu-id="bea87-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bea87-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bea87-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bea87-123">Authorization</span></span>|<span data-ttu-id="bea87-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="bea87-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bea87-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bea87-125">Accept</span></span>|<span data-ttu-id="bea87-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bea87-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bea87-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bea87-127">Request body</span></span>
<span data-ttu-id="bea87-128">В теле запроса добавьте представление объекта managedAppOperation в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bea87-128">In the request body, supply a JSON representation for the managedAppOperation object.</span></span>

<span data-ttu-id="bea87-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта managedAppOperation.</span><span class="sxs-lookup"><span data-stu-id="bea87-129">The following table shows the properties that are required when you create the managedAppOperation.</span></span>

|<span data-ttu-id="bea87-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="bea87-130">Property</span></span>|<span data-ttu-id="bea87-131">Тип</span><span class="sxs-lookup"><span data-stu-id="bea87-131">Type</span></span>|<span data-ttu-id="bea87-132">Описание</span><span class="sxs-lookup"><span data-stu-id="bea87-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bea87-133">displayName</span><span class="sxs-lookup"><span data-stu-id="bea87-133">displayName</span></span>|<span data-ttu-id="bea87-134">String</span><span class="sxs-lookup"><span data-stu-id="bea87-134">String</span></span>|<span data-ttu-id="bea87-135">Имя операции.</span><span class="sxs-lookup"><span data-stu-id="bea87-135">The operation name.</span></span>|
|<span data-ttu-id="bea87-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bea87-136">lastModifiedDateTime</span></span>|<span data-ttu-id="bea87-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bea87-137">DateTimeOffset</span></span>|<span data-ttu-id="bea87-138">Время последнего изменения операции для приложения.</span><span class="sxs-lookup"><span data-stu-id="bea87-138">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="bea87-139">state</span><span class="sxs-lookup"><span data-stu-id="bea87-139">state</span></span>|<span data-ttu-id="bea87-140">String</span><span class="sxs-lookup"><span data-stu-id="bea87-140">String</span></span>|<span data-ttu-id="bea87-141">Текущее состояние операции</span><span class="sxs-lookup"><span data-stu-id="bea87-141">The current state of the operation</span></span>|
|<span data-ttu-id="bea87-142">id</span><span class="sxs-lookup"><span data-stu-id="bea87-142">id</span></span>|<span data-ttu-id="bea87-143">String</span><span class="sxs-lookup"><span data-stu-id="bea87-143">String</span></span>|<span data-ttu-id="bea87-144">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bea87-144">Key of the entity.</span></span>|
|<span data-ttu-id="bea87-145">version</span><span class="sxs-lookup"><span data-stu-id="bea87-145">version</span></span>|<span data-ttu-id="bea87-146">String</span><span class="sxs-lookup"><span data-stu-id="bea87-146">String</span></span>|<span data-ttu-id="bea87-147">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="bea87-147">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="bea87-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="bea87-148">Response</span></span>
<span data-ttu-id="bea87-149">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [managedAppOperation](../resources/intune-mam-managedappoperation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="bea87-149">If successful, this method returns a `201 Created` response code and a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bea87-150">Пример</span><span class="sxs-lookup"><span data-stu-id="bea87-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="bea87-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="bea87-151">Request</span></span>
<span data-ttu-id="bea87-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bea87-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
Content-type: application/json
Content-length: 223

{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "state": "State value",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="bea87-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="bea87-153">Response</span></span>
<span data-ttu-id="bea87-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="bea87-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





