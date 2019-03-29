---
title: Create macOSGeneralDeviceConfiguration
description: Создание объекта macOSGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e02159e9f577e001a675de5ee64768f63d1090c0
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30979524"
---
# <a name="create-macosgeneraldeviceconfiguration"></a><span data-ttu-id="2d2de-103">Create macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="2d2de-103">Create macOSGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="2d2de-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2d2de-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d2de-105">Создание объекта [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2d2de-105">Create a new [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2d2de-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="2d2de-106">Prerequisites</span></span>
<span data-ttu-id="2d2de-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d2de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d2de-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2d2de-109">Permission type</span></span>|<span data-ttu-id="2d2de-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2d2de-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d2de-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2d2de-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2d2de-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d2de-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2d2de-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2d2de-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d2de-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d2de-114">Not supported.</span></span>|
|<span data-ttu-id="2d2de-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2d2de-115">Application</span></span>|<span data-ttu-id="2d2de-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d2de-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d2de-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2d2de-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2d2de-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2d2de-118">Request headers</span></span>
|<span data-ttu-id="2d2de-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2d2de-119">Header</span></span>|<span data-ttu-id="2d2de-120">Значение</span><span class="sxs-lookup"><span data-stu-id="2d2de-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d2de-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2d2de-121">Authorization</span></span>|<span data-ttu-id="2d2de-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2d2de-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2d2de-123">Accept</span><span class="sxs-lookup"><span data-stu-id="2d2de-123">Accept</span></span>|<span data-ttu-id="2d2de-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2d2de-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d2de-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2d2de-125">Request body</span></span>
<span data-ttu-id="2d2de-126">В тексте запроса добавьте представление объекта macOSGeneralDeviceConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2d2de-126">In the request body, supply a JSON representation for the macOSGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="2d2de-127">В приведенной ниже таблице показаны, которые необходимо указывать при создании объекта macOSGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="2d2de-127">The following table shows the properties that are required when you create the macOSGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="2d2de-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="2d2de-128">Property</span></span>|<span data-ttu-id="2d2de-129">Тип</span><span class="sxs-lookup"><span data-stu-id="2d2de-129">Type</span></span>|<span data-ttu-id="2d2de-130">Описание</span><span class="sxs-lookup"><span data-stu-id="2d2de-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d2de-131">id</span><span class="sxs-lookup"><span data-stu-id="2d2de-131">id</span></span>|<span data-ttu-id="2d2de-132">Строка</span><span class="sxs-lookup"><span data-stu-id="2d2de-132">String</span></span>|<span data-ttu-id="2d2de-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2d2de-133">Key of the entity.</span></span> <span data-ttu-id="2d2de-134">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2d2de-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d2de-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2d2de-135">lastModifiedDateTime</span></span>|<span data-ttu-id="2d2de-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d2de-136">DateTimeOffset</span></span>|<span data-ttu-id="2d2de-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="2d2de-137">DateTime the object was last modified.</span></span> <span data-ttu-id="2d2de-138">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2d2de-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d2de-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2d2de-139">createdDateTime</span></span>|<span data-ttu-id="2d2de-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d2de-140">DateTimeOffset</span></span>|<span data-ttu-id="2d2de-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="2d2de-141">DateTime the object was created.</span></span> <span data-ttu-id="2d2de-142">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2d2de-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d2de-143">description</span><span class="sxs-lookup"><span data-stu-id="2d2de-143">description</span></span>|<span data-ttu-id="2d2de-144">String</span><span class="sxs-lookup"><span data-stu-id="2d2de-144">String</span></span>|<span data-ttu-id="2d2de-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2d2de-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2d2de-146">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2d2de-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d2de-147">displayName</span><span class="sxs-lookup"><span data-stu-id="2d2de-147">displayName</span></span>|<span data-ttu-id="2d2de-148">String</span><span class="sxs-lookup"><span data-stu-id="2d2de-148">String</span></span>|<span data-ttu-id="2d2de-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2d2de-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2d2de-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2d2de-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d2de-151">version</span><span class="sxs-lookup"><span data-stu-id="2d2de-151">version</span></span>|<span data-ttu-id="2d2de-152">Int32</span><span class="sxs-lookup"><span data-stu-id="2d2de-152">Int32</span></span>|<span data-ttu-id="2d2de-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2d2de-153">Version of the device configuration.</span></span> <span data-ttu-id="2d2de-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2d2de-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d2de-155">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="2d2de-155">compliantAppsList</span></span>|<span data-ttu-id="2d2de-156">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="2d2de-156">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="2d2de-157">Список приложений, соответствующих требованиям (список разрешений или блокировок, определяется свойством CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="2d2de-157">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="2d2de-158">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="2d2de-158">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="2d2de-159">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="2d2de-159">compliantAppListType</span></span>|[<span data-ttu-id="2d2de-160">Апплисттипе</span><span class="sxs-lookup"><span data-stu-id="2d2de-160">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="2d2de-161">Список, включенный в CompliantAppsList.</span><span class="sxs-lookup"><span data-stu-id="2d2de-161">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="2d2de-162">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="2d2de-162">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="2d2de-163">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="2d2de-163">emailInDomainSuffixes</span></span>|<span data-ttu-id="2d2de-164">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2d2de-164">String collection</span></span>|<span data-ttu-id="2d2de-165">Электронный адрес без суффикса, соответствующего одной из этих строк, будет считаться не добавленным в домен.</span><span class="sxs-lookup"><span data-stu-id="2d2de-165">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="2d2de-166">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="2d2de-166">passwordBlockSimple</span></span>|<span data-ttu-id="2d2de-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d2de-167">Boolean</span></span>|<span data-ttu-id="2d2de-168">Блокировка простых паролей.</span><span class="sxs-lookup"><span data-stu-id="2d2de-168">Block simple passwords.</span></span>|
|<span data-ttu-id="2d2de-169">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="2d2de-169">passwordExpirationDays</span></span>|<span data-ttu-id="2d2de-170">Int32</span><span class="sxs-lookup"><span data-stu-id="2d2de-170">Int32</span></span>|<span data-ttu-id="2d2de-171">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="2d2de-171">Number of days before the password expires.</span></span>|
|<span data-ttu-id="2d2de-172">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="2d2de-172">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="2d2de-173">Int32</span><span class="sxs-lookup"><span data-stu-id="2d2de-173">Int32</span></span>|<span data-ttu-id="2d2de-174">Количество наборов символов, которые должен содержать пароль.</span><span class="sxs-lookup"><span data-stu-id="2d2de-174">Number of character sets a password must contain.</span></span> <span data-ttu-id="2d2de-175">Допустимые значения: от 0 до 4.</span><span class="sxs-lookup"><span data-stu-id="2d2de-175">Valid values 0 to 4</span></span>|
|<span data-ttu-id="2d2de-176">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="2d2de-176">passwordMinimumLength</span></span>|<span data-ttu-id="2d2de-177">Int32</span><span class="sxs-lookup"><span data-stu-id="2d2de-177">Int32</span></span>|<span data-ttu-id="2d2de-178">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="2d2de-178">Minimum length of passwords.</span></span>|
|<span data-ttu-id="2d2de-179">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="2d2de-179">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="2d2de-180">Int32</span><span class="sxs-lookup"><span data-stu-id="2d2de-180">Int32</span></span>|<span data-ttu-id="2d2de-181">Период бездействия (в минутах), по истечении которого будет запрашиваться пароль.</span><span class="sxs-lookup"><span data-stu-id="2d2de-181">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="2d2de-182">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="2d2de-182">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="2d2de-183">Int32</span><span class="sxs-lookup"><span data-stu-id="2d2de-183">Int32</span></span>|<span data-ttu-id="2d2de-184">Период бездействия (в минутах), по истечении которого будет гаснуть экран.</span><span class="sxs-lookup"><span data-stu-id="2d2de-184">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="2d2de-185">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="2d2de-185">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="2d2de-186">Int32</span><span class="sxs-lookup"><span data-stu-id="2d2de-186">Int32</span></span>|<span data-ttu-id="2d2de-187">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="2d2de-187">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="2d2de-188">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="2d2de-188">passwordRequiredType</span></span>|[<span data-ttu-id="2d2de-189">Рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="2d2de-189">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="2d2de-190">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="2d2de-190">Type of password that is required.</span></span> <span data-ttu-id="2d2de-191">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="2d2de-191">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="2d2de-192">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="2d2de-192">passwordRequired</span></span>|<span data-ttu-id="2d2de-193">Логический</span><span class="sxs-lookup"><span data-stu-id="2d2de-193">Boolean</span></span>|<span data-ttu-id="2d2de-194">Указывает, обязательно ли использовать пароль.</span><span class="sxs-lookup"><span data-stu-id="2d2de-194">Whether or not to require a password.</span></span>|



## <a name="response"></a><span data-ttu-id="2d2de-195">Ответ</span><span class="sxs-lookup"><span data-stu-id="2d2de-195">Response</span></span>
<span data-ttu-id="2d2de-196">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="2d2de-196">If successful, this method returns a `201 Created` response code and a [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d2de-197">Пример</span><span class="sxs-lookup"><span data-stu-id="2d2de-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="2d2de-198">Запрос</span><span class="sxs-lookup"><span data-stu-id="2d2de-198">Request</span></span>
<span data-ttu-id="2d2de-199">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2d2de-199">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2d2de-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d2de-200">Response</span></span>
<span data-ttu-id="2d2de-p112">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2d2de-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



