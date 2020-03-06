---
title: Create macOSGeneralDeviceConfiguration
description: Создание объекта macOSGeneralDeviceConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: db1062a779aeea498c129e9fb8039365488b6bdb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42514328"
---
# <a name="create-macosgeneraldeviceconfiguration"></a><span data-ttu-id="de6b0-103">Create macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="de6b0-103">Create macOSGeneralDeviceConfiguration</span></span>

<span data-ttu-id="de6b0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de6b0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="de6b0-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="de6b0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de6b0-106">Создание объекта [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="de6b0-106">Create a new [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="de6b0-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="de6b0-107">Prerequisites</span></span>
<span data-ttu-id="de6b0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de6b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de6b0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de6b0-110">Permission type</span></span>|<span data-ttu-id="de6b0-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="de6b0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de6b0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de6b0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="de6b0-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de6b0-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="de6b0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de6b0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de6b0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de6b0-115">Not supported.</span></span>|
|<span data-ttu-id="de6b0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="de6b0-116">Application</span></span>|<span data-ttu-id="de6b0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de6b0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="de6b0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de6b0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="de6b0-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="de6b0-119">Request headers</span></span>
|<span data-ttu-id="de6b0-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="de6b0-120">Header</span></span>|<span data-ttu-id="de6b0-121">Значение</span><span class="sxs-lookup"><span data-stu-id="de6b0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de6b0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="de6b0-122">Authorization</span></span>|<span data-ttu-id="de6b0-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="de6b0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de6b0-124">Accept</span><span class="sxs-lookup"><span data-stu-id="de6b0-124">Accept</span></span>|<span data-ttu-id="de6b0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="de6b0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de6b0-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="de6b0-126">Request body</span></span>
<span data-ttu-id="de6b0-127">В тексте запроса добавьте представление объекта macOSGeneralDeviceConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="de6b0-127">In the request body, supply a JSON representation for the macOSGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="de6b0-128">В приведенной ниже таблице показаны, которые необходимо указывать при создании объекта macOSGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="de6b0-128">The following table shows the properties that are required when you create the macOSGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="de6b0-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="de6b0-129">Property</span></span>|<span data-ttu-id="de6b0-130">Тип</span><span class="sxs-lookup"><span data-stu-id="de6b0-130">Type</span></span>|<span data-ttu-id="de6b0-131">Описание</span><span class="sxs-lookup"><span data-stu-id="de6b0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de6b0-132">id</span><span class="sxs-lookup"><span data-stu-id="de6b0-132">id</span></span>|<span data-ttu-id="de6b0-133">String</span><span class="sxs-lookup"><span data-stu-id="de6b0-133">String</span></span>|<span data-ttu-id="de6b0-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="de6b0-134">Key of the entity.</span></span> <span data-ttu-id="de6b0-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="de6b0-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de6b0-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="de6b0-136">lastModifiedDateTime</span></span>|<span data-ttu-id="de6b0-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de6b0-137">DateTimeOffset</span></span>|<span data-ttu-id="de6b0-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="de6b0-138">DateTime the object was last modified.</span></span> <span data-ttu-id="de6b0-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="de6b0-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de6b0-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="de6b0-140">createdDateTime</span></span>|<span data-ttu-id="de6b0-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de6b0-141">DateTimeOffset</span></span>|<span data-ttu-id="de6b0-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="de6b0-142">DateTime the object was created.</span></span> <span data-ttu-id="de6b0-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="de6b0-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de6b0-144">description</span><span class="sxs-lookup"><span data-stu-id="de6b0-144">description</span></span>|<span data-ttu-id="de6b0-145">String</span><span class="sxs-lookup"><span data-stu-id="de6b0-145">String</span></span>|<span data-ttu-id="de6b0-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="de6b0-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="de6b0-147">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="de6b0-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de6b0-148">displayName</span><span class="sxs-lookup"><span data-stu-id="de6b0-148">displayName</span></span>|<span data-ttu-id="de6b0-149">Строка</span><span class="sxs-lookup"><span data-stu-id="de6b0-149">String</span></span>|<span data-ttu-id="de6b0-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="de6b0-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="de6b0-151">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="de6b0-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de6b0-152">version</span><span class="sxs-lookup"><span data-stu-id="de6b0-152">version</span></span>|<span data-ttu-id="de6b0-153">Int32</span><span class="sxs-lookup"><span data-stu-id="de6b0-153">Int32</span></span>|<span data-ttu-id="de6b0-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="de6b0-154">Version of the device configuration.</span></span> <span data-ttu-id="de6b0-155">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de6b0-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de6b0-156">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="de6b0-156">compliantAppsList</span></span>|<span data-ttu-id="de6b0-157">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="de6b0-157">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="de6b0-158">Список приложений, соответствующих требованиям (список разрешений или блокировок, определяется свойством CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="de6b0-158">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="de6b0-159">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="de6b0-159">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="de6b0-160">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="de6b0-160">compliantAppListType</span></span>|[<span data-ttu-id="de6b0-161">апплисттипе</span><span class="sxs-lookup"><span data-stu-id="de6b0-161">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="de6b0-162">Список, включенный в CompliantAppsList.</span><span class="sxs-lookup"><span data-stu-id="de6b0-162">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="de6b0-163">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="de6b0-163">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="de6b0-164">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="de6b0-164">emailInDomainSuffixes</span></span>|<span data-ttu-id="de6b0-165">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="de6b0-165">String collection</span></span>|<span data-ttu-id="de6b0-166">Электронный адрес без суффикса, соответствующего одной из этих строк, будет считаться не добавленным в домен.</span><span class="sxs-lookup"><span data-stu-id="de6b0-166">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="de6b0-167">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="de6b0-167">passwordBlockSimple</span></span>|<span data-ttu-id="de6b0-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="de6b0-168">Boolean</span></span>|<span data-ttu-id="de6b0-169">Блокировка простых паролей.</span><span class="sxs-lookup"><span data-stu-id="de6b0-169">Block simple passwords.</span></span>|
|<span data-ttu-id="de6b0-170">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="de6b0-170">passwordExpirationDays</span></span>|<span data-ttu-id="de6b0-171">Int32</span><span class="sxs-lookup"><span data-stu-id="de6b0-171">Int32</span></span>|<span data-ttu-id="de6b0-172">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="de6b0-172">Number of days before the password expires.</span></span>|
|<span data-ttu-id="de6b0-173">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="de6b0-173">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="de6b0-174">Int32</span><span class="sxs-lookup"><span data-stu-id="de6b0-174">Int32</span></span>|<span data-ttu-id="de6b0-175">Количество наборов символов, которые должен содержать пароль.</span><span class="sxs-lookup"><span data-stu-id="de6b0-175">Number of character sets a password must contain.</span></span> <span data-ttu-id="de6b0-176">Допустимые значения: от 0 до 4.</span><span class="sxs-lookup"><span data-stu-id="de6b0-176">Valid values 0 to 4</span></span>|
|<span data-ttu-id="de6b0-177">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="de6b0-177">passwordMinimumLength</span></span>|<span data-ttu-id="de6b0-178">Int32</span><span class="sxs-lookup"><span data-stu-id="de6b0-178">Int32</span></span>|<span data-ttu-id="de6b0-179">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="de6b0-179">Minimum length of passwords.</span></span>|
|<span data-ttu-id="de6b0-180">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="de6b0-180">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="de6b0-181">Int32</span><span class="sxs-lookup"><span data-stu-id="de6b0-181">Int32</span></span>|<span data-ttu-id="de6b0-182">Период бездействия (в минутах), по истечении которого будет запрашиваться пароль.</span><span class="sxs-lookup"><span data-stu-id="de6b0-182">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="de6b0-183">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="de6b0-183">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="de6b0-184">Int32</span><span class="sxs-lookup"><span data-stu-id="de6b0-184">Int32</span></span>|<span data-ttu-id="de6b0-185">Период бездействия (в минутах), по истечении которого будет гаснуть экран.</span><span class="sxs-lookup"><span data-stu-id="de6b0-185">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="de6b0-186">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="de6b0-186">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="de6b0-187">Int32</span><span class="sxs-lookup"><span data-stu-id="de6b0-187">Int32</span></span>|<span data-ttu-id="de6b0-188">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="de6b0-188">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="de6b0-189">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="de6b0-189">passwordRequiredType</span></span>|[<span data-ttu-id="de6b0-190">рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="de6b0-190">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="de6b0-191">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="de6b0-191">Type of password that is required.</span></span> <span data-ttu-id="de6b0-192">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="de6b0-192">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="de6b0-193">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="de6b0-193">passwordRequired</span></span>|<span data-ttu-id="de6b0-194">Логический</span><span class="sxs-lookup"><span data-stu-id="de6b0-194">Boolean</span></span>|<span data-ttu-id="de6b0-195">Указывает, обязательно ли использовать пароль.</span><span class="sxs-lookup"><span data-stu-id="de6b0-195">Whether or not to require a password.</span></span>|



## <a name="response"></a><span data-ttu-id="de6b0-196">Ответ</span><span class="sxs-lookup"><span data-stu-id="de6b0-196">Response</span></span>
<span data-ttu-id="de6b0-197">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="de6b0-197">If successful, this method returns a `201 Created` response code and a [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de6b0-198">Пример</span><span class="sxs-lookup"><span data-stu-id="de6b0-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="de6b0-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="de6b0-199">Request</span></span>
<span data-ttu-id="de6b0-200">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="de6b0-200">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="de6b0-201">Отклик</span><span class="sxs-lookup"><span data-stu-id="de6b0-201">Response</span></span>
<span data-ttu-id="de6b0-p112">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="de6b0-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




