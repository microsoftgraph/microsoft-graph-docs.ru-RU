---
title: Update macOSGeneralDeviceConfiguration
description: Обновление свойств объекта macOSGeneralDeviceConfiguration.
ms.openlocfilehash: a2ed3f7aa939f7df18389306cc840e3afdcaf856
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024376"
---
# <a name="update-macosgeneraldeviceconfiguration"></a><span data-ttu-id="6f5e8-103">Update macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="6f5e8-103">Update macOSGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="6f5e8-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6f5e8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6f5e8-105">Обновление свойств объекта [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f5e8-105">Update the properties of a [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6f5e8-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="6f5e8-106">Prerequisites</span></span>
<span data-ttu-id="6f5e8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f5e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f5e8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f5e8-109">Permission type</span></span>|<span data-ttu-id="6f5e8-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f5e8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f5e8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f5e8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6f5e8-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f5e8-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6f5e8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f5e8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f5e8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f5e8-114">Not supported.</span></span>|
|<span data-ttu-id="6f5e8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6f5e8-115">Application</span></span>|<span data-ttu-id="6f5e8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f5e8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f5e8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f5e8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6f5e8-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6f5e8-118">Request headers</span></span>
|<span data-ttu-id="6f5e8-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6f5e8-119">Header</span></span>|<span data-ttu-id="6f5e8-120">Значение</span><span class="sxs-lookup"><span data-stu-id="6f5e8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f5e8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f5e8-121">Authorization</span></span>|<span data-ttu-id="6f5e8-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6f5e8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f5e8-123">Accept</span><span class="sxs-lookup"><span data-stu-id="6f5e8-123">Accept</span></span>|<span data-ttu-id="6f5e8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6f5e8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f5e8-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6f5e8-125">Request body</span></span>
<span data-ttu-id="6f5e8-126">В теле запроса добавьте представление объекта [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6f5e8-126">In the request body, supply a JSON representation for the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="6f5e8-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f5e8-127">The following table shows the properties that are required when you create the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="6f5e8-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f5e8-128">Property</span></span>|<span data-ttu-id="6f5e8-129">Тип</span><span class="sxs-lookup"><span data-stu-id="6f5e8-129">Type</span></span>|<span data-ttu-id="6f5e8-130">Описание</span><span class="sxs-lookup"><span data-stu-id="6f5e8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f5e8-131">id</span><span class="sxs-lookup"><span data-stu-id="6f5e8-131">id</span></span>|<span data-ttu-id="6f5e8-132">String</span><span class="sxs-lookup"><span data-stu-id="6f5e8-132">String</span></span>|<span data-ttu-id="6f5e8-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6f5e8-133">Key of the entity.</span></span> <span data-ttu-id="6f5e8-134">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f5e8-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f5e8-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6f5e8-135">lastModifiedDateTime</span></span>|<span data-ttu-id="6f5e8-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f5e8-136">DateTimeOffset</span></span>|<span data-ttu-id="6f5e8-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="6f5e8-137">DateTime the object was last modified.</span></span> <span data-ttu-id="6f5e8-138">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f5e8-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f5e8-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6f5e8-139">createdDateTime</span></span>|<span data-ttu-id="6f5e8-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f5e8-140">DateTimeOffset</span></span>|<span data-ttu-id="6f5e8-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="6f5e8-141">DateTime the object was created.</span></span> <span data-ttu-id="6f5e8-142">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f5e8-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f5e8-143">описание</span><span class="sxs-lookup"><span data-stu-id="6f5e8-143">description</span></span>|<span data-ttu-id="6f5e8-144">String</span><span class="sxs-lookup"><span data-stu-id="6f5e8-144">String</span></span>|<span data-ttu-id="6f5e8-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6f5e8-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6f5e8-146">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f5e8-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f5e8-147">displayName</span><span class="sxs-lookup"><span data-stu-id="6f5e8-147">displayName</span></span>|<span data-ttu-id="6f5e8-148">String</span><span class="sxs-lookup"><span data-stu-id="6f5e8-148">String</span></span>|<span data-ttu-id="6f5e8-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6f5e8-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6f5e8-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f5e8-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f5e8-151">version</span><span class="sxs-lookup"><span data-stu-id="6f5e8-151">version</span></span>|<span data-ttu-id="6f5e8-152">Int32</span><span class="sxs-lookup"><span data-stu-id="6f5e8-152">Int32</span></span>|<span data-ttu-id="6f5e8-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6f5e8-153">Version of the device configuration.</span></span> <span data-ttu-id="6f5e8-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f5e8-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f5e8-155">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="6f5e8-155">compliantAppsList</span></span>|<span data-ttu-id="6f5e8-156">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="6f5e8-156">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="6f5e8-157">Список приложений (разрешенных или заблокированных в зависимости от значения свойства CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="6f5e8-157">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="6f5e8-158">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="6f5e8-158">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="6f5e8-159">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="6f5e8-159">compliantAppListType</span></span>|[<span data-ttu-id="6f5e8-160">appListType</span><span class="sxs-lookup"><span data-stu-id="6f5e8-160">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="6f5e8-161">Список, включенный в CompliantAppsList.</span><span class="sxs-lookup"><span data-stu-id="6f5e8-161">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="6f5e8-162">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="6f5e8-162">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="6f5e8-163">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="6f5e8-163">emailInDomainSuffixes</span></span>|<span data-ttu-id="6f5e8-164">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6f5e8-164">String collection</span></span>|<span data-ttu-id="6f5e8-165">Электронный адрес без суффикса, соответствующего одной из этих строк, будет считаться не добавленным в домен.</span><span class="sxs-lookup"><span data-stu-id="6f5e8-165">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="6f5e8-166">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="6f5e8-166">passwordBlockSimple</span></span>|<span data-ttu-id="6f5e8-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f5e8-167">Boolean</span></span>|<span data-ttu-id="6f5e8-168">Блокировка простых паролей.</span><span class="sxs-lookup"><span data-stu-id="6f5e8-168">Block simple passwords.</span></span>|
|<span data-ttu-id="6f5e8-169">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="6f5e8-169">passwordExpirationDays</span></span>|<span data-ttu-id="6f5e8-170">Int32</span><span class="sxs-lookup"><span data-stu-id="6f5e8-170">Int32</span></span>|<span data-ttu-id="6f5e8-171">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="6f5e8-171">Number of days before the password expires.</span></span>|
|<span data-ttu-id="6f5e8-172">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="6f5e8-172">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="6f5e8-173">Int32</span><span class="sxs-lookup"><span data-stu-id="6f5e8-173">Int32</span></span>|<span data-ttu-id="6f5e8-174">Количество наборов символов, которые должен содержать пароль.</span><span class="sxs-lookup"><span data-stu-id="6f5e8-174">Number of character sets a password must contain.</span></span> <span data-ttu-id="6f5e8-175">Допустимые значения: от 0 до 4.</span><span class="sxs-lookup"><span data-stu-id="6f5e8-175">Valid values 0 to 4</span></span>|
|<span data-ttu-id="6f5e8-176">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="6f5e8-176">passwordMinimumLength</span></span>|<span data-ttu-id="6f5e8-177">Int32</span><span class="sxs-lookup"><span data-stu-id="6f5e8-177">Int32</span></span>|<span data-ttu-id="6f5e8-178">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="6f5e8-178">Minimum length of passwords.</span></span>|
|<span data-ttu-id="6f5e8-179">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="6f5e8-179">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="6f5e8-180">Int32</span><span class="sxs-lookup"><span data-stu-id="6f5e8-180">Int32</span></span>|<span data-ttu-id="6f5e8-181">Период бездействия (в минутах), по истечении которого будет запрашиваться пароль.</span><span class="sxs-lookup"><span data-stu-id="6f5e8-181">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="6f5e8-182">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="6f5e8-182">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="6f5e8-183">Int32</span><span class="sxs-lookup"><span data-stu-id="6f5e8-183">Int32</span></span>|<span data-ttu-id="6f5e8-184">Период бездействия (в минутах), по истечении которого гаснет экран.</span><span class="sxs-lookup"><span data-stu-id="6f5e8-184">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="6f5e8-185">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="6f5e8-185">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="6f5e8-186">Int32</span><span class="sxs-lookup"><span data-stu-id="6f5e8-186">Int32</span></span>|<span data-ttu-id="6f5e8-187">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="6f5e8-187">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="6f5e8-188">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="6f5e8-188">passwordRequiredType</span></span>|[<span data-ttu-id="6f5e8-189">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="6f5e8-189">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="6f5e8-190">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="6f5e8-190">Type of password that is required.</span></span> <span data-ttu-id="6f5e8-191">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="6f5e8-191">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="6f5e8-192">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="6f5e8-192">passwordRequired</span></span>|<span data-ttu-id="6f5e8-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f5e8-193">Boolean</span></span>|<span data-ttu-id="6f5e8-194">Указывает, обязательно ли использовать пароль.</span><span class="sxs-lookup"><span data-stu-id="6f5e8-194">Whether or not to require a password.</span></span>|



## <a name="response"></a><span data-ttu-id="6f5e8-195">Ответ</span><span class="sxs-lookup"><span data-stu-id="6f5e8-195">Response</span></span>
<span data-ttu-id="6f5e8-196">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6f5e8-196">If successful, this method returns a `200 OK` response code and an updated [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f5e8-197">Пример</span><span class="sxs-lookup"><span data-stu-id="6f5e8-197">Example</span></span>
### <a name="request"></a><span data-ttu-id="6f5e8-198">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f5e8-198">Request</span></span>
<span data-ttu-id="6f5e8-199">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f5e8-199">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="6f5e8-200">Ответ</span><span class="sxs-lookup"><span data-stu-id="6f5e8-200">Response</span></span>
<span data-ttu-id="6f5e8-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="6f5e8-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



