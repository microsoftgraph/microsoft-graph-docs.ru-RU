---
title: Создание объекта windowsPhone81GeneralConfiguration
description: Создает объект windowsPhone81GeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dfda055c4b2c525617d7a97aa9ae73edc5195770
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32519985"
---
# <a name="create-windowsphone81generalconfiguration"></a><span data-ttu-id="05b3b-103">Создание объекта windowsPhone81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="05b3b-103">Create windowsPhone81GeneralConfiguration</span></span>

> <span data-ttu-id="05b3b-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="05b3b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05b3b-105">Создает объект [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="05b3b-105">Create a new [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="05b3b-106">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="05b3b-106">Prerequisites</span></span>
<span data-ttu-id="05b3b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05b3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05b3b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="05b3b-109">Permission type</span></span>|<span data-ttu-id="05b3b-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="05b3b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05b3b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="05b3b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="05b3b-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05b3b-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="05b3b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="05b3b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05b3b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05b3b-114">Not supported.</span></span>|
|<span data-ttu-id="05b3b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="05b3b-115">Application</span></span>|<span data-ttu-id="05b3b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05b3b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="05b3b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="05b3b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="05b3b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="05b3b-118">Request headers</span></span>
|<span data-ttu-id="05b3b-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="05b3b-119">Header</span></span>|<span data-ttu-id="05b3b-120">Значение</span><span class="sxs-lookup"><span data-stu-id="05b3b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05b3b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="05b3b-121">Authorization</span></span>|<span data-ttu-id="05b3b-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="05b3b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05b3b-123">Accept</span><span class="sxs-lookup"><span data-stu-id="05b3b-123">Accept</span></span>|<span data-ttu-id="05b3b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="05b3b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05b3b-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="05b3b-125">Request body</span></span>
<span data-ttu-id="05b3b-126">В теле запроса добавьте представление объекта windowsPhone81GeneralConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="05b3b-126">In the request body, supply a JSON representation for the windowsPhone81GeneralConfiguration object.</span></span>

<span data-ttu-id="05b3b-127">Ниже показаны свойства, которые необходимо указывать при создании объекта windowsPhone81GeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="05b3b-127">The following table shows the properties that are required when you create the windowsPhone81GeneralConfiguration.</span></span>

