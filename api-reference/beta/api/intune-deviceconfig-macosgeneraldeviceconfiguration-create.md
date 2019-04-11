---
title: Create macOSGeneralDeviceConfiguration
description: Создание объекта macOSGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3c2705b947e97597b38ef2d22441193cbafba01b
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31770734"
---
# <a name="create-macosgeneraldeviceconfiguration"></a><span data-ttu-id="c762f-103">Create macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="c762f-103">Create macOSGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="c762f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c762f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c762f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c762f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c762f-106">Создание объекта [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c762f-106">Create a new [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c762f-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="c762f-107">Prerequisites</span></span>
<span data-ttu-id="c762f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c762f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c762f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c762f-110">Permission type</span></span>|<span data-ttu-id="c762f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c762f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c762f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c762f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c762f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c762f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c762f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c762f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c762f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c762f-115">Not supported.</span></span>|
|<span data-ttu-id="c762f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c762f-116">Application</span></span>|<span data-ttu-id="c762f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c762f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c762f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c762f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c762f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c762f-119">Request headers</span></span>
|<span data-ttu-id="c762f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c762f-120">Header</span></span>|<span data-ttu-id="c762f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c762f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c762f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c762f-122">Authorization</span></span>|<span data-ttu-id="c762f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c762f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c762f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c762f-124">Accept</span></span>|<span data-ttu-id="c762f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c762f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c762f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c762f-126">Request body</span></span>
<span data-ttu-id="c762f-127">В тексте запроса добавьте представление объекта macOSGeneralDeviceConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c762f-127">In the request body, supply a JSON representation for the macOSGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="c762f-128">В приведенной ниже таблице показаны, которые необходимо указывать при создании объекта macOSGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="c762f-128">The following table shows the properties that are required when you create the macOSGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="c762f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c762f-129">Property</span></span>|<span data-ttu-id="c762f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c762f-130">Type</span></span>|<span data-ttu-id="c762f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c762f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c762f-132">id</span><span class="sxs-lookup"><span data-stu-id="c762f-132">id</span></span>|<span data-ttu-id="c762f-133">Строка</span><span class="sxs-lookup"><span data-stu-id="c762f-133">String</span></span>|<span data-ttu-id="c762f-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c762f-134">Key of the entity.</span></span> <span data-ttu-id="c762f-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c762f-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c762f-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c762f-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c762f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c762f-137">DateTimeOffset</span></span>|<span data-ttu-id="c762f-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c762f-138">DateTime the object was last modified.</span></span> <span data-ttu-id="c762f-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c762f-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c762f-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c762f-140">roleScopeTagIds</span></span>|<span data-ttu-id="c762f-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c762f-141">String collection</span></span>|<span data-ttu-id="c762f-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="c762f-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c762f-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c762f-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c762f-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="c762f-144">supportsScopeTags</span></span>|<span data-ttu-id="c762f-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="c762f-145">Boolean</span></span>|<span data-ttu-id="c762f-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="c762f-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c762f-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="c762f-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c762f-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="c762f-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c762f-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c762f-149">This property is read-only.</span></span> <span data-ttu-id="c762f-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c762f-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c762f-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c762f-151">createdDateTime</span></span>|<span data-ttu-id="c762f-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c762f-152">DateTimeOffset</span></span>|<span data-ttu-id="c762f-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c762f-153">DateTime the object was created.</span></span> <span data-ttu-id="c762f-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c762f-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c762f-155">description</span><span class="sxs-lookup"><span data-stu-id="c762f-155">description</span></span>|<span data-ttu-id="c762f-156">String</span><span class="sxs-lookup"><span data-stu-id="c762f-156">String</span></span>|<span data-ttu-id="c762f-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c762f-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c762f-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c762f-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c762f-159">displayName</span><span class="sxs-lookup"><span data-stu-id="c762f-159">displayName</span></span>|<span data-ttu-id="c762f-160">String</span><span class="sxs-lookup"><span data-stu-id="c762f-160">String</span></span>|<span data-ttu-id="c762f-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c762f-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c762f-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c762f-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c762f-163">version</span><span class="sxs-lookup"><span data-stu-id="c762f-163">version</span></span>|<span data-ttu-id="c762f-164">Int32</span><span class="sxs-lookup"><span data-stu-id="c762f-164">Int32</span></span>|<span data-ttu-id="c762f-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c762f-165">Version of the device configuration.</span></span> <span data-ttu-id="c762f-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c762f-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c762f-167">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="c762f-167">compliantAppsList</span></span>|<span data-ttu-id="c762f-168">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="c762f-168">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="c762f-169">Список приложений, соответствующих требованиям (список разрешений или блокировок, определяется свойством CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="c762f-169">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="c762f-170">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="c762f-170">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="c762f-171">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="c762f-171">compliantAppListType</span></span>|[<span data-ttu-id="c762f-172">Апплисттипе</span><span class="sxs-lookup"><span data-stu-id="c762f-172">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="c762f-173">Список, включенный в CompliantAppsList.</span><span class="sxs-lookup"><span data-stu-id="c762f-173">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="c762f-174">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="c762f-174">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="c762f-175">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="c762f-175">emailInDomainSuffixes</span></span>|<span data-ttu-id="c762f-176">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c762f-176">String collection</span></span>|<span data-ttu-id="c762f-177">Электронный адрес без суффикса, соответствующего одной из этих строк, будет считаться не добавленным в домен.</span><span class="sxs-lookup"><span data-stu-id="c762f-177">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="c762f-178">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="c762f-178">passwordBlockSimple</span></span>|<span data-ttu-id="c762f-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="c762f-179">Boolean</span></span>|<span data-ttu-id="c762f-180">Блокировка простых паролей.</span><span class="sxs-lookup"><span data-stu-id="c762f-180">Block simple passwords.</span></span>|
|<span data-ttu-id="c762f-181">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="c762f-181">passwordExpirationDays</span></span>|<span data-ttu-id="c762f-182">Int32</span><span class="sxs-lookup"><span data-stu-id="c762f-182">Int32</span></span>|<span data-ttu-id="c762f-183">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="c762f-183">Number of days before the password expires.</span></span>|
|<span data-ttu-id="c762f-184">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="c762f-184">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="c762f-185">Int32</span><span class="sxs-lookup"><span data-stu-id="c762f-185">Int32</span></span>|<span data-ttu-id="c762f-186">Количество наборов символов, которые должен содержать пароль.</span><span class="sxs-lookup"><span data-stu-id="c762f-186">Number of character sets a password must contain.</span></span> <span data-ttu-id="c762f-187">Допустимые значения: от 0 до 4.</span><span class="sxs-lookup"><span data-stu-id="c762f-187">Valid values 0 to 4</span></span>|
|<span data-ttu-id="c762f-188">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="c762f-188">passwordMinimumLength</span></span>|<span data-ttu-id="c762f-189">Int32</span><span class="sxs-lookup"><span data-stu-id="c762f-189">Int32</span></span>|<span data-ttu-id="c762f-190">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="c762f-190">Minimum length of passwords.</span></span>|
|<span data-ttu-id="c762f-191">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="c762f-191">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="c762f-192">Int32</span><span class="sxs-lookup"><span data-stu-id="c762f-192">Int32</span></span>|<span data-ttu-id="c762f-193">Период бездействия (в минутах), по истечении которого будет запрашиваться пароль.</span><span class="sxs-lookup"><span data-stu-id="c762f-193">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="c762f-194">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="c762f-194">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="c762f-195">Int32</span><span class="sxs-lookup"><span data-stu-id="c762f-195">Int32</span></span>|<span data-ttu-id="c762f-196">Период бездействия (в минутах), по истечении которого будет гаснуть экран.</span><span class="sxs-lookup"><span data-stu-id="c762f-196">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="c762f-197">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="c762f-197">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="c762f-198">Int32</span><span class="sxs-lookup"><span data-stu-id="c762f-198">Int32</span></span>|<span data-ttu-id="c762f-199">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="c762f-199">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="c762f-200">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="c762f-200">passwordRequiredType</span></span>|[<span data-ttu-id="c762f-201">Рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="c762f-201">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="c762f-202">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="c762f-202">Type of password that is required.</span></span> <span data-ttu-id="c762f-203">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="c762f-203">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="c762f-204">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="c762f-204">passwordRequired</span></span>|<span data-ttu-id="c762f-205">Логический</span><span class="sxs-lookup"><span data-stu-id="c762f-205">Boolean</span></span>|<span data-ttu-id="c762f-206">Определяет, нужно ли запрашивать ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="c762f-206">Whether or not to require a password.</span></span>|
|<span data-ttu-id="c762f-207">Кэйчаинблоккклаудсинк</span><span class="sxs-lookup"><span data-stu-id="c762f-207">keychainBlockCloudSync</span></span>|<span data-ttu-id="c762f-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="c762f-208">Boolean</span></span>|<span data-ttu-id="c762f-209">Указывает, заблокирована ли синхронизация ключей iCloud для iCloud (macOS 10,12 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="c762f-209">Indicates whether or not iCloud keychain synchronization is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="c762f-210">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="c762f-210">airPrintBlocked</span></span>|<span data-ttu-id="c762f-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="c762f-211">Boolean</span></span>|<span data-ttu-id="c762f-212">Указывает, заблокировано ли Аирпринт (macOS 10,12 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="c762f-212">Indicates whether or not AirPrint is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="c762f-213">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="c762f-213">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="c762f-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="c762f-214">Boolean</span></span>|<span data-ttu-id="c762f-215">Указывает, требуются ли доверенные сертификаты для обмена данными при печати TLS (macOS 10,13 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="c762f-215">Indicates if trusted certificates are required for TLS printing communication (macOS 10.13 and later).</span></span>|
|<span data-ttu-id="c762f-216">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="c762f-216">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="c762f-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="c762f-217">Boolean</span></span>|<span data-ttu-id="c762f-218">Указывает, блокируется ли Ибеакон обнаружение принтеров Аирпринт.</span><span class="sxs-lookup"><span data-stu-id="c762f-218">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="c762f-219">Это предотвращает ложные сигналы Аирпринт Bluetooth от фишинга для сетевого трафика (macOS 10,3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="c762f-219">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (macOS 10.3 and later).</span></span>|
|<span data-ttu-id="c762f-220">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="c762f-220">safariBlockAutofill</span></span>|<span data-ttu-id="c762f-221">Логический</span><span class="sxs-lookup"><span data-stu-id="c762f-221">Boolean</span></span>|<span data-ttu-id="c762f-222">Указывает, следует ли запретить использовать автозаполнение в Safari.</span><span class="sxs-lookup"><span data-stu-id="c762f-222">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="c762f-223">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="c762f-223">cameraBlocked</span></span>|<span data-ttu-id="c762f-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="c762f-224">Boolean</span></span>|<span data-ttu-id="c762f-225">Указывает, следует ли запретить доступ к камере устройства.</span><span class="sxs-lookup"><span data-stu-id="c762f-225">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="c762f-226">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="c762f-226">iTunesBlockMusicService</span></span>|<span data-ttu-id="c762f-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="c762f-227">Boolean</span></span>|<span data-ttu-id="c762f-228">Указывает, следует ли заблокировать музыкальную службу и вернуть приложение "Музыка" в классический режим.</span><span class="sxs-lookup"><span data-stu-id="c762f-228">Indicates whether or not to block Music service and revert Music app to classic mode.</span></span>|
|<span data-ttu-id="c762f-229">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="c762f-229">spotlightBlockInternetResults</span></span>|<span data-ttu-id="c762f-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="c762f-230">Boolean</span></span>|<span data-ttu-id="c762f-231">Указывает, следует ли запретить получение результатов из поиска в Интернете.</span><span class="sxs-lookup"><span data-stu-id="c762f-231">Indicates whether or not to block Spotlight from returning any results from an Internet search.</span></span>|
|<span data-ttu-id="c762f-232">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="c762f-232">keyboardBlockDictation</span></span>|<span data-ttu-id="c762f-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="c762f-233">Boolean</span></span>|<span data-ttu-id="c762f-234">Указывает, следует ли запретить пользователю использовать диктовку.</span><span class="sxs-lookup"><span data-stu-id="c762f-234">Indicates whether or not to block the user from using dictation input.</span></span>|
|<span data-ttu-id="c762f-235">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="c762f-235">definitionLookupBlocked</span></span>|<span data-ttu-id="c762f-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="c762f-236">Boolean</span></span>|<span data-ttu-id="c762f-237">Указывает, следует ли заблокировать Поиск определений.</span><span class="sxs-lookup"><span data-stu-id="c762f-237">Indicates whether or not to block definition lookup.</span></span>|
|<span data-ttu-id="c762f-238">Апплеватчблоккаутаунлокк</span><span class="sxs-lookup"><span data-stu-id="c762f-238">appleWatchBlockAutoUnlock</span></span>|<span data-ttu-id="c762f-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="c762f-239">Boolean</span></span>|<span data-ttu-id="c762f-240">Указывает, следует ли запретить пользователям разблокирование своего Mac-адреса с контрольной записью Apple.</span><span class="sxs-lookup"><span data-stu-id="c762f-240">Indicates whether or to block users from unlocking their Mac with Apple Watch.</span></span>|
|<span data-ttu-id="c762f-241">Итунесблоккфилешаринг</span><span class="sxs-lookup"><span data-stu-id="c762f-241">iTunesBlockFileSharing</span></span>|<span data-ttu-id="c762f-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="c762f-242">Boolean</span></span>|<span data-ttu-id="c762f-243">Указывает, следует ли запретить передачу файлов с помощью iTunes.</span><span class="sxs-lookup"><span data-stu-id="c762f-243">Indicates whether or not to block files from being transferred using iTunes.</span></span>|
|<span data-ttu-id="c762f-244">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="c762f-244">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="c762f-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="c762f-245">Boolean</span></span>|<span data-ttu-id="c762f-246">Указывает, следует ли заблокировать синхронизацию документов iCloud.</span><span class="sxs-lookup"><span data-stu-id="c762f-246">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="c762f-247">Иклаудблоккмаил</span><span class="sxs-lookup"><span data-stu-id="c762f-247">iCloudBlockMail</span></span>|<span data-ttu-id="c762f-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="c762f-248">Boolean</span></span>|<span data-ttu-id="c762f-249">Указывает, следует ли запретить синхронизацию почты для iCloud.</span><span class="sxs-lookup"><span data-stu-id="c762f-249">Indicates whether or not to block iCloud from syncing mail.</span></span>|
|<span data-ttu-id="c762f-250">Иклаудблоккаддрессбук</span><span class="sxs-lookup"><span data-stu-id="c762f-250">iCloudBlockAddressBook</span></span>|<span data-ttu-id="c762f-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="c762f-251">Boolean</span></span>|<span data-ttu-id="c762f-252">Указывает, следует ли запретить синхронизацию контактов с iCloud.</span><span class="sxs-lookup"><span data-stu-id="c762f-252">Indicates whether or not to block iCloud from syncing contacts.</span></span>|
|<span data-ttu-id="c762f-253">Иклаудблокккалендар</span><span class="sxs-lookup"><span data-stu-id="c762f-253">iCloudBlockCalendar</span></span>|<span data-ttu-id="c762f-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="c762f-254">Boolean</span></span>|<span data-ttu-id="c762f-255">Указывает, следует ли запретить синхронизацию календарей в iCloud.</span><span class="sxs-lookup"><span data-stu-id="c762f-255">Indicates whether or not to block iCloud from syncing calendars.</span></span>|
|<span data-ttu-id="c762f-256">Иклаудблоккреминдерс</span><span class="sxs-lookup"><span data-stu-id="c762f-256">iCloudBlockReminders</span></span>|<span data-ttu-id="c762f-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="c762f-257">Boolean</span></span>|<span data-ttu-id="c762f-258">Указывает, следует ли запретить синхронизацию напоминаний для iCloud.</span><span class="sxs-lookup"><span data-stu-id="c762f-258">Indicates whether or not to block iCloud from syncing reminders.</span></span>|
|<span data-ttu-id="c762f-259">Иклаудблоккбукмаркс</span><span class="sxs-lookup"><span data-stu-id="c762f-259">iCloudBlockBookmarks</span></span>|<span data-ttu-id="c762f-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="c762f-260">Boolean</span></span>|<span data-ttu-id="c762f-261">Указывает, следует ли блокировать синхронизацию закладок в iCloud.</span><span class="sxs-lookup"><span data-stu-id="c762f-261">Indicates whether or not to block iCloud from syncing bookmarks.</span></span>|
|<span data-ttu-id="c762f-262">Иклаудблоккнотес</span><span class="sxs-lookup"><span data-stu-id="c762f-262">iCloudBlockNotes</span></span>|<span data-ttu-id="c762f-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="c762f-263">Boolean</span></span>|<span data-ttu-id="c762f-264">Указывает, следует ли запретить синхронизацию заметок в iCloud.</span><span class="sxs-lookup"><span data-stu-id="c762f-264">Indicates whether or not to block iCloud from syncing notes.</span></span>|
|<span data-ttu-id="c762f-265">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="c762f-265">airDropBlocked</span></span>|<span data-ttu-id="c762f-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="c762f-266">Boolean</span></span>|<span data-ttu-id="c762f-267">Указывает, следует ли запретить AirDrop.</span><span class="sxs-lookup"><span data-stu-id="c762f-267">Indicates whether or not to allow AirDrop.</span></span>|
|<span data-ttu-id="c762f-268">Пассвордблоккмодификатион</span><span class="sxs-lookup"><span data-stu-id="c762f-268">passwordBlockModification</span></span>|<span data-ttu-id="c762f-269">Boolean</span><span class="sxs-lookup"><span data-stu-id="c762f-269">Boolean</span></span>|<span data-ttu-id="c762f-270">Указывает, следует ли запретить изменение секретного кода.</span><span class="sxs-lookup"><span data-stu-id="c762f-270">Indicates whether or not to allow passcode modification.</span></span>|
|<span data-ttu-id="c762f-271">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="c762f-271">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="c762f-272">Логический</span><span class="sxs-lookup"><span data-stu-id="c762f-272">Boolean</span></span>|<span data-ttu-id="c762f-273">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="c762f-273">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="c762f-274">Пассвордблоккаутофилл</span><span class="sxs-lookup"><span data-stu-id="c762f-274">passwordBlockAutoFill</span></span>|<span data-ttu-id="c762f-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="c762f-275">Boolean</span></span>|<span data-ttu-id="c762f-276">Указывает, следует ли заблокировать функцию автоЗаполнения паролей.</span><span class="sxs-lookup"><span data-stu-id="c762f-276">Indicates whether or not to block the AutoFill Passwords feature.</span></span>|
|<span data-ttu-id="c762f-277">Пассвордблоккпроксимитирекуестс</span><span class="sxs-lookup"><span data-stu-id="c762f-277">passwordBlockProximityRequests</span></span>|<span data-ttu-id="c762f-278">Boolean</span><span class="sxs-lookup"><span data-stu-id="c762f-278">Boolean</span></span>|<span data-ttu-id="c762f-279">Указывает, следует ли запретить запрашивать пароли с ближайших устройств.</span><span class="sxs-lookup"><span data-stu-id="c762f-279">Indicates whether or not to block requesting passwords from nearby devices.</span></span>|
|<span data-ttu-id="c762f-280">Пассвордблоккаирдропшаринг</span><span class="sxs-lookup"><span data-stu-id="c762f-280">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="c762f-281">Boolean</span><span class="sxs-lookup"><span data-stu-id="c762f-281">Boolean</span></span>|<span data-ttu-id="c762f-282">Указывает, следует ли заблокировать общий доступ к паролям с помощью функции паролей AirDrop.</span><span class="sxs-lookup"><span data-stu-id="c762f-282">Indicates whether or not to block sharing passwords with the AirDrop passwords feature.</span></span>|
|<span data-ttu-id="c762f-283">Софтвареупдатесенфорцедделайиндайс</span><span class="sxs-lookup"><span data-stu-id="c762f-283">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="c762f-284">Int32</span><span class="sxs-lookup"><span data-stu-id="c762f-284">Int32</span></span>|<span data-ttu-id="c762f-285">Задает число дней, в течение которых обновление программного обеспечения будет делед для защищенного устройства.</span><span class="sxs-lookup"><span data-stu-id="c762f-285">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="c762f-286">Допустимые значения: от 0 до 90.</span><span class="sxs-lookup"><span data-stu-id="c762f-286">Valid values 0 to 90</span></span>|
|<span data-ttu-id="c762f-287">Софтвареупдатесфорцеделайед</span><span class="sxs-lookup"><span data-stu-id="c762f-287">softwareUpdatesForceDelayed</span></span>|<span data-ttu-id="c762f-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="c762f-288">Boolean</span></span>|<span data-ttu-id="c762f-289">Указывает, следует ли откладывать видимость обновлений программного обеспечения, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="c762f-289">Indicates whether or not to delay user visibility of software updates when the device is in supervised mode.</span></span>|
|<span data-ttu-id="c762f-290">Контенткачингблоккед</span><span class="sxs-lookup"><span data-stu-id="c762f-290">contentCachingBlocked</span></span>|<span data-ttu-id="c762f-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="c762f-291">Boolean</span></span>|<span data-ttu-id="c762f-292">Указывает, следует ли запретить кэширование контента.</span><span class="sxs-lookup"><span data-stu-id="c762f-292">Indicates whether or not to allow content caching.</span></span>|



## <a name="response"></a><span data-ttu-id="c762f-293">Ответ</span><span class="sxs-lookup"><span data-stu-id="c762f-293">Response</span></span>
<span data-ttu-id="c762f-294">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c762f-294">If successful, this method returns a `201 Created` response code and a [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c762f-295">Пример</span><span class="sxs-lookup"><span data-stu-id="c762f-295">Example</span></span>

### <a name="request"></a><span data-ttu-id="c762f-296">Запрос</span><span class="sxs-lookup"><span data-stu-id="c762f-296">Request</span></span>
<span data-ttu-id="c762f-297">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c762f-297">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1988

{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  "passwordRequired": true,
  "keychainBlockCloudSync": true,
  "airPrintBlocked": true,
  "airPrintForceTrustedTLS": true,
  "airPrintBlockiBeaconDiscovery": true,
  "safariBlockAutofill": true,
  "cameraBlocked": true,
  "iTunesBlockMusicService": true,
  "spotlightBlockInternetResults": true,
  "keyboardBlockDictation": true,
  "definitionLookupBlocked": true,
  "appleWatchBlockAutoUnlock": true,
  "iTunesBlockFileSharing": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockMail": true,
  "iCloudBlockAddressBook": true,
  "iCloudBlockCalendar": true,
  "iCloudBlockReminders": true,
  "iCloudBlockBookmarks": true,
  "iCloudBlockNotes": true,
  "airDropBlocked": true,
  "passwordBlockModification": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockAutoFill": true,
  "passwordBlockProximityRequests": true,
  "passwordBlockAirDropSharing": true,
  "softwareUpdatesEnforcedDelayInDays": 2,
  "softwareUpdatesForceDelayed": true,
  "contentCachingBlocked": true
}
```

### <a name="response"></a><span data-ttu-id="c762f-298">Отклик</span><span class="sxs-lookup"><span data-stu-id="c762f-298">Response</span></span>
<span data-ttu-id="c762f-p116">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c762f-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2160

{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
  "id": "dc356aee-6aee-dc35-ee6a-35dcee6a35dc",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  "passwordRequired": true,
  "keychainBlockCloudSync": true,
  "airPrintBlocked": true,
  "airPrintForceTrustedTLS": true,
  "airPrintBlockiBeaconDiscovery": true,
  "safariBlockAutofill": true,
  "cameraBlocked": true,
  "iTunesBlockMusicService": true,
  "spotlightBlockInternetResults": true,
  "keyboardBlockDictation": true,
  "definitionLookupBlocked": true,
  "appleWatchBlockAutoUnlock": true,
  "iTunesBlockFileSharing": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockMail": true,
  "iCloudBlockAddressBook": true,
  "iCloudBlockCalendar": true,
  "iCloudBlockReminders": true,
  "iCloudBlockBookmarks": true,
  "iCloudBlockNotes": true,
  "airDropBlocked": true,
  "passwordBlockModification": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockAutoFill": true,
  "passwordBlockProximityRequests": true,
  "passwordBlockAirDropSharing": true,
  "softwareUpdatesEnforcedDelayInDays": 2,
  "softwareUpdatesForceDelayed": true,
  "contentCachingBlocked": true
}
```





