---
title: Создание объекта deviceEnrollmentLimitConfiguration
description: Создание объекта deviceEnrollmentLimitConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9b1bd0eb77340f9278862bfc42e9bec68843b935
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956019"
---
# <a name="create-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="eb94c-103">Создание объекта deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="eb94c-103">Create deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="eb94c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="eb94c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eb94c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb94c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eb94c-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="eb94c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eb94c-107">Создание объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eb94c-107">Create a new [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="eb94c-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="eb94c-108">Prerequisites</span></span>
<span data-ttu-id="eb94c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb94c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb94c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eb94c-111">Permission type</span></span>|<span data-ttu-id="eb94c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="eb94c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb94c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eb94c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="eb94c-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb94c-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="eb94c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eb94c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb94c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb94c-116">Not supported.</span></span>|
|<span data-ttu-id="eb94c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eb94c-117">Application</span></span>|<span data-ttu-id="eb94c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb94c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb94c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eb94c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="eb94c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eb94c-120">Request headers</span></span>
|<span data-ttu-id="eb94c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="eb94c-121">Header</span></span>|<span data-ttu-id="eb94c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="eb94c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb94c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb94c-123">Authorization</span></span>|<span data-ttu-id="eb94c-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="eb94c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb94c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="eb94c-125">Accept</span></span>|<span data-ttu-id="eb94c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="eb94c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb94c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eb94c-127">Request body</span></span>
<span data-ttu-id="eb94c-128">В тексте запроса добавьте представление объекта deviceEnrollmentLimitConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eb94c-128">In the request body, supply a JSON representation for the deviceEnrollmentLimitConfiguration object.</span></span>

<span data-ttu-id="eb94c-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceEnrollmentLimitConfiguration.</span><span class="sxs-lookup"><span data-stu-id="eb94c-129">The following table shows the properties that are required when you create the deviceEnrollmentLimitConfiguration.</span></span>

|<span data-ttu-id="eb94c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="eb94c-130">Property</span></span>|<span data-ttu-id="eb94c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="eb94c-131">Type</span></span>|<span data-ttu-id="eb94c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="eb94c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb94c-133">id</span><span class="sxs-lookup"><span data-stu-id="eb94c-133">id</span></span>|<span data-ttu-id="eb94c-134">String</span><span class="sxs-lookup"><span data-stu-id="eb94c-134">String</span></span>|<span data-ttu-id="eb94c-135">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eb94c-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="eb94c-136">displayName</span><span class="sxs-lookup"><span data-stu-id="eb94c-136">displayName</span></span>|<span data-ttu-id="eb94c-137">String</span><span class="sxs-lookup"><span data-stu-id="eb94c-137">String</span></span>|<span data-ttu-id="eb94c-138">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eb94c-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="eb94c-139">описание</span><span class="sxs-lookup"><span data-stu-id="eb94c-139">description</span></span>|<span data-ttu-id="eb94c-140">String</span><span class="sxs-lookup"><span data-stu-id="eb94c-140">String</span></span>|<span data-ttu-id="eb94c-141">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eb94c-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="eb94c-142">priority</span><span class="sxs-lookup"><span data-stu-id="eb94c-142">priority</span></span>|<span data-ttu-id="eb94c-143">Int32</span><span class="sxs-lookup"><span data-stu-id="eb94c-143">Int32</span></span>|<span data-ttu-id="eb94c-144">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eb94c-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="eb94c-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eb94c-145">createdDateTime</span></span>|<span data-ttu-id="eb94c-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb94c-146">DateTimeOffset</span></span>|<span data-ttu-id="eb94c-147">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eb94c-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="eb94c-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eb94c-148">lastModifiedDateTime</span></span>|<span data-ttu-id="eb94c-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb94c-149">DateTimeOffset</span></span>|<span data-ttu-id="eb94c-150">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eb94c-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="eb94c-151">version</span><span class="sxs-lookup"><span data-stu-id="eb94c-151">version</span></span>|<span data-ttu-id="eb94c-152">Int32</span><span class="sxs-lookup"><span data-stu-id="eb94c-152">Int32</span></span>|<span data-ttu-id="eb94c-153">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eb94c-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="eb94c-154">limit</span><span class="sxs-lookup"><span data-stu-id="eb94c-154">limit</span></span>|<span data-ttu-id="eb94c-155">Int32</span><span class="sxs-lookup"><span data-stu-id="eb94c-155">Int32</span></span>|<span data-ttu-id="eb94c-156">Н/Д</span><span class="sxs-lookup"><span data-stu-id="eb94c-156">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="eb94c-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="eb94c-157">Response</span></span>
<span data-ttu-id="eb94c-158">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="eb94c-158">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb94c-159">Пример</span><span class="sxs-lookup"><span data-stu-id="eb94c-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="eb94c-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="eb94c-160">Request</span></span>
<span data-ttu-id="eb94c-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eb94c-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="eb94c-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="eb94c-162">Response</span></span>
<span data-ttu-id="eb94c-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="eb94c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





