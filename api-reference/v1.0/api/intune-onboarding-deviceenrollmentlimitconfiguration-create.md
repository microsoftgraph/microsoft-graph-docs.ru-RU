---
title: Создание объекта deviceEnrollmentLimitConfiguration
description: Создание объекта deviceEnrollmentLimitConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4f3be4bb3cebe2e8dd08bff5764143d231680dfb
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52745074"
---
# <a name="create-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="5b074-103">Создание объекта deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="5b074-103">Create deviceEnrollmentLimitConfiguration</span></span>

<span data-ttu-id="5b074-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b074-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5b074-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5b074-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b074-106">Создание объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b074-106">Create a new [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5b074-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5b074-107">Prerequisites</span></span>
<span data-ttu-id="5b074-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b074-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b074-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5b074-110">Permission type</span></span>|<span data-ttu-id="5b074-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5b074-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b074-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b074-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5b074-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b074-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5b074-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b074-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b074-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b074-115">Not supported.</span></span>|
|<span data-ttu-id="5b074-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="5b074-116">Application</span></span>|<span data-ttu-id="5b074-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b074-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b074-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b074-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5b074-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5b074-119">Request headers</span></span>
|<span data-ttu-id="5b074-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5b074-120">Header</span></span>|<span data-ttu-id="5b074-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5b074-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b074-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b074-122">Authorization</span></span>|<span data-ttu-id="5b074-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b074-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b074-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5b074-124">Accept</span></span>|<span data-ttu-id="5b074-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5b074-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b074-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5b074-126">Request body</span></span>
<span data-ttu-id="5b074-127">В тексте запроса добавьте представление объекта deviceEnrollmentLimitConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5b074-127">In the request body, supply a JSON representation for the deviceEnrollmentLimitConfiguration object.</span></span>

<span data-ttu-id="5b074-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceEnrollmentLimitConfiguration.</span><span class="sxs-lookup"><span data-stu-id="5b074-128">The following table shows the properties that are required when you create the deviceEnrollmentLimitConfiguration.</span></span>

|<span data-ttu-id="5b074-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5b074-129">Property</span></span>|<span data-ttu-id="5b074-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5b074-130">Type</span></span>|<span data-ttu-id="5b074-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5b074-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b074-132">id</span><span class="sxs-lookup"><span data-stu-id="5b074-132">id</span></span>|<span data-ttu-id="5b074-133">String</span><span class="sxs-lookup"><span data-stu-id="5b074-133">String</span></span>|<span data-ttu-id="5b074-134">Уникальный идентификатор учетной записи, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5b074-134">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="5b074-135">displayName</span><span class="sxs-lookup"><span data-stu-id="5b074-135">displayName</span></span>|<span data-ttu-id="5b074-136">String</span><span class="sxs-lookup"><span data-stu-id="5b074-136">String</span></span>|<span data-ttu-id="5b074-137">Отображающее имя конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5b074-137">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="5b074-138">description</span><span class="sxs-lookup"><span data-stu-id="5b074-138">description</span></span>|<span data-ttu-id="5b074-139">String</span><span class="sxs-lookup"><span data-stu-id="5b074-139">String</span></span>|<span data-ttu-id="5b074-140">Описание конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5b074-140">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="5b074-141">priority</span><span class="sxs-lookup"><span data-stu-id="5b074-141">priority</span></span>|<span data-ttu-id="5b074-142">Int32</span><span class="sxs-lookup"><span data-stu-id="5b074-142">Int32</span></span>|<span data-ttu-id="5b074-143">Приоритет используется, когда пользователь существует в нескольких группах, которые назначены конфигурации регистрации.</span><span class="sxs-lookup"><span data-stu-id="5b074-143">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="5b074-144">Пользователи подчиняются только конфигурации с наименьшим значением приоритета.</span><span class="sxs-lookup"><span data-stu-id="5b074-144">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="5b074-145">Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5b074-145">Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="5b074-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5b074-146">createdDateTime</span></span>|<span data-ttu-id="5b074-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b074-147">DateTimeOffset</span></span>|<span data-ttu-id="5b074-148">Создано время даты в UTC конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5b074-148">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="5b074-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5b074-149">lastModifiedDateTime</span></span>|<span data-ttu-id="5b074-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b074-150">DateTimeOffset</span></span>|<span data-ttu-id="5b074-151">Последнее измененное время даты в UTC конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5b074-151">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="5b074-152">version</span><span class="sxs-lookup"><span data-stu-id="5b074-152">version</span></span>|<span data-ttu-id="5b074-153">Int32</span><span class="sxs-lookup"><span data-stu-id="5b074-153">Int32</span></span>|<span data-ttu-id="5b074-154">Версия конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5b074-154">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="5b074-155">limit</span><span class="sxs-lookup"><span data-stu-id="5b074-155">limit</span></span>|<span data-ttu-id="5b074-156">Int32</span><span class="sxs-lookup"><span data-stu-id="5b074-156">Int32</span></span>|<span data-ttu-id="5b074-157">Максимальное число устройств, которые пользователь может записать</span><span class="sxs-lookup"><span data-stu-id="5b074-157">The maximum number of devices that a user can enroll</span></span>|



## <a name="response"></a><span data-ttu-id="5b074-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b074-158">Response</span></span>
<span data-ttu-id="5b074-159">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5b074-159">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b074-160">Пример</span><span class="sxs-lookup"><span data-stu-id="5b074-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b074-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b074-161">Request</span></span>
<span data-ttu-id="5b074-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5b074-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5b074-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b074-163">Response</span></span>
<span data-ttu-id="5b074-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5b074-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




