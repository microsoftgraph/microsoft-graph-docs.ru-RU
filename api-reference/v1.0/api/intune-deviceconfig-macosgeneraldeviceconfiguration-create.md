---
title: Create macOSGeneralDeviceConfiguration
description: Создание объекта macOSGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8f36883aa25e9b285c2e0363a47a7aafc07dc5f1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851648"
---
# <a name="create-macosgeneraldeviceconfiguration"></a><span data-ttu-id="c8010-103">Create macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="c8010-103">Create macOSGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="c8010-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c8010-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c8010-105">Создание объекта [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c8010-105">Create a new [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c8010-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="c8010-106">Prerequisites</span></span>
<span data-ttu-id="c8010-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8010-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8010-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c8010-109">Permission type</span></span>|<span data-ttu-id="c8010-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c8010-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8010-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c8010-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c8010-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8010-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c8010-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c8010-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8010-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8010-114">Not supported.</span></span>|
|<span data-ttu-id="c8010-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c8010-115">Application</span></span>|<span data-ttu-id="c8010-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8010-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8010-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c8010-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c8010-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c8010-118">Request headers</span></span>
|<span data-ttu-id="c8010-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c8010-119">Header</span></span>|<span data-ttu-id="c8010-120">Значение</span><span class="sxs-lookup"><span data-stu-id="c8010-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8010-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8010-121">Authorization</span></span>|<span data-ttu-id="c8010-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c8010-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8010-123">Accept</span><span class="sxs-lookup"><span data-stu-id="c8010-123">Accept</span></span>|<span data-ttu-id="c8010-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c8010-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8010-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c8010-125">Request body</span></span>
<span data-ttu-id="c8010-126">В тексте запроса добавьте представление объекта macOSGeneralDeviceConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c8010-126">In the request body, supply a JSON representation for the macOSGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="c8010-127">В приведенной ниже таблице показаны, которые необходимо указывать при создании объекта macOSGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="c8010-127">The following table shows the properties that are required when you create the macOSGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="c8010-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="c8010-128">Property</span></span>|<span data-ttu-id="c8010-129">Тип</span><span class="sxs-lookup"><span data-stu-id="c8010-129">Type</span></span>|<span data-ttu-id="c8010-130">Описание</span><span class="sxs-lookup"><span data-stu-id="c8010-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8010-131">id</span><span class="sxs-lookup"><span data-stu-id="c8010-131">id</span></span>|<span data-ttu-id="c8010-132">Строка</span><span class="sxs-lookup"><span data-stu-id="c8010-132">String</span></span>|<span data-ttu-id="c8010-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c8010-133">Key of the entity.</span></span> <span data-ttu-id="c8010-134">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c8010-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8010-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c8010-135">lastModifiedDateTime</span></span>|<span data-ttu-id="c8010-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8010-136">DateTimeOffset</span></span>|<span data-ttu-id="c8010-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c8010-137">DateTime the object was last modified.</span></span> <span data-ttu-id="c8010-138">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c8010-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8010-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c8010-139">createdDateTime</span></span>|<span data-ttu-id="c8010-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8010-140">DateTimeOffset</span></span>|<span data-ttu-id="c8010-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c8010-141">DateTime the object was created.</span></span> <span data-ttu-id="c8010-142">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c8010-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8010-143">описание</span><span class="sxs-lookup"><span data-stu-id="c8010-143">description</span></span>|<span data-ttu-id="c8010-144">Строка</span><span class="sxs-lookup"><span data-stu-id="c8010-144">String</span></span>|<span data-ttu-id="c8010-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c8010-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c8010-146">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c8010-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8010-147">displayName</span><span class="sxs-lookup"><span data-stu-id="c8010-147">displayName</span></span>|<span data-ttu-id="c8010-148">Строка</span><span class="sxs-lookup"><span data-stu-id="c8010-148">String</span></span>|<span data-ttu-id="c8010-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c8010-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c8010-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c8010-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8010-151">version</span><span class="sxs-lookup"><span data-stu-id="c8010-151">version</span></span>|<span data-ttu-id="c8010-152">Int32</span><span class="sxs-lookup"><span data-stu-id="c8010-152">Int32</span></span>|<span data-ttu-id="c8010-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c8010-153">Version of the device configuration.</span></span> <span data-ttu-id="c8010-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c8010-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8010-155">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="c8010-155">compliantAppsList</span></span>|<span data-ttu-id="c8010-156">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="c8010-156">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="c8010-157">Список приложений (разрешенных или заблокированных в зависимости от значения свойства CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="c8010-157">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="c8010-158">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="c8010-158">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="c8010-159">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="c8010-159">compliantAppListType</span></span>|[<span data-ttu-id="c8010-160">appListType</span><span class="sxs-lookup"><span data-stu-id="c8010-160">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="c8010-161">Список, включенный в CompliantAppsList.</span><span class="sxs-lookup"><span data-stu-id="c8010-161">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="c8010-162">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="c8010-162">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="c8010-163">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="c8010-163">emailInDomainSuffixes</span></span>|<span data-ttu-id="c8010-164">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c8010-164">String collection</span></span>|<span data-ttu-id="c8010-165">Электронный адрес без суффикса, соответствующего одной из этих строк, будет считаться не добавленным в домен.</span><span class="sxs-lookup"><span data-stu-id="c8010-165">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="c8010-166">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="c8010-166">passwordBlockSimple</span></span>|<span data-ttu-id="c8010-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="c8010-167">Boolean</span></span>|<span data-ttu-id="c8010-168">Блокировка простых паролей.</span><span class="sxs-lookup"><span data-stu-id="c8010-168">Block simple passwords.</span></span>|
|<span data-ttu-id="c8010-169">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="c8010-169">passwordExpirationDays</span></span>|<span data-ttu-id="c8010-170">Int32</span><span class="sxs-lookup"><span data-stu-id="c8010-170">Int32</span></span>|<span data-ttu-id="c8010-171">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="c8010-171">Number of days before the password expires.</span></span>|
|<span data-ttu-id="c8010-172">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="c8010-172">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="c8010-173">Int32</span><span class="sxs-lookup"><span data-stu-id="c8010-173">Int32</span></span>|<span data-ttu-id="c8010-174">Количество наборов символов, которые должен содержать пароль.</span><span class="sxs-lookup"><span data-stu-id="c8010-174">Number of character sets a password must contain.</span></span> <span data-ttu-id="c8010-175">Допустимые значения: от 0 до 4.</span><span class="sxs-lookup"><span data-stu-id="c8010-175">Valid values 0 to 4</span></span>|
|<span data-ttu-id="c8010-176">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="c8010-176">passwordMinimumLength</span></span>|<span data-ttu-id="c8010-177">Int32</span><span class="sxs-lookup"><span data-stu-id="c8010-177">Int32</span></span>|<span data-ttu-id="c8010-178">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="c8010-178">Minimum length of passwords.</span></span>|
|<span data-ttu-id="c8010-179">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="c8010-179">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="c8010-180">Int32</span><span class="sxs-lookup"><span data-stu-id="c8010-180">Int32</span></span>|<span data-ttu-id="c8010-181">Период бездействия (в минутах), по истечении которого будет запрашиваться пароль.</span><span class="sxs-lookup"><span data-stu-id="c8010-181">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="c8010-182">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="c8010-182">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="c8010-183">Int32</span><span class="sxs-lookup"><span data-stu-id="c8010-183">Int32</span></span>|<span data-ttu-id="c8010-184">Период бездействия (в минутах), по истечении которого гаснет экран.</span><span class="sxs-lookup"><span data-stu-id="c8010-184">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="c8010-185">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="c8010-185">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="c8010-186">Int32</span><span class="sxs-lookup"><span data-stu-id="c8010-186">Int32</span></span>|<span data-ttu-id="c8010-187">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="c8010-187">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="c8010-188">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="c8010-188">passwordRequiredType</span></span>|[<span data-ttu-id="c8010-189">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="c8010-189">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="c8010-190">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="c8010-190">Type of password that is required.</span></span> <span data-ttu-id="c8010-191">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="c8010-191">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="c8010-192">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="c8010-192">passwordRequired</span></span>|<span data-ttu-id="c8010-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="c8010-193">Boolean</span></span>|<span data-ttu-id="c8010-194">Указывает, обязательно ли использовать пароль.</span><span class="sxs-lookup"><span data-stu-id="c8010-194">Whether or not to require a password.</span></span>|



## <a name="response"></a><span data-ttu-id="c8010-195">Ответ</span><span class="sxs-lookup"><span data-stu-id="c8010-195">Response</span></span>
<span data-ttu-id="c8010-196">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c8010-196">If successful, this method returns a `201 Created` response code and a [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8010-197">Пример</span><span class="sxs-lookup"><span data-stu-id="c8010-197">Example</span></span>
### <a name="request"></a><span data-ttu-id="c8010-198">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8010-198">Request</span></span>
<span data-ttu-id="c8010-199">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c8010-199">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c8010-200">Ответ</span><span class="sxs-lookup"><span data-stu-id="c8010-200">Response</span></span>
<span data-ttu-id="c8010-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c8010-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



