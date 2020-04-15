---
title: Create macOSGeneralDeviceConfiguration
description: Создание объекта macOSGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2067ff6847f2419f7aa6885129c64dbeb097290f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43387857"
---
# <a name="create-macosgeneraldeviceconfiguration"></a><span data-ttu-id="0d876-103">Create macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="0d876-103">Create macOSGeneralDeviceConfiguration</span></span>

<span data-ttu-id="0d876-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d876-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0d876-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0d876-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d876-106">Создание объекта [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0d876-106">Create a new [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0d876-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="0d876-107">Prerequisites</span></span>
<span data-ttu-id="0d876-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d876-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d876-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0d876-110">Permission type</span></span>|<span data-ttu-id="0d876-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0d876-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d876-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0d876-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0d876-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d876-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0d876-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0d876-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d876-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d876-115">Not supported.</span></span>|
|<span data-ttu-id="0d876-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0d876-116">Application</span></span>|<span data-ttu-id="0d876-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d876-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d876-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0d876-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0d876-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0d876-119">Request headers</span></span>
|<span data-ttu-id="0d876-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0d876-120">Header</span></span>|<span data-ttu-id="0d876-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0d876-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d876-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d876-122">Authorization</span></span>|<span data-ttu-id="0d876-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0d876-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d876-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0d876-124">Accept</span></span>|<span data-ttu-id="0d876-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0d876-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d876-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0d876-126">Request body</span></span>
<span data-ttu-id="0d876-127">В тексте запроса добавьте представление объекта macOSGeneralDeviceConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0d876-127">In the request body, supply a JSON representation for the macOSGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="0d876-128">В приведенной ниже таблице показаны, которые необходимо указывать при создании объекта macOSGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="0d876-128">The following table shows the properties that are required when you create the macOSGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="0d876-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="0d876-129">Property</span></span>|<span data-ttu-id="0d876-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0d876-130">Type</span></span>|<span data-ttu-id="0d876-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0d876-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d876-132">id</span><span class="sxs-lookup"><span data-stu-id="0d876-132">id</span></span>|<span data-ttu-id="0d876-133">String</span><span class="sxs-lookup"><span data-stu-id="0d876-133">String</span></span>|<span data-ttu-id="0d876-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0d876-134">Key of the entity.</span></span> <span data-ttu-id="0d876-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0d876-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d876-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0d876-136">lastModifiedDateTime</span></span>|<span data-ttu-id="0d876-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d876-137">DateTimeOffset</span></span>|<span data-ttu-id="0d876-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="0d876-138">DateTime the object was last modified.</span></span> <span data-ttu-id="0d876-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0d876-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d876-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0d876-140">createdDateTime</span></span>|<span data-ttu-id="0d876-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d876-141">DateTimeOffset</span></span>|<span data-ttu-id="0d876-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="0d876-142">DateTime the object was created.</span></span> <span data-ttu-id="0d876-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0d876-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d876-144">description</span><span class="sxs-lookup"><span data-stu-id="0d876-144">description</span></span>|<span data-ttu-id="0d876-145">String</span><span class="sxs-lookup"><span data-stu-id="0d876-145">String</span></span>|<span data-ttu-id="0d876-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0d876-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0d876-147">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0d876-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d876-148">displayName</span><span class="sxs-lookup"><span data-stu-id="0d876-148">displayName</span></span>|<span data-ttu-id="0d876-149">Строка</span><span class="sxs-lookup"><span data-stu-id="0d876-149">String</span></span>|<span data-ttu-id="0d876-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0d876-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0d876-151">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0d876-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d876-152">version</span><span class="sxs-lookup"><span data-stu-id="0d876-152">version</span></span>|<span data-ttu-id="0d876-153">Int32</span><span class="sxs-lookup"><span data-stu-id="0d876-153">Int32</span></span>|<span data-ttu-id="0d876-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0d876-154">Version of the device configuration.</span></span> <span data-ttu-id="0d876-155">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0d876-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d876-156">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="0d876-156">compliantAppsList</span></span>|<span data-ttu-id="0d876-157">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="0d876-157">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="0d876-158">Список приложений, соответствующих требованиям (список разрешений или блокировок, определяется свойством CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="0d876-158">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="0d876-159">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="0d876-159">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="0d876-160">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="0d876-160">compliantAppListType</span></span>|[<span data-ttu-id="0d876-161">апплисттипе</span><span class="sxs-lookup"><span data-stu-id="0d876-161">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="0d876-162">Список, включенный в CompliantAppsList.</span><span class="sxs-lookup"><span data-stu-id="0d876-162">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="0d876-163">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="0d876-163">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="0d876-164">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="0d876-164">emailInDomainSuffixes</span></span>|<span data-ttu-id="0d876-165">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0d876-165">String collection</span></span>|<span data-ttu-id="0d876-166">Электронный адрес без суффикса, соответствующего одной из этих строк, будет считаться не добавленным в домен.</span><span class="sxs-lookup"><span data-stu-id="0d876-166">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="0d876-167">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="0d876-167">passwordBlockSimple</span></span>|<span data-ttu-id="0d876-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="0d876-168">Boolean</span></span>|<span data-ttu-id="0d876-169">Блокировка простых паролей.</span><span class="sxs-lookup"><span data-stu-id="0d876-169">Block simple passwords.</span></span>|
|<span data-ttu-id="0d876-170">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="0d876-170">passwordExpirationDays</span></span>|<span data-ttu-id="0d876-171">Int32</span><span class="sxs-lookup"><span data-stu-id="0d876-171">Int32</span></span>|<span data-ttu-id="0d876-172">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="0d876-172">Number of days before the password expires.</span></span>|
|<span data-ttu-id="0d876-173">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="0d876-173">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="0d876-174">Int32</span><span class="sxs-lookup"><span data-stu-id="0d876-174">Int32</span></span>|<span data-ttu-id="0d876-175">Количество наборов символов, которые должен содержать пароль.</span><span class="sxs-lookup"><span data-stu-id="0d876-175">Number of character sets a password must contain.</span></span> <span data-ttu-id="0d876-176">Допустимые значения: от 0 до 4.</span><span class="sxs-lookup"><span data-stu-id="0d876-176">Valid values 0 to 4</span></span>|
|<span data-ttu-id="0d876-177">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="0d876-177">passwordMinimumLength</span></span>|<span data-ttu-id="0d876-178">Int32</span><span class="sxs-lookup"><span data-stu-id="0d876-178">Int32</span></span>|<span data-ttu-id="0d876-179">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="0d876-179">Minimum length of passwords.</span></span>|
|<span data-ttu-id="0d876-180">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="0d876-180">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="0d876-181">Int32</span><span class="sxs-lookup"><span data-stu-id="0d876-181">Int32</span></span>|<span data-ttu-id="0d876-182">Период бездействия (в минутах), по истечении которого будет запрашиваться пароль.</span><span class="sxs-lookup"><span data-stu-id="0d876-182">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="0d876-183">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="0d876-183">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="0d876-184">Int32</span><span class="sxs-lookup"><span data-stu-id="0d876-184">Int32</span></span>|<span data-ttu-id="0d876-185">Период бездействия (в минутах), по истечении которого будет гаснуть экран.</span><span class="sxs-lookup"><span data-stu-id="0d876-185">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="0d876-186">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="0d876-186">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="0d876-187">Int32</span><span class="sxs-lookup"><span data-stu-id="0d876-187">Int32</span></span>|<span data-ttu-id="0d876-188">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="0d876-188">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="0d876-189">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="0d876-189">passwordRequiredType</span></span>|[<span data-ttu-id="0d876-190">рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="0d876-190">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="0d876-191">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="0d876-191">Type of password that is required.</span></span> <span data-ttu-id="0d876-192">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="0d876-192">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="0d876-193">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="0d876-193">passwordRequired</span></span>|<span data-ttu-id="0d876-194">Логический</span><span class="sxs-lookup"><span data-stu-id="0d876-194">Boolean</span></span>|<span data-ttu-id="0d876-195">Указывает, обязательно ли использовать пароль.</span><span class="sxs-lookup"><span data-stu-id="0d876-195">Whether or not to require a password.</span></span>|



## <a name="response"></a><span data-ttu-id="0d876-196">Ответ</span><span class="sxs-lookup"><span data-stu-id="0d876-196">Response</span></span>
<span data-ttu-id="0d876-197">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="0d876-197">If successful, this method returns a `201 Created` response code and a [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d876-198">Пример</span><span class="sxs-lookup"><span data-stu-id="0d876-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="0d876-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d876-199">Request</span></span>
<span data-ttu-id="0d876-200">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0d876-200">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 906

{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumCharacterSetCount": 0,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true
}
```

### <a name="response"></a><span data-ttu-id="0d876-201">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d876-201">Response</span></span>
<span data-ttu-id="0d876-p112">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0d876-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1078

{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
  "id": "dc356aee-6aee-dc35-ee6a-35dcee6a35dc",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumCharacterSetCount": 0,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true
}
```