|<span data-ttu-id="05b3b-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="05b3b-128">Property</span></span>|<span data-ttu-id="05b3b-129">Тип</span><span class="sxs-lookup"><span data-stu-id="05b3b-129">Type</span></span>|<span data-ttu-id="05b3b-130">Описание</span><span class="sxs-lookup"><span data-stu-id="05b3b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05b3b-131">id</span><span class="sxs-lookup"><span data-stu-id="05b3b-131">id</span></span>|<span data-ttu-id="05b3b-132">Строка</span><span class="sxs-lookup"><span data-stu-id="05b3b-132">String</span></span>|<span data-ttu-id="05b3b-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="05b3b-133">Key of the entity.</span></span> <span data-ttu-id="05b3b-134">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="05b3b-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05b3b-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="05b3b-135">lastModifiedDateTime</span></span>|<span data-ttu-id="05b3b-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05b3b-136">DateTimeOffset</span></span>|<span data-ttu-id="05b3b-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="05b3b-137">DateTime the object was last modified.</span></span> <span data-ttu-id="05b3b-138">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="05b3b-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05b3b-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="05b3b-139">createdDateTime</span></span>|<span data-ttu-id="05b3b-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05b3b-140">DateTimeOffset</span></span>|<span data-ttu-id="05b3b-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="05b3b-141">DateTime the object was created.</span></span> <span data-ttu-id="05b3b-142">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="05b3b-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05b3b-143">description</span><span class="sxs-lookup"><span data-stu-id="05b3b-143">description</span></span>|<span data-ttu-id="05b3b-144">String</span><span class="sxs-lookup"><span data-stu-id="05b3b-144">String</span></span>|<span data-ttu-id="05b3b-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="05b3b-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="05b3b-146">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="05b3b-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05b3b-147">displayName</span><span class="sxs-lookup"><span data-stu-id="05b3b-147">displayName</span></span>|<span data-ttu-id="05b3b-148">String</span><span class="sxs-lookup"><span data-stu-id="05b3b-148">String</span></span>|<span data-ttu-id="05b3b-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="05b3b-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="05b3b-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="05b3b-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05b3b-151">version</span><span class="sxs-lookup"><span data-stu-id="05b3b-151">version</span></span>|<span data-ttu-id="05b3b-152">Int32</span><span class="sxs-lookup"><span data-stu-id="05b3b-152">Int32</span></span>|<span data-ttu-id="05b3b-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="05b3b-153">Version of the device configuration.</span></span> <span data-ttu-id="05b3b-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="05b3b-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05b3b-155">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="05b3b-155">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="05b3b-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="05b3b-156">Boolean</span></span>|<span data-ttu-id="05b3b-157">Указывает, применяется ли эта политика только к Windows Phone 8.1.</span><span class="sxs-lookup"><span data-stu-id="05b3b-157">Value indicating whether this policy only applies to Windows Phone 8.1.</span></span> <span data-ttu-id="05b3b-158">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="05b3b-158">This property is read-only.</span></span>|
|<span data-ttu-id="05b3b-159">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="05b3b-159">appsBlockCopyPaste</span></span>|<span data-ttu-id="05b3b-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="05b3b-160">Boolean</span></span>|<span data-ttu-id="05b3b-161">Указывает, следует ли заблокировать копирование данных.</span><span class="sxs-lookup"><span data-stu-id="05b3b-161">Indicates whether or not to block copy paste.</span></span>|
|<span data-ttu-id="05b3b-162">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="05b3b-162">bluetoothBlocked</span></span>|<span data-ttu-id="05b3b-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="05b3b-163">Boolean</span></span>|<span data-ttu-id="05b3b-164">Указывает, следует ли заблокировать Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="05b3b-164">Indicates whether or not to block bluetooth.</span></span>|
|<span data-ttu-id="05b3b-165">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="05b3b-165">cameraBlocked</span></span>|<span data-ttu-id="05b3b-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="05b3b-166">Boolean</span></span>|<span data-ttu-id="05b3b-167">Указывает, следует ли заблокировать камеру.</span><span class="sxs-lookup"><span data-stu-id="05b3b-167">Indicates whether or not to block camera.</span></span>|
|<span data-ttu-id="05b3b-168">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="05b3b-168">cellularBlockWifiTethering</span></span>|<span data-ttu-id="05b3b-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="05b3b-169">Boolean</span></span>|<span data-ttu-id="05b3b-170">Указывает, следует ли заблокировать модем Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="05b3b-170">Indicates whether or not to block Wi-Fi tethering.</span></span> <span data-ttu-id="05b3b-171">Ни на что не влияет, если Wi-Fi заблокирован.</span><span class="sxs-lookup"><span data-stu-id="05b3b-171">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="05b3b-172">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="05b3b-172">compliantAppsList</span></span>|<span data-ttu-id="05b3b-173">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="05b3b-173">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="05b3b-174">Список приложений, соответствующих требованиям (список разрешений или блокировок, определяется свойством CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="05b3b-174">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="05b3b-175">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="05b3b-175">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="05b3b-176">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="05b3b-176">compliantAppListType</span></span>|[<span data-ttu-id="05b3b-177">Апплисттипе</span><span class="sxs-lookup"><span data-stu-id="05b3b-177">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="05b3b-178">Список, указанный с помощью свойства AppComplianceList.</span><span class="sxs-lookup"><span data-stu-id="05b3b-178">List that is in the AppComplianceList.</span></span> <span data-ttu-id="05b3b-179">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="05b3b-179">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="05b3b-180">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="05b3b-180">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="05b3b-181">Логический</span><span class="sxs-lookup"><span data-stu-id="05b3b-181">Boolean</span></span>|<span data-ttu-id="05b3b-182">Указывает, следует ли заблокировать отправку диагностических данных.</span><span class="sxs-lookup"><span data-stu-id="05b3b-182">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="05b3b-183">emailBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="05b3b-183">emailBlockAddingAccounts</span></span>|<span data-ttu-id="05b3b-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="05b3b-184">Boolean</span></span>|<span data-ttu-id="05b3b-185">Указывает, следует ли заблокировать пользовательские учетные записи электронной почты.</span><span class="sxs-lookup"><span data-stu-id="05b3b-185">Indicates whether or not to block custom email accounts.</span></span>|
|<span data-ttu-id="05b3b-186">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="05b3b-186">locationServicesBlocked</span></span>|<span data-ttu-id="05b3b-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="05b3b-187">Boolean</span></span>|<span data-ttu-id="05b3b-188">Указывает, следует ли заблокировать службы определения местоположения.</span><span class="sxs-lookup"><span data-stu-id="05b3b-188">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="05b3b-189">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="05b3b-189">microsoftAccountBlocked</span></span>|<span data-ttu-id="05b3b-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="05b3b-190">Boolean</span></span>|<span data-ttu-id="05b3b-191">Указывает, следует ли запретить использовать учетную запись Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="05b3b-191">Indicates whether or not to block using a Microsoft Account.</span></span>|
|<span data-ttu-id="05b3b-192">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="05b3b-192">nfcBlocked</span></span>|<span data-ttu-id="05b3b-193">Логический</span><span class="sxs-lookup"><span data-stu-id="05b3b-193">Boolean</span></span>|<span data-ttu-id="05b3b-194">Указывает, следует ли заблокировать NFC.</span><span class="sxs-lookup"><span data-stu-id="05b3b-194">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="05b3b-195">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="05b3b-195">passwordBlockSimple</span></span>|<span data-ttu-id="05b3b-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="05b3b-196">Boolean</span></span>|<span data-ttu-id="05b3b-197">Указывает, следует ли заблокировать синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="05b3b-197">Indicates whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="05b3b-198">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="05b3b-198">passwordExpirationDays</span></span>|<span data-ttu-id="05b3b-199">Int32</span><span class="sxs-lookup"><span data-stu-id="05b3b-199">Int32</span></span>|<span data-ttu-id="05b3b-200">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="05b3b-200">Number of days before the password expires.</span></span>|
|<span data-ttu-id="05b3b-201">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="05b3b-201">passwordMinimumLength</span></span>|<span data-ttu-id="05b3b-202">Int32</span><span class="sxs-lookup"><span data-stu-id="05b3b-202">Int32</span></span>|<span data-ttu-id="05b3b-203">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="05b3b-203">Minimum length of passwords.</span></span>|
|<span data-ttu-id="05b3b-204">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="05b3b-204">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="05b3b-205">Int32</span><span class="sxs-lookup"><span data-stu-id="05b3b-205">Int32</span></span>|<span data-ttu-id="05b3b-206">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="05b3b-206">Minutes of inactivity before screen timeout.</span></span>|
|<span data-ttu-id="05b3b-207">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="05b3b-207">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="05b3b-208">Int32</span><span class="sxs-lookup"><span data-stu-id="05b3b-208">Int32</span></span>|<span data-ttu-id="05b3b-209">Количество наборов символов, которые должен содержать пароль.</span><span class="sxs-lookup"><span data-stu-id="05b3b-209">Number of character sets a password must contain.</span></span>|
|<span data-ttu-id="05b3b-210">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="05b3b-210">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="05b3b-211">Int32</span><span class="sxs-lookup"><span data-stu-id="05b3b-211">Int32</span></span>|<span data-ttu-id="05b3b-212">Количество предыдущих паролей, которые следует заблокировать.</span><span class="sxs-lookup"><span data-stu-id="05b3b-212">Number of previous passwords to block.</span></span> <span data-ttu-id="05b3b-213">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="05b3b-213">Valid values 0 to 24</span></span>|
|<span data-ttu-id="05b3b-214">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="05b3b-214">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="05b3b-215">Int32</span><span class="sxs-lookup"><span data-stu-id="05b3b-215">Int32</span></span>|<span data-ttu-id="05b3b-216">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="05b3b-216">Number of sign in failures allowed before factory reset.</span></span>|
|<span data-ttu-id="05b3b-217">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="05b3b-217">passwordRequiredType</span></span>|[<span data-ttu-id="05b3b-218">Рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="05b3b-218">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="05b3b-219">Необходимый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="05b3b-219">Password type that is required.</span></span> <span data-ttu-id="05b3b-220">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="05b3b-220">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="05b3b-221">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="05b3b-221">passwordRequired</span></span>|<span data-ttu-id="05b3b-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="05b3b-222">Boolean</span></span>|<span data-ttu-id="05b3b-223">Указывает, обязательно ли использовать пароль.</span><span class="sxs-lookup"><span data-stu-id="05b3b-223">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="05b3b-224">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="05b3b-224">screenCaptureBlocked</span></span>|<span data-ttu-id="05b3b-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="05b3b-225">Boolean</span></span>|<span data-ttu-id="05b3b-226">Указывает, следует ли запретить делать снимки экрана.</span><span class="sxs-lookup"><span data-stu-id="05b3b-226">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="05b3b-227">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="05b3b-227">storageBlockRemovableStorage</span></span>|<span data-ttu-id="05b3b-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="05b3b-228">Boolean</span></span>|<span data-ttu-id="05b3b-229">Указывает, следует ли запретить использовать съемные носители.</span><span class="sxs-lookup"><span data-stu-id="05b3b-229">Indicates whether or not to block removable storage.</span></span>|
|<span data-ttu-id="05b3b-230">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="05b3b-230">storageRequireEncryption</span></span>|<span data-ttu-id="05b3b-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="05b3b-231">Boolean</span></span>|<span data-ttu-id="05b3b-232">Указывает, обязательно ли шифрование.</span><span class="sxs-lookup"><span data-stu-id="05b3b-232">Indicates whether or not to require encryption.</span></span>|
|<span data-ttu-id="05b3b-233">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="05b3b-233">webBrowserBlocked</span></span>|<span data-ttu-id="05b3b-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="05b3b-234">Boolean</span></span>|<span data-ttu-id="05b3b-235">Указывает, следует ли заблокировать веб-браузер.</span><span class="sxs-lookup"><span data-stu-id="05b3b-235">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="05b3b-236">wifiBlocked</span><span class="sxs-lookup"><span data-stu-id="05b3b-236">wifiBlocked</span></span>|<span data-ttu-id="05b3b-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="05b3b-237">Boolean</span></span>|<span data-ttu-id="05b3b-238">Указывает, следует ли заблокировать Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="05b3b-238">Indicates whether or not to block Wi-Fi.</span></span>|
|<span data-ttu-id="05b3b-239">wifiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="05b3b-239">wifiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="05b3b-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="05b3b-240">Boolean</span></span>|<span data-ttu-id="05b3b-241">Указывает, следует ли заблокировать автоматическое подключение к хот-спотам Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="05b3b-241">Indicates whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="05b3b-242">Ни на что не влияет, если Wi-Fi заблокирован.</span><span class="sxs-lookup"><span data-stu-id="05b3b-242">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="05b3b-243">wifiBlockHotspotReporting</span><span class="sxs-lookup"><span data-stu-id="05b3b-243">wifiBlockHotspotReporting</span></span>|<span data-ttu-id="05b3b-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="05b3b-244">Boolean</span></span>|<span data-ttu-id="05b3b-245">Указывает, следует ли запретить устройству сообщать об обнаруженных хот-спотах Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="05b3b-245">Indicates whether or not to block Wi-Fi hotspot reporting.</span></span> <span data-ttu-id="05b3b-246">Ни на что не влияет, если Wi-Fi заблокирован.</span><span class="sxs-lookup"><span data-stu-id="05b3b-246">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="05b3b-247">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="05b3b-247">windowsStoreBlocked</span></span>|<span data-ttu-id="05b3b-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="05b3b-248">Boolean</span></span>|<span data-ttu-id="05b3b-249">Указывает, следует ли заблокировать Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="05b3b-249">Indicates whether or not to block the Windows Store.</span></span>|



## <a name="response"></a><span data-ttu-id="05b3b-250">Отклик</span><span class="sxs-lookup"><span data-stu-id="05b3b-250">Response</span></span>
<span data-ttu-id="05b3b-251">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="05b3b-251">If successful, this method returns a `201 Created` response code and a [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05b3b-252">Пример</span><span class="sxs-lookup"><span data-stu-id="05b3b-252">Example</span></span>

### <a name="request"></a><span data-ttu-id="05b3b-253">Запрос</span><span class="sxs-lookup"><span data-stu-id="05b3b-253">Request</span></span>
<span data-ttu-id="05b3b-254">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="05b3b-254">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1461

{
  "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "applyOnlyToWindowsPhone81": true,
  "appsBlockCopyPaste": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockWifiTethering": true,
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
  "diagnosticDataBlockSubmission": true,
  "emailBlockAddingAccounts": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "nfcBlocked": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireEncryption": true,
  "webBrowserBlocked": true,
  "wifiBlocked": true,
  "wifiBlockAutomaticConnectHotspots": true,
  "wifiBlockHotspotReporting": true,
  "windowsStoreBlocked": true
}
```

### <a name="response"></a><span data-ttu-id="05b3b-255">Отклик</span><span class="sxs-lookup"><span data-stu-id="05b3b-255">Response</span></span>
<span data-ttu-id="05b3b-p116">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="05b3b-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1633

{
  "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
  "id": "f5e0e34d-e34d-f5e0-4de3-e0f54de3e0f5",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "applyOnlyToWindowsPhone81": true,
  "appsBlockCopyPaste": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockWifiTethering": true,
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
  "diagnosticDataBlockSubmission": true,
  "emailBlockAddingAccounts": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "nfcBlocked": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireEncryption": true,
  "webBrowserBlocked": true,
  "wifiBlocked": true,
  "wifiBlockAutomaticConnectHotspots": true,
  "wifiBlockHotspotReporting": true,
  "windowsStoreBlocked": true
}
```



