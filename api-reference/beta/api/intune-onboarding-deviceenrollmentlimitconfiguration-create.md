---
title: Создание объекта deviceEnrollmentLimitConfiguration
description: Создание объекта deviceEnrollmentLimitConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7509be622b9e89ba35d65730018b8158a3444d6b
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135084"
---
# <a name="create-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="c1977-103">Создание объекта deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="c1977-103">Create deviceEnrollmentLimitConfiguration</span></span>

<span data-ttu-id="c1977-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1977-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c1977-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1977-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1977-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c1977-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1977-107">Создание объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1977-107">Create a new [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c1977-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c1977-108">Prerequisites</span></span>
<span data-ttu-id="c1977-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1977-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1977-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c1977-111">Permission type</span></span>|<span data-ttu-id="c1977-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c1977-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1977-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c1977-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c1977-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1977-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c1977-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c1977-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1977-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1977-116">Not supported.</span></span>|
|<span data-ttu-id="c1977-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="c1977-117">Application</span></span>|<span data-ttu-id="c1977-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1977-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1977-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c1977-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c1977-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c1977-120">Request headers</span></span>
|<span data-ttu-id="c1977-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c1977-121">Header</span></span>|<span data-ttu-id="c1977-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c1977-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1977-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1977-123">Authorization</span></span>|<span data-ttu-id="c1977-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c1977-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1977-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c1977-125">Accept</span></span>|<span data-ttu-id="c1977-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c1977-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1977-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c1977-127">Request body</span></span>
<span data-ttu-id="c1977-128">В тексте запроса добавьте представление объекта deviceEnrollmentLimitConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c1977-128">In the request body, supply a JSON representation for the deviceEnrollmentLimitConfiguration object.</span></span>

<span data-ttu-id="c1977-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceEnrollmentLimitConfiguration.</span><span class="sxs-lookup"><span data-stu-id="c1977-129">The following table shows the properties that are required when you create the deviceEnrollmentLimitConfiguration.</span></span>

|<span data-ttu-id="c1977-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c1977-130">Property</span></span>|<span data-ttu-id="c1977-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c1977-131">Type</span></span>|<span data-ttu-id="c1977-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c1977-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1977-133">id</span><span class="sxs-lookup"><span data-stu-id="c1977-133">id</span></span>|<span data-ttu-id="c1977-134">Строка</span><span class="sxs-lookup"><span data-stu-id="c1977-134">String</span></span>|<span data-ttu-id="c1977-135">Уникальный идентификатор учетной записи, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1977-135">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c1977-136">displayName</span><span class="sxs-lookup"><span data-stu-id="c1977-136">displayName</span></span>|<span data-ttu-id="c1977-137">Строка</span><span class="sxs-lookup"><span data-stu-id="c1977-137">String</span></span>|<span data-ttu-id="c1977-138">Отображающее имя конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1977-138">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c1977-139">description</span><span class="sxs-lookup"><span data-stu-id="c1977-139">description</span></span>|<span data-ttu-id="c1977-140">Строка</span><span class="sxs-lookup"><span data-stu-id="c1977-140">String</span></span>|<span data-ttu-id="c1977-141">Описание конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1977-141">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c1977-142">priority</span><span class="sxs-lookup"><span data-stu-id="c1977-142">priority</span></span>|<span data-ttu-id="c1977-143">Int32</span><span class="sxs-lookup"><span data-stu-id="c1977-143">Int32</span></span>|<span data-ttu-id="c1977-144">Приоритет используется, когда пользователь существует в нескольких группах, которые назначены конфигурации регистрации.</span><span class="sxs-lookup"><span data-stu-id="c1977-144">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="c1977-145">Пользователи подчиняются только конфигурации с наименьшим значением приоритета.</span><span class="sxs-lookup"><span data-stu-id="c1977-145">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="c1977-146">Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1977-146">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c1977-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c1977-147">createdDateTime</span></span>|<span data-ttu-id="c1977-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1977-148">DateTimeOffset</span></span>|<span data-ttu-id="c1977-149">Создано время даты в UTC конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1977-149">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c1977-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c1977-150">lastModifiedDateTime</span></span>|<span data-ttu-id="c1977-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1977-151">DateTimeOffset</span></span>|<span data-ttu-id="c1977-152">Последнее измененное время даты в UTC конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1977-152">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c1977-153">version</span><span class="sxs-lookup"><span data-stu-id="c1977-153">version</span></span>|<span data-ttu-id="c1977-154">Int32</span><span class="sxs-lookup"><span data-stu-id="c1977-154">Int32</span></span>|<span data-ttu-id="c1977-155">Версия конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1977-155">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c1977-156">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c1977-156">roleScopeTagIds</span></span>|<span data-ttu-id="c1977-157">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c1977-157">String collection</span></span>|<span data-ttu-id="c1977-158">Необязательные теги области ролей для ограничений регистрации.</span><span class="sxs-lookup"><span data-stu-id="c1977-158">Optional role scope tags for the enrollment restrictions.</span></span> <span data-ttu-id="c1977-159">Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1977-159">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c1977-160">limit</span><span class="sxs-lookup"><span data-stu-id="c1977-160">limit</span></span>|<span data-ttu-id="c1977-161">Int32</span><span class="sxs-lookup"><span data-stu-id="c1977-161">Int32</span></span>|<span data-ttu-id="c1977-162">Максимальное число устройств, которые пользователь может записать</span><span class="sxs-lookup"><span data-stu-id="c1977-162">The maximum number of devices that a user can enroll</span></span>|



## <a name="response"></a><span data-ttu-id="c1977-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1977-163">Response</span></span>
<span data-ttu-id="c1977-164">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c1977-164">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1977-165">Пример</span><span class="sxs-lookup"><span data-stu-id="c1977-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1977-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1977-166">Request</span></span>
<span data-ttu-id="c1977-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c1977-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 267

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "limit": 5
}
```

### <a name="response"></a><span data-ttu-id="c1977-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1977-168">Response</span></span>
<span data-ttu-id="c1977-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c1977-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 439

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
  "id": "4f8c4e4c-4e4c-4f8c-4c4e-8c4f4c4e8c4f",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "limit": 5
}
```




