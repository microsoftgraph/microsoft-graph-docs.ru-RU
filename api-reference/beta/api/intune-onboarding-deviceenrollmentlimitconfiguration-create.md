---
title: Создание объекта deviceEnrollmentLimitConfiguration
description: Создание объекта deviceEnrollmentLimitConfiguration.
ms.openlocfilehash: 6a8cb46b022f68082bd3d291c87e612bde06ab4d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079564"
---
# <a name="create-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="a658d-103">Создание объекта deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="a658d-103">Create deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="a658d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a658d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a658d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a658d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a658d-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a658d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a658d-107">Создание объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a658d-107">Create a new [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a658d-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a658d-108">Prerequisites</span></span>
<span data-ttu-id="a658d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a658d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a658d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a658d-111">Permission type</span></span>|<span data-ttu-id="a658d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a658d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a658d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a658d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a658d-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a658d-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a658d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a658d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a658d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a658d-116">Not supported.</span></span>|
|<span data-ttu-id="a658d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a658d-117">Application</span></span>|<span data-ttu-id="a658d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a658d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a658d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a658d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a658d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a658d-120">Request headers</span></span>
|<span data-ttu-id="a658d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a658d-121">Header</span></span>|<span data-ttu-id="a658d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a658d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a658d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a658d-123">Authorization</span></span>|<span data-ttu-id="a658d-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a658d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a658d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a658d-125">Accept</span></span>|<span data-ttu-id="a658d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a658d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a658d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a658d-127">Request body</span></span>
<span data-ttu-id="a658d-128">В тексте запроса добавьте представление объекта deviceEnrollmentLimitConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a658d-128">In the request body, supply a JSON representation for the deviceEnrollmentLimitConfiguration object.</span></span>

<span data-ttu-id="a658d-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceEnrollmentLimitConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a658d-129">The following table shows the properties that are required when you create the deviceEnrollmentLimitConfiguration.</span></span>

|<span data-ttu-id="a658d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a658d-130">Property</span></span>|<span data-ttu-id="a658d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a658d-131">Type</span></span>|<span data-ttu-id="a658d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a658d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a658d-133">id</span><span class="sxs-lookup"><span data-stu-id="a658d-133">id</span></span>|<span data-ttu-id="a658d-134">String</span><span class="sxs-lookup"><span data-stu-id="a658d-134">String</span></span>|<span data-ttu-id="a658d-135">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a658d-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a658d-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a658d-136">displayName</span></span>|<span data-ttu-id="a658d-137">String</span><span class="sxs-lookup"><span data-stu-id="a658d-137">String</span></span>|<span data-ttu-id="a658d-138">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a658d-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a658d-139">описание</span><span class="sxs-lookup"><span data-stu-id="a658d-139">description</span></span>|<span data-ttu-id="a658d-140">String</span><span class="sxs-lookup"><span data-stu-id="a658d-140">String</span></span>|<span data-ttu-id="a658d-141">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a658d-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a658d-142">priority</span><span class="sxs-lookup"><span data-stu-id="a658d-142">priority</span></span>|<span data-ttu-id="a658d-143">Int32</span><span class="sxs-lookup"><span data-stu-id="a658d-143">Int32</span></span>|<span data-ttu-id="a658d-144">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a658d-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a658d-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a658d-145">createdDateTime</span></span>|<span data-ttu-id="a658d-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a658d-146">DateTimeOffset</span></span>|<span data-ttu-id="a658d-147">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a658d-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a658d-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a658d-148">lastModifiedDateTime</span></span>|<span data-ttu-id="a658d-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a658d-149">DateTimeOffset</span></span>|<span data-ttu-id="a658d-150">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a658d-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a658d-151">version</span><span class="sxs-lookup"><span data-stu-id="a658d-151">version</span></span>|<span data-ttu-id="a658d-152">Int32</span><span class="sxs-lookup"><span data-stu-id="a658d-152">Int32</span></span>|<span data-ttu-id="a658d-153">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a658d-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a658d-154">limit</span><span class="sxs-lookup"><span data-stu-id="a658d-154">limit</span></span>|<span data-ttu-id="a658d-155">Int32</span><span class="sxs-lookup"><span data-stu-id="a658d-155">Int32</span></span>|<span data-ttu-id="a658d-156">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a658d-156">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a658d-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="a658d-157">Response</span></span>
<span data-ttu-id="a658d-158">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a658d-158">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a658d-159">Пример</span><span class="sxs-lookup"><span data-stu-id="a658d-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="a658d-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="a658d-160">Request</span></span>
<span data-ttu-id="a658d-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a658d-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 269

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "limit": 5
}
```

### <a name="response"></a><span data-ttu-id="a658d-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="a658d-162">Response</span></span>
<span data-ttu-id="a658d-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="a658d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 377

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
  "id": "4f8c4e4c-4e4c-4f8c-4c4e-8c4f4c4e8c4f",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "limit": 5
}
```





