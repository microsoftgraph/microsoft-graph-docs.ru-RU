---
title: Создание объекта deviceEnrollmentLimitConfiguration
description: Создание объекта deviceEnrollmentLimitConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 818560655b15215542ca9bdea12bd84430eebc5c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36353038"
---
# <a name="create-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="2a604-103">Создание объекта deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="2a604-103">Create deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="2a604-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a604-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a604-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2a604-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a604-106">Создание объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2a604-106">Create a new [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2a604-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2a604-107">Prerequisites</span></span>
<span data-ttu-id="2a604-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a604-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a604-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2a604-110">Permission type</span></span>|<span data-ttu-id="2a604-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2a604-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a604-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2a604-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2a604-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a604-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2a604-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2a604-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a604-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a604-115">Not supported.</span></span>|
|<span data-ttu-id="2a604-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2a604-116">Application</span></span>|<span data-ttu-id="2a604-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a604-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a604-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2a604-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2a604-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2a604-119">Request headers</span></span>
|<span data-ttu-id="2a604-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2a604-120">Header</span></span>|<span data-ttu-id="2a604-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2a604-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a604-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2a604-122">Authorization</span></span>|<span data-ttu-id="2a604-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2a604-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a604-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2a604-124">Accept</span></span>|<span data-ttu-id="2a604-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2a604-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a604-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2a604-126">Request body</span></span>
<span data-ttu-id="2a604-127">В тексте запроса добавьте представление объекта deviceEnrollmentLimitConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2a604-127">In the request body, supply a JSON representation for the deviceEnrollmentLimitConfiguration object.</span></span>

<span data-ttu-id="2a604-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceEnrollmentLimitConfiguration.</span><span class="sxs-lookup"><span data-stu-id="2a604-128">The following table shows the properties that are required when you create the deviceEnrollmentLimitConfiguration.</span></span>

|<span data-ttu-id="2a604-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="2a604-129">Property</span></span>|<span data-ttu-id="2a604-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2a604-130">Type</span></span>|<span data-ttu-id="2a604-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2a604-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a604-132">id</span><span class="sxs-lookup"><span data-stu-id="2a604-132">id</span></span>|<span data-ttu-id="2a604-133">String</span><span class="sxs-lookup"><span data-stu-id="2a604-133">String</span></span>|<span data-ttu-id="2a604-134">Уникальный идентификатор для учетной записи, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2a604-134">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2a604-135">displayName</span><span class="sxs-lookup"><span data-stu-id="2a604-135">displayName</span></span>|<span data-ttu-id="2a604-136">Строка</span><span class="sxs-lookup"><span data-stu-id="2a604-136">String</span></span>|<span data-ttu-id="2a604-137">Отображаемое имя конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2a604-137">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2a604-138">description</span><span class="sxs-lookup"><span data-stu-id="2a604-138">description</span></span>|<span data-ttu-id="2a604-139">String</span><span class="sxs-lookup"><span data-stu-id="2a604-139">String</span></span>|<span data-ttu-id="2a604-140">Описание конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2a604-140">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2a604-141">priority</span><span class="sxs-lookup"><span data-stu-id="2a604-141">priority</span></span>|<span data-ttu-id="2a604-142">Int32</span><span class="sxs-lookup"><span data-stu-id="2a604-142">Int32</span></span>|<span data-ttu-id="2a604-143">Priority используется, когда пользователь существует в нескольких группах, которым назначена Настройка регистрации.</span><span class="sxs-lookup"><span data-stu-id="2a604-143">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="2a604-144">Пользователи подчиняются только конфигурации с наименьшим значением приоритета.</span><span class="sxs-lookup"><span data-stu-id="2a604-144">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="2a604-145">Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2a604-145">Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2a604-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2a604-146">createdDateTime</span></span>|<span data-ttu-id="2a604-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a604-147">DateTimeOffset</span></span>|<span data-ttu-id="2a604-148">Созданная Дата и время в формате UTC для настройки регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2a604-148">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2a604-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2a604-149">lastModifiedDateTime</span></span>|<span data-ttu-id="2a604-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a604-150">DateTimeOffset</span></span>|<span data-ttu-id="2a604-151">Дата и время последнего изменения конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2a604-151">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2a604-152">version</span><span class="sxs-lookup"><span data-stu-id="2a604-152">version</span></span>|<span data-ttu-id="2a604-153">Int32</span><span class="sxs-lookup"><span data-stu-id="2a604-153">Int32</span></span>|<span data-ttu-id="2a604-154">Версия конфигурации регистрации устройств, унаследованная от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2a604-154">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2a604-155">limit</span><span class="sxs-lookup"><span data-stu-id="2a604-155">limit</span></span>|<span data-ttu-id="2a604-156">Int32</span><span class="sxs-lookup"><span data-stu-id="2a604-156">Int32</span></span>|<span data-ttu-id="2a604-157">Максимальное число устройств, которые может регистрировать пользователь</span><span class="sxs-lookup"><span data-stu-id="2a604-157">The maximum number of devices that a user can enroll</span></span>|



## <a name="response"></a><span data-ttu-id="2a604-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a604-158">Response</span></span>
<span data-ttu-id="2a604-159">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2a604-159">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a604-160">Пример</span><span class="sxs-lookup"><span data-stu-id="2a604-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="2a604-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="2a604-161">Request</span></span>
<span data-ttu-id="2a604-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2a604-162">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
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

### <a name="response"></a><span data-ttu-id="2a604-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a604-163">Response</span></span>
<span data-ttu-id="2a604-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2a604-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






