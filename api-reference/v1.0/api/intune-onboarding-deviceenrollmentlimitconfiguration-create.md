---
title: Создание объекта deviceEnrollmentLimitConfiguration
description: Создание объекта deviceEnrollmentLimitConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4d6773086a44205a3ddb2c5603e2a898c5bfab10
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262155"
---
# <a name="create-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="021d6-103">Создание объекта deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="021d6-103">Create deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="021d6-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="021d6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="021d6-105">Создание объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="021d6-105">Create a new [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="021d6-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="021d6-106">Prerequisites</span></span>
<span data-ttu-id="021d6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="021d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="021d6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="021d6-109">Permission type</span></span>|<span data-ttu-id="021d6-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="021d6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="021d6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="021d6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="021d6-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="021d6-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="021d6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="021d6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="021d6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="021d6-114">Not supported.</span></span>|
|<span data-ttu-id="021d6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="021d6-115">Application</span></span>|<span data-ttu-id="021d6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="021d6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="021d6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="021d6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="021d6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="021d6-118">Request headers</span></span>
|<span data-ttu-id="021d6-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="021d6-119">Header</span></span>|<span data-ttu-id="021d6-120">Значение</span><span class="sxs-lookup"><span data-stu-id="021d6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="021d6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="021d6-121">Authorization</span></span>|<span data-ttu-id="021d6-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="021d6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="021d6-123">Accept</span><span class="sxs-lookup"><span data-stu-id="021d6-123">Accept</span></span>|<span data-ttu-id="021d6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="021d6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="021d6-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="021d6-125">Request body</span></span>
<span data-ttu-id="021d6-126">В тексте запроса добавьте представление объекта deviceEnrollmentLimitConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="021d6-126">In the request body, supply a JSON representation for the deviceEnrollmentLimitConfiguration object.</span></span>

<span data-ttu-id="021d6-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceEnrollmentLimitConfiguration.</span><span class="sxs-lookup"><span data-stu-id="021d6-127">The following table shows the properties that are required when you create the deviceEnrollmentLimitConfiguration.</span></span>

|<span data-ttu-id="021d6-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="021d6-128">Property</span></span>|<span data-ttu-id="021d6-129">Тип</span><span class="sxs-lookup"><span data-stu-id="021d6-129">Type</span></span>|<span data-ttu-id="021d6-130">Описание</span><span class="sxs-lookup"><span data-stu-id="021d6-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="021d6-131">id</span><span class="sxs-lookup"><span data-stu-id="021d6-131">id</span></span>|<span data-ttu-id="021d6-132">String</span><span class="sxs-lookup"><span data-stu-id="021d6-132">String</span></span>|<span data-ttu-id="021d6-133">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="021d6-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="021d6-134">displayName</span><span class="sxs-lookup"><span data-stu-id="021d6-134">displayName</span></span>|<span data-ttu-id="021d6-135">String</span><span class="sxs-lookup"><span data-stu-id="021d6-135">String</span></span>|<span data-ttu-id="021d6-136">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="021d6-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="021d6-137">description</span><span class="sxs-lookup"><span data-stu-id="021d6-137">description</span></span>|<span data-ttu-id="021d6-138">String</span><span class="sxs-lookup"><span data-stu-id="021d6-138">String</span></span>|<span data-ttu-id="021d6-139">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="021d6-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="021d6-140">priority</span><span class="sxs-lookup"><span data-stu-id="021d6-140">priority</span></span>|<span data-ttu-id="021d6-141">Int32</span><span class="sxs-lookup"><span data-stu-id="021d6-141">Int32</span></span>|<span data-ttu-id="021d6-142">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="021d6-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="021d6-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="021d6-143">createdDateTime</span></span>|<span data-ttu-id="021d6-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="021d6-144">DateTimeOffset</span></span>|<span data-ttu-id="021d6-145">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="021d6-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="021d6-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="021d6-146">lastModifiedDateTime</span></span>|<span data-ttu-id="021d6-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="021d6-147">DateTimeOffset</span></span>|<span data-ttu-id="021d6-148">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="021d6-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="021d6-149">version</span><span class="sxs-lookup"><span data-stu-id="021d6-149">version</span></span>|<span data-ttu-id="021d6-150">Int32</span><span class="sxs-lookup"><span data-stu-id="021d6-150">Int32</span></span>|<span data-ttu-id="021d6-151">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="021d6-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="021d6-152">limit</span><span class="sxs-lookup"><span data-stu-id="021d6-152">limit</span></span>|<span data-ttu-id="021d6-153">Int32</span><span class="sxs-lookup"><span data-stu-id="021d6-153">Int32</span></span>|<span data-ttu-id="021d6-154">Н/Д</span><span class="sxs-lookup"><span data-stu-id="021d6-154">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="021d6-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="021d6-155">Response</span></span>
<span data-ttu-id="021d6-156">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="021d6-156">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="021d6-157">Пример</span><span class="sxs-lookup"><span data-stu-id="021d6-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="021d6-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="021d6-158">Request</span></span>
<span data-ttu-id="021d6-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="021d6-159">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 205

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "limit": 5
}
```

### <a name="response"></a><span data-ttu-id="021d6-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="021d6-160">Response</span></span>
<span data-ttu-id="021d6-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="021d6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



