---
title: Создание Андроиддевицеовнеркомплианцеполици
description: Создание нового объекта Андроиддевицеовнеркомплианцеполици.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5f36a9aaf47bb29f60c09616dd4235f45fcbbfcf
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33933692"
---
# <a name="create-androiddeviceownercompliancepolicy"></a><span data-ttu-id="3f98c-103">Создание Андроиддевицеовнеркомплианцеполици</span><span class="sxs-lookup"><span data-stu-id="3f98c-103">Create androidDeviceOwnerCompliancePolicy</span></span>

> <span data-ttu-id="3f98c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f98c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f98c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3f98c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f98c-106">Создание нового объекта [андроиддевицеовнеркомплианцеполици](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="3f98c-106">Create a new [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3f98c-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3f98c-107">Prerequisites</span></span>
<span data-ttu-id="3f98c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f98c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f98c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3f98c-110">Permission type</span></span>|<span data-ttu-id="3f98c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3f98c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3f98c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3f98c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3f98c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f98c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3f98c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3f98c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3f98c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f98c-115">Not supported.</span></span>|
|<span data-ttu-id="3f98c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3f98c-116">Application</span></span>|<span data-ttu-id="3f98c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f98c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3f98c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3f98c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="3f98c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3f98c-119">Request headers</span></span>
|<span data-ttu-id="3f98c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3f98c-120">Header</span></span>|<span data-ttu-id="3f98c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="3f98c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3f98c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3f98c-122">Authorization</span></span>|<span data-ttu-id="3f98c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3f98c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3f98c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="3f98c-124">Accept</span></span>|<span data-ttu-id="3f98c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3f98c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f98c-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3f98c-126">Request body</span></span>
<span data-ttu-id="3f98c-127">В тексте запроса добавьте представление объекта Андроиддевицеовнеркомплианцеполици в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3f98c-127">In the request body, supply a JSON representation for the androidDeviceOwnerCompliancePolicy object.</span></span>

<span data-ttu-id="3f98c-128">В следующей таблице приведены свойства, необходимые при создании Андроиддевицеовнеркомплианцеполици.</span><span class="sxs-lookup"><span data-stu-id="3f98c-128">The following table shows the properties that are required when you create the androidDeviceOwnerCompliancePolicy.</span></span>

|<span data-ttu-id="3f98c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="3f98c-129">Property</span></span>|<span data-ttu-id="3f98c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="3f98c-130">Type</span></span>|<span data-ttu-id="3f98c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="3f98c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f98c-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3f98c-132">roleScopeTagIds</span></span>|<span data-ttu-id="3f98c-133">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="3f98c-133">String collection</span></span>|<span data-ttu-id="3f98c-134">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="3f98c-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3f98c-135">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3f98c-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3f98c-136">id</span><span class="sxs-lookup"><span data-stu-id="3f98c-136">id</span></span>|<span data-ttu-id="3f98c-137">Строка</span><span class="sxs-lookup"><span data-stu-id="3f98c-137">String</span></span>|<span data-ttu-id="3f98c-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3f98c-138">Key of the entity.</span></span> <span data-ttu-id="3f98c-139">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3f98c-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3f98c-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3f98c-140">createdDateTime</span></span>|<span data-ttu-id="3f98c-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f98c-141">DateTimeOffset</span></span>|<span data-ttu-id="3f98c-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="3f98c-142">DateTime the object was created.</span></span> <span data-ttu-id="3f98c-143">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3f98c-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3f98c-144">description</span><span class="sxs-lookup"><span data-stu-id="3f98c-144">description</span></span>|<span data-ttu-id="3f98c-145">String</span><span class="sxs-lookup"><span data-stu-id="3f98c-145">String</span></span>|<span data-ttu-id="3f98c-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3f98c-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3f98c-147">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3f98c-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3f98c-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3f98c-148">lastModifiedDateTime</span></span>|<span data-ttu-id="3f98c-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f98c-149">DateTimeOffset</span></span>|<span data-ttu-id="3f98c-150">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="3f98c-150">DateTime the object was last modified.</span></span> <span data-ttu-id="3f98c-151">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3f98c-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3f98c-152">displayName</span><span class="sxs-lookup"><span data-stu-id="3f98c-152">displayName</span></span>|<span data-ttu-id="3f98c-153">Строка</span><span class="sxs-lookup"><span data-stu-id="3f98c-153">String</span></span>|<span data-ttu-id="3f98c-154">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3f98c-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3f98c-155">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3f98c-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3f98c-156">version</span><span class="sxs-lookup"><span data-stu-id="3f98c-156">version</span></span>|<span data-ttu-id="3f98c-157">Int32</span><span class="sxs-lookup"><span data-stu-id="3f98c-157">Int32</span></span>|<span data-ttu-id="3f98c-158">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3f98c-158">Version of the device configuration.</span></span> <span data-ttu-id="3f98c-159">Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3f98c-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3f98c-160">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="3f98c-160">osMinimumVersion</span></span>|<span data-ttu-id="3f98c-161">Строка</span><span class="sxs-lookup"><span data-stu-id="3f98c-161">String</span></span>|<span data-ttu-id="3f98c-162">Минимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="3f98c-162">Minimum Android version.</span></span>|
|<span data-ttu-id="3f98c-163">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="3f98c-163">osMaximumVersion</span></span>|<span data-ttu-id="3f98c-164">Строка</span><span class="sxs-lookup"><span data-stu-id="3f98c-164">String</span></span>|<span data-ttu-id="3f98c-165">Максимальная версия Android.</span><span class="sxs-lookup"><span data-stu-id="3f98c-165">Maximum Android version.</span></span>|
|<span data-ttu-id="3f98c-166">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="3f98c-166">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="3f98c-167">String</span><span class="sxs-lookup"><span data-stu-id="3f98c-167">String</span></span>|<span data-ttu-id="3f98c-168">Минимальный уровень обновления для системы безопасности Android.</span><span class="sxs-lookup"><span data-stu-id="3f98c-168">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="3f98c-169">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="3f98c-169">passwordRequired</span></span>|<span data-ttu-id="3f98c-170">Логический</span><span class="sxs-lookup"><span data-stu-id="3f98c-170">Boolean</span></span>|<span data-ttu-id="3f98c-171">Указывает, что для разблокировки устройства требуется указывать пароль.</span><span class="sxs-lookup"><span data-stu-id="3f98c-171">Require a password to unlock device.</span></span>|
|<span data-ttu-id="3f98c-172">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="3f98c-172">passwordMinimumLength</span></span>|<span data-ttu-id="3f98c-173">Int32</span><span class="sxs-lookup"><span data-stu-id="3f98c-173">Int32</span></span>|<span data-ttu-id="3f98c-174">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="3f98c-174">Minimum password length.</span></span> <span data-ttu-id="3f98c-175">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="3f98c-175">Valid values 4 to 16</span></span>|
|<span data-ttu-id="3f98c-176">Пассвордминимумлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="3f98c-176">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="3f98c-177">Int32</span><span class="sxs-lookup"><span data-stu-id="3f98c-177">Int32</span></span>|<span data-ttu-id="3f98c-178">Указывает минимальное число символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="3f98c-178">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="3f98c-179">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="3f98c-179">Valid values 1 to 16</span></span>|
|<span data-ttu-id="3f98c-180">Пассвордминимумловеркасечарактерс</span><span class="sxs-lookup"><span data-stu-id="3f98c-180">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="3f98c-181">Int32</span><span class="sxs-lookup"><span data-stu-id="3f98c-181">Int32</span></span>|<span data-ttu-id="3f98c-182">Указывает минимальное число символов нижнего регистра, необходимое для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="3f98c-182">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="3f98c-183">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="3f98c-183">Valid values 1 to 16</span></span>|
|<span data-ttu-id="3f98c-184">Пассвордминимумнонлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="3f98c-184">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="3f98c-185">Int32</span><span class="sxs-lookup"><span data-stu-id="3f98c-185">Int32</span></span>|<span data-ttu-id="3f98c-186">Указывает минимальное количество небуквенных символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="3f98c-186">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="3f98c-187">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="3f98c-187">Valid values 1 to 16</span></span>|
|<span data-ttu-id="3f98c-188">Пассвордминимумнумерикчарактерс</span><span class="sxs-lookup"><span data-stu-id="3f98c-188">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="3f98c-189">Int32</span><span class="sxs-lookup"><span data-stu-id="3f98c-189">Int32</span></span>|<span data-ttu-id="3f98c-190">Указывает минимальное количество числовых символов, необходимое для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="3f98c-190">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="3f98c-191">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="3f98c-191">Valid values 1 to 16</span></span>|
|<span data-ttu-id="3f98c-192">Пассвордминимумсимболчарактерс</span><span class="sxs-lookup"><span data-stu-id="3f98c-192">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="3f98c-193">Int32</span><span class="sxs-lookup"><span data-stu-id="3f98c-193">Int32</span></span>|<span data-ttu-id="3f98c-194">Указывает минимальное число символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="3f98c-194">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="3f98c-195">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="3f98c-195">Valid values 1 to 16</span></span>|
|<span data-ttu-id="3f98c-196">Пассвордминимумупперкасечарактерс</span><span class="sxs-lookup"><span data-stu-id="3f98c-196">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="3f98c-197">Int32</span><span class="sxs-lookup"><span data-stu-id="3f98c-197">Int32</span></span>|<span data-ttu-id="3f98c-198">Указывает минимальное количество символов в верхнем регистре, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="3f98c-198">Indicates the minimum number of upper case letter characters required for device password.</span></span> <span data-ttu-id="3f98c-199">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="3f98c-199">Valid values 1 to 16</span></span>|
|<span data-ttu-id="3f98c-200">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="3f98c-200">passwordRequiredType</span></span>|[<span data-ttu-id="3f98c-201">Андроиддевицеовнеррекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="3f98c-201">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="3f98c-202">Тип символов в пароле.</span><span class="sxs-lookup"><span data-stu-id="3f98c-202">Type of characters in password.</span></span> <span data-ttu-id="3f98c-203">Возможные значения: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.</span><span class="sxs-lookup"><span data-stu-id="3f98c-203">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.</span></span>|
|<span data-ttu-id="3f98c-204">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="3f98c-204">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="3f98c-205">Int32</span><span class="sxs-lookup"><span data-stu-id="3f98c-205">Int32</span></span>|<span data-ttu-id="3f98c-206">Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="3f98c-206">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="3f98c-207">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="3f98c-207">passwordExpirationDays</span></span>|<span data-ttu-id="3f98c-208">Int32</span><span class="sxs-lookup"><span data-stu-id="3f98c-208">Int32</span></span>|<span data-ttu-id="3f98c-209">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="3f98c-209">Number of days before the password expires.</span></span> <span data-ttu-id="3f98c-210">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="3f98c-210">Valid values 1 to 365</span></span>|
|<span data-ttu-id="3f98c-211">Пассвордпревиауспассвордкаунттоблокк</span><span class="sxs-lookup"><span data-stu-id="3f98c-211">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="3f98c-212">Int32</span><span class="sxs-lookup"><span data-stu-id="3f98c-212">Int32</span></span>|<span data-ttu-id="3f98c-213">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="3f98c-213">Number of previous passwords to block.</span></span> <span data-ttu-id="3f98c-214">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="3f98c-214">Valid values 1 to 24</span></span>|
|<span data-ttu-id="3f98c-215">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="3f98c-215">storageRequireEncryption</span></span>|<span data-ttu-id="3f98c-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f98c-216">Boolean</span></span>|<span data-ttu-id="3f98c-217">Указывает, что шифрование на устройствах с Android должно быть обязательным.</span><span class="sxs-lookup"><span data-stu-id="3f98c-217">Require encryption on Android devices.</span></span>|



## <a name="response"></a><span data-ttu-id="3f98c-218">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f98c-218">Response</span></span>
<span data-ttu-id="3f98c-219">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроиддевицеовнеркомплианцеполици](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3f98c-219">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f98c-220">Пример</span><span class="sxs-lookup"><span data-stu-id="3f98c-220">Example</span></span>

### <a name="request"></a><span data-ttu-id="3f98c-221">Запрос</span><span class="sxs-lookup"><span data-stu-id="3f98c-221">Request</span></span>
<span data-ttu-id="3f98c-222">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3f98c-222">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 932

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordMinimumLetterCharacters": 15,
  "passwordMinimumLowerCaseCharacters": 2,
  "passwordMinimumNonLetterCharacters": 2,
  "passwordMinimumNumericCharacters": 0,
  "passwordMinimumSymbolCharacters": 15,
  "passwordMinimumUpperCaseCharacters": 2,
  "passwordRequiredType": "required",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordCountToBlock": 4,
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="3f98c-223">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f98c-223">Response</span></span>
<span data-ttu-id="3f98c-p119">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3f98c-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1104

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "be2464b4-64b4-be24-b464-24beb46424be",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordMinimumLetterCharacters": 15,
  "passwordMinimumLowerCaseCharacters": 2,
  "passwordMinimumNonLetterCharacters": 2,
  "passwordMinimumNumericCharacters": 0,
  "passwordMinimumSymbolCharacters": 15,
  "passwordMinimumUpperCaseCharacters": 2,
  "passwordRequiredType": "required",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordCountToBlock": 4,
  "storageRequireEncryption": true
}
```




