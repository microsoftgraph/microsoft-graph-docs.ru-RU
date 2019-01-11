---
title: Создание объекта managedAppOperation
description: Создание объекта managedAppOperation.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: eac205f4e8bd443ed90784e85e623869b440b204
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877247"
---
# <a name="create-managedappoperation"></a><span data-ttu-id="3e94e-103">Создание объекта managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="3e94e-103">Create managedAppOperation</span></span>

> <span data-ttu-id="3e94e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3e94e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3e94e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e94e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3e94e-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3e94e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3e94e-107">Создание объекта [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="3e94e-107">Create a new [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3e94e-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3e94e-108">Prerequisites</span></span>
<span data-ttu-id="3e94e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e94e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e94e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3e94e-111">Permission type</span></span>|<span data-ttu-id="3e94e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3e94e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e94e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3e94e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3e94e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e94e-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3e94e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3e94e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e94e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e94e-116">Not supported.</span></span>|
|<span data-ttu-id="3e94e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3e94e-117">Application</span></span>|<span data-ttu-id="3e94e-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e94e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e94e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3e94e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
```

## <a name="request-headers"></a><span data-ttu-id="3e94e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3e94e-120">Request headers</span></span>
|<span data-ttu-id="3e94e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3e94e-121">Header</span></span>|<span data-ttu-id="3e94e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3e94e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3e94e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e94e-123">Authorization</span></span>|<span data-ttu-id="3e94e-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3e94e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3e94e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3e94e-125">Accept</span></span>|<span data-ttu-id="3e94e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3e94e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e94e-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3e94e-127">Request body</span></span>
<span data-ttu-id="3e94e-128">В теле запроса добавьте представление объекта managedAppOperation в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3e94e-128">In the request body, supply a JSON representation for the managedAppOperation object.</span></span>

<span data-ttu-id="3e94e-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта managedAppOperation.</span><span class="sxs-lookup"><span data-stu-id="3e94e-129">The following table shows the properties that are required when you create the managedAppOperation.</span></span>

|<span data-ttu-id="3e94e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3e94e-130">Property</span></span>|<span data-ttu-id="3e94e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3e94e-131">Type</span></span>|<span data-ttu-id="3e94e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3e94e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e94e-133">displayName</span><span class="sxs-lookup"><span data-stu-id="3e94e-133">displayName</span></span>|<span data-ttu-id="3e94e-134">String</span><span class="sxs-lookup"><span data-stu-id="3e94e-134">String</span></span>|<span data-ttu-id="3e94e-135">Имя операции.</span><span class="sxs-lookup"><span data-stu-id="3e94e-135">The operation name.</span></span>|
|<span data-ttu-id="3e94e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3e94e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="3e94e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e94e-137">DateTimeOffset</span></span>|<span data-ttu-id="3e94e-138">Время последнего изменения операции для приложения.</span><span class="sxs-lookup"><span data-stu-id="3e94e-138">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="3e94e-139">state</span><span class="sxs-lookup"><span data-stu-id="3e94e-139">state</span></span>|<span data-ttu-id="3e94e-140">String</span><span class="sxs-lookup"><span data-stu-id="3e94e-140">String</span></span>|<span data-ttu-id="3e94e-141">Текущее состояние операции</span><span class="sxs-lookup"><span data-stu-id="3e94e-141">The current state of the operation</span></span>|
|<span data-ttu-id="3e94e-142">id</span><span class="sxs-lookup"><span data-stu-id="3e94e-142">id</span></span>|<span data-ttu-id="3e94e-143">Строка</span><span class="sxs-lookup"><span data-stu-id="3e94e-143">String</span></span>|<span data-ttu-id="3e94e-144">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3e94e-144">Key of the entity.</span></span>|
|<span data-ttu-id="3e94e-145">version</span><span class="sxs-lookup"><span data-stu-id="3e94e-145">version</span></span>|<span data-ttu-id="3e94e-146">Строка</span><span class="sxs-lookup"><span data-stu-id="3e94e-146">String</span></span>|<span data-ttu-id="3e94e-147">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="3e94e-147">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="3e94e-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e94e-148">Response</span></span>
<span data-ttu-id="3e94e-149">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [managedAppOperation](../resources/intune-mam-managedappoperation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3e94e-149">If successful, this method returns a `201 Created` response code and a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e94e-150">Пример</span><span class="sxs-lookup"><span data-stu-id="3e94e-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="3e94e-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e94e-151">Request</span></span>
<span data-ttu-id="3e94e-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3e94e-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3e94e-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="3e94e-153">Response</span></span>
<span data-ttu-id="3e94e-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3e94e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





