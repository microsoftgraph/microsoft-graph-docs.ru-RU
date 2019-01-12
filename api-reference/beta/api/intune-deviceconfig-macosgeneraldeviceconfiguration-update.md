---
title: Update macOSGeneralDeviceConfiguration
description: Обновление свойств объекта macOSGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: db5f07f2cfbf183cfe38c7a5837e1ccaf78821bb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929125"
---
# <a name="update-macosgeneraldeviceconfiguration"></a><span data-ttu-id="b9431-103">Update macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="b9431-103">Update macOSGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="b9431-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b9431-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b9431-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9431-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b9431-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b9431-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b9431-107">Обновление свойств объекта [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b9431-107">Update the properties of a [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b9431-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="b9431-108">Prerequisites</span></span>
<span data-ttu-id="b9431-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9431-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9431-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b9431-111">Permission type</span></span>|<span data-ttu-id="b9431-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b9431-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9431-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b9431-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b9431-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9431-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b9431-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b9431-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9431-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9431-116">Not supported.</span></span>|
|<span data-ttu-id="b9431-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b9431-117">Application</span></span>|<span data-ttu-id="b9431-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9431-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9431-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b9431-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b9431-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b9431-120">Request headers</span></span>
|<span data-ttu-id="b9431-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b9431-121">Header</span></span>|<span data-ttu-id="b9431-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b9431-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9431-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9431-123">Authorization</span></span>|<span data-ttu-id="b9431-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b9431-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9431-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b9431-125">Accept</span></span>|<span data-ttu-id="b9431-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b9431-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9431-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b9431-127">Request body</span></span>
<span data-ttu-id="b9431-128">В теле запроса добавьте представление объекта [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b9431-128">In the request body, supply a JSON representation for the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="b9431-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b9431-129">The following table shows the properties that are required when you create the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="b9431-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b9431-130">Property</span></span>|<span data-ttu-id="b9431-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b9431-131">Type</span></span>|<span data-ttu-id="b9431-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b9431-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9431-133">id</span><span class="sxs-lookup"><span data-stu-id="b9431-133">id</span></span>|<span data-ttu-id="b9431-134">Строка</span><span class="sxs-lookup"><span data-stu-id="b9431-134">String</span></span>|<span data-ttu-id="b9431-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b9431-135">Key of the entity.</span></span> <span data-ttu-id="b9431-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b9431-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9431-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b9431-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b9431-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9431-138">DateTimeOffset</span></span>|<span data-ttu-id="b9431-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="b9431-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b9431-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b9431-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9431-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b9431-141">roleScopeTagIds</span></span>|<span data-ttu-id="b9431-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b9431-142">String collection</span></span>|<span data-ttu-id="b9431-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="b9431-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b9431-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b9431-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9431-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b9431-145">supportsScopeTags</span></span>|<span data-ttu-id="b9431-146">Логический</span><span class="sxs-lookup"><span data-stu-id="b9431-146">Boolean</span></span>|<span data-ttu-id="b9431-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="b9431-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b9431-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="b9431-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b9431-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="b9431-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b9431-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b9431-150">This property is read-only.</span></span> <span data-ttu-id="b9431-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b9431-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9431-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b9431-152">createdDateTime</span></span>|<span data-ttu-id="b9431-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9431-153">DateTimeOffset</span></span>|<span data-ttu-id="b9431-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="b9431-154">DateTime the object was created.</span></span> <span data-ttu-id="b9431-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b9431-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9431-156">описание</span><span class="sxs-lookup"><span data-stu-id="b9431-156">description</span></span>|<span data-ttu-id="b9431-157">Строка</span><span class="sxs-lookup"><span data-stu-id="b9431-157">String</span></span>|<span data-ttu-id="b9431-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b9431-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b9431-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b9431-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9431-160">displayName</span><span class="sxs-lookup"><span data-stu-id="b9431-160">displayName</span></span>|<span data-ttu-id="b9431-161">Строка</span><span class="sxs-lookup"><span data-stu-id="b9431-161">String</span></span>|<span data-ttu-id="b9431-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b9431-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b9431-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b9431-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9431-164">version</span><span class="sxs-lookup"><span data-stu-id="b9431-164">version</span></span>|<span data-ttu-id="b9431-165">Int32</span><span class="sxs-lookup"><span data-stu-id="b9431-165">Int32</span></span>|<span data-ttu-id="b9431-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b9431-166">Version of the device configuration.</span></span> <span data-ttu-id="b9431-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b9431-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9431-168">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="b9431-168">compliantAppsList</span></span>|<span data-ttu-id="b9431-169">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="b9431-169">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="b9431-170">Список приложений (разрешенных или заблокированных в зависимости от значения свойства CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="b9431-170">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="b9431-171">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="b9431-171">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="b9431-172">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="b9431-172">compliantAppListType</span></span>|[<span data-ttu-id="b9431-173">appListType</span><span class="sxs-lookup"><span data-stu-id="b9431-173">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="b9431-174">Список, включенный в CompliantAppsList.</span><span class="sxs-lookup"><span data-stu-id="b9431-174">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="b9431-175">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="b9431-175">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="b9431-176">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="b9431-176">emailInDomainSuffixes</span></span>|<span data-ttu-id="b9431-177">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b9431-177">String collection</span></span>|<span data-ttu-id="b9431-178">Электронный адрес без суффикса, соответствующего одной из этих строк, будет считаться не добавленным в домен.</span><span class="sxs-lookup"><span data-stu-id="b9431-178">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="b9431-179">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="b9431-179">passwordBlockSimple</span></span>|<span data-ttu-id="b9431-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9431-180">Boolean</span></span>|<span data-ttu-id="b9431-181">Блокировка простых паролей.</span><span class="sxs-lookup"><span data-stu-id="b9431-181">Block simple passwords.</span></span>|
|<span data-ttu-id="b9431-182">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="b9431-182">passwordExpirationDays</span></span>|<span data-ttu-id="b9431-183">Int32</span><span class="sxs-lookup"><span data-stu-id="b9431-183">Int32</span></span>|<span data-ttu-id="b9431-184">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="b9431-184">Number of days before the password expires.</span></span>|
|<span data-ttu-id="b9431-185">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="b9431-185">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="b9431-186">Int32</span><span class="sxs-lookup"><span data-stu-id="b9431-186">Int32</span></span>|<span data-ttu-id="b9431-187">Количество наборов символов, которые должен содержать пароль.</span><span class="sxs-lookup"><span data-stu-id="b9431-187">Number of character sets a password must contain.</span></span> <span data-ttu-id="b9431-188">Допустимые значения: от 0 до 4.</span><span class="sxs-lookup"><span data-stu-id="b9431-188">Valid values 0 to 4</span></span>|
|<span data-ttu-id="b9431-189">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="b9431-189">passwordMinimumLength</span></span>|<span data-ttu-id="b9431-190">Int32</span><span class="sxs-lookup"><span data-stu-id="b9431-190">Int32</span></span>|<span data-ttu-id="b9431-191">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="b9431-191">Minimum length of passwords.</span></span>|
|<span data-ttu-id="b9431-192">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="b9431-192">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="b9431-193">Int32</span><span class="sxs-lookup"><span data-stu-id="b9431-193">Int32</span></span>|<span data-ttu-id="b9431-194">Период бездействия (в минутах), по истечении которого будет запрашиваться пароль.</span><span class="sxs-lookup"><span data-stu-id="b9431-194">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="b9431-195">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="b9431-195">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="b9431-196">Int32</span><span class="sxs-lookup"><span data-stu-id="b9431-196">Int32</span></span>|<span data-ttu-id="b9431-197">Период бездействия (в минутах), по истечении которого гаснет экран.</span><span class="sxs-lookup"><span data-stu-id="b9431-197">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="b9431-198">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="b9431-198">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="b9431-199">Int32</span><span class="sxs-lookup"><span data-stu-id="b9431-199">Int32</span></span>|<span data-ttu-id="b9431-200">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="b9431-200">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="b9431-201">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="b9431-201">passwordRequiredType</span></span>|[<span data-ttu-id="b9431-202">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="b9431-202">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="b9431-203">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="b9431-203">Type of password that is required.</span></span> <span data-ttu-id="b9431-204">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="b9431-204">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="b9431-205">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="b9431-205">passwordRequired</span></span>|<span data-ttu-id="b9431-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9431-206">Boolean</span></span>|<span data-ttu-id="b9431-207">Указывает, обязательно ли использовать пароль.</span><span class="sxs-lookup"><span data-stu-id="b9431-207">Whether or not to require a password.</span></span>|
|<span data-ttu-id="b9431-208">keychainBlockCloudSync</span><span class="sxs-lookup"><span data-stu-id="b9431-208">keychainBlockCloudSync</span></span>|<span data-ttu-id="b9431-209">Логический</span><span class="sxs-lookup"><span data-stu-id="b9431-209">Boolean</span></span>|<span data-ttu-id="b9431-210">Указывает, является ли iCloud ключей синхронизации заблокированных (macOS 10.12 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="b9431-210">Indicates whether or not iCloud keychain synchronization is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="b9431-211">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="b9431-211">airPrintBlocked</span></span>|<span data-ttu-id="b9431-212">Логический</span><span class="sxs-lookup"><span data-stu-id="b9431-212">Boolean</span></span>|<span data-ttu-id="b9431-213">Указывает, является ли AirPrint заблокированных (macOS 10.12 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="b9431-213">Indicates whether or not AirPrint is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="b9431-214">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="b9431-214">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="b9431-215">Логический</span><span class="sxs-lookup"><span data-stu-id="b9431-215">Boolean</span></span>|<span data-ttu-id="b9431-216">Указывает, являются ли доверенные сертификаты для печати обмена данными TLS (macOS 10.13 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="b9431-216">Indicates if trusted certificates are required for TLS printing communication (macOS 10.13 and later).</span></span>|
|<span data-ttu-id="b9431-217">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="b9431-217">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="b9431-218">Логический</span><span class="sxs-lookup"><span data-stu-id="b9431-218">Boolean</span></span>|<span data-ttu-id="b9431-219">Указывает, заблокирован ли обнаружения iBeacon AirPrint принтеров.</span><span class="sxs-lookup"><span data-stu-id="b9431-219">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="b9431-220">Это позволяет предотвратить ложных маяки AirPrint Bluetooth от фишинга для сетевого трафика (macOS 10.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="b9431-220">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (macOS 10.3 and later).</span></span>|
|<span data-ttu-id="b9431-221">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="b9431-221">safariBlockAutofill</span></span>|<span data-ttu-id="b9431-222">Логический</span><span class="sxs-lookup"><span data-stu-id="b9431-222">Boolean</span></span>|<span data-ttu-id="b9431-223">Указывает, следует ли запретить использовать автозаполнение в Safari.</span><span class="sxs-lookup"><span data-stu-id="b9431-223">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="b9431-224">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="b9431-224">cameraBlocked</span></span>|<span data-ttu-id="b9431-225">Логический</span><span class="sxs-lookup"><span data-stu-id="b9431-225">Boolean</span></span>|<span data-ttu-id="b9431-226">Указывает, следует ли запретить доступ к камере устройства.</span><span class="sxs-lookup"><span data-stu-id="b9431-226">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="b9431-227">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="b9431-227">iTunesBlockMusicService</span></span>|<span data-ttu-id="b9431-228">Логический</span><span class="sxs-lookup"><span data-stu-id="b9431-228">Boolean</span></span>|<span data-ttu-id="b9431-229">Указывает, следует ли блокировать службы музыки и вернуться музыки приложения в классическом режиме.</span><span class="sxs-lookup"><span data-stu-id="b9431-229">Indicates whether or not to block Music service and revert Music app to classic mode.</span></span>|
|<span data-ttu-id="b9431-230">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="b9431-230">spotlightBlockInternetResults</span></span>|<span data-ttu-id="b9431-231">Логический</span><span class="sxs-lookup"><span data-stu-id="b9431-231">Boolean</span></span>|<span data-ttu-id="b9431-232">Указывает, следует ли запретить возвращение результатов из и поиск в Интернете в центре внимания.</span><span class="sxs-lookup"><span data-stu-id="b9431-232">Indicates whether or not to block Spotlight from returning any results from an Internet search.</span></span>|
|<span data-ttu-id="b9431-233">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="b9431-233">keyboardBlockDictation</span></span>|<span data-ttu-id="b9431-234">Логический</span><span class="sxs-lookup"><span data-stu-id="b9431-234">Boolean</span></span>|<span data-ttu-id="b9431-235">Указывает, следует ли пользователь с помощью диктовки входные данные.</span><span class="sxs-lookup"><span data-stu-id="b9431-235">Indicates whether or not to block the user from using dictation input.</span></span>|
|<span data-ttu-id="b9431-236">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="b9431-236">definitionLookupBlocked</span></span>|<span data-ttu-id="b9431-237">Логический</span><span class="sxs-lookup"><span data-stu-id="b9431-237">Boolean</span></span>|<span data-ttu-id="b9431-238">Указывает, следует ли блокировать определение подстановки.</span><span class="sxs-lookup"><span data-stu-id="b9431-238">Indicates whether or not to block definition lookup.</span></span>|
|<span data-ttu-id="b9431-239">appleWatchBlockAutoUnlock</span><span class="sxs-lookup"><span data-stu-id="b9431-239">appleWatchBlockAutoUnlock</span></span>|<span data-ttu-id="b9431-240">Логический</span><span class="sxs-lookup"><span data-stu-id="b9431-240">Boolean</span></span>|<span data-ttu-id="b9431-241">Указывает, является ли или чтобы запретить пользователям разблокирование их Mac с Apple Watch.</span><span class="sxs-lookup"><span data-stu-id="b9431-241">Indicates whether or to block users from unlocking their Mac with Apple Watch.</span></span>|
|<span data-ttu-id="b9431-242">iTunesBlockFileSharing</span><span class="sxs-lookup"><span data-stu-id="b9431-242">iTunesBlockFileSharing</span></span>|<span data-ttu-id="b9431-243">Логический</span><span class="sxs-lookup"><span data-stu-id="b9431-243">Boolean</span></span>|<span data-ttu-id="b9431-244">Указывает ли для блокировки файлов, из которых передаются с помощью iTunes.</span><span class="sxs-lookup"><span data-stu-id="b9431-244">Indicates whether or not to block files from being transferred using iTunes.</span></span>|
|<span data-ttu-id="b9431-245">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="b9431-245">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="b9431-246">Логический</span><span class="sxs-lookup"><span data-stu-id="b9431-246">Boolean</span></span>|<span data-ttu-id="b9431-247">Указывает, следует ли заблокировать синхронизацию документов iCloud.</span><span class="sxs-lookup"><span data-stu-id="b9431-247">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="b9431-248">iCloudBlockMail</span><span class="sxs-lookup"><span data-stu-id="b9431-248">iCloudBlockMail</span></span>|<span data-ttu-id="b9431-249">Логический</span><span class="sxs-lookup"><span data-stu-id="b9431-249">Boolean</span></span>|<span data-ttu-id="b9431-250">Указывает, следует ли блокировать iCloud синхронизацию почты.</span><span class="sxs-lookup"><span data-stu-id="b9431-250">Indicates whether or not to block iCloud from syncing mail.</span></span>|
|<span data-ttu-id="b9431-251">iCloudBlockAddressBook</span><span class="sxs-lookup"><span data-stu-id="b9431-251">iCloudBlockAddressBook</span></span>|<span data-ttu-id="b9431-252">Логический</span><span class="sxs-lookup"><span data-stu-id="b9431-252">Boolean</span></span>|<span data-ttu-id="b9431-253">Указывает, следует ли блокировать iCloud синхронизацию контактов.</span><span class="sxs-lookup"><span data-stu-id="b9431-253">Indicates whether or not to block iCloud from syncing contacts.</span></span>|
|<span data-ttu-id="b9431-254">iCloudBlockCalendar</span><span class="sxs-lookup"><span data-stu-id="b9431-254">iCloudBlockCalendar</span></span>|<span data-ttu-id="b9431-255">Логический</span><span class="sxs-lookup"><span data-stu-id="b9431-255">Boolean</span></span>|<span data-ttu-id="b9431-256">Указывает, следует ли блокировать iCloud из списка синхронизации календарей.</span><span class="sxs-lookup"><span data-stu-id="b9431-256">Indicates whether or not to block iCloud from syncing calendars.</span></span>|
|<span data-ttu-id="b9431-257">iCloudBlockReminders</span><span class="sxs-lookup"><span data-stu-id="b9431-257">iCloudBlockReminders</span></span>|<span data-ttu-id="b9431-258">Логический</span><span class="sxs-lookup"><span data-stu-id="b9431-258">Boolean</span></span>|<span data-ttu-id="b9431-259">Указывает, следует ли блокировать iCloud синхронизацию напоминания.</span><span class="sxs-lookup"><span data-stu-id="b9431-259">Indicates whether or not to block iCloud from syncing reminders.</span></span>|
|<span data-ttu-id="b9431-260">iCloudBlockBookmarks</span><span class="sxs-lookup"><span data-stu-id="b9431-260">iCloudBlockBookmarks</span></span>|<span data-ttu-id="b9431-261">Логический</span><span class="sxs-lookup"><span data-stu-id="b9431-261">Boolean</span></span>|<span data-ttu-id="b9431-262">Указывает, следует ли блокировать iCloud синхронизацию закладки.</span><span class="sxs-lookup"><span data-stu-id="b9431-262">Indicates whether or not to block iCloud from syncing bookmarks.</span></span>|
|<span data-ttu-id="b9431-263">iCloudBlockNotes</span><span class="sxs-lookup"><span data-stu-id="b9431-263">iCloudBlockNotes</span></span>|<span data-ttu-id="b9431-264">Логический</span><span class="sxs-lookup"><span data-stu-id="b9431-264">Boolean</span></span>|<span data-ttu-id="b9431-265">Указывает, следует ли блокировать iCloud синхронизацию заметки.</span><span class="sxs-lookup"><span data-stu-id="b9431-265">Indicates whether or not to block iCloud from syncing notes.</span></span>|
|<span data-ttu-id="b9431-266">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="b9431-266">airDropBlocked</span></span>|<span data-ttu-id="b9431-267">Логический</span><span class="sxs-lookup"><span data-stu-id="b9431-267">Boolean</span></span>|<span data-ttu-id="b9431-268">Указывает, следует ли разрешить AirDrop.</span><span class="sxs-lookup"><span data-stu-id="b9431-268">Indicates whether or not to allow AirDrop.</span></span>|
|<span data-ttu-id="b9431-269">passwordBlockModification</span><span class="sxs-lookup"><span data-stu-id="b9431-269">passwordBlockModification</span></span>|<span data-ttu-id="b9431-270">Логический</span><span class="sxs-lookup"><span data-stu-id="b9431-270">Boolean</span></span>|<span data-ttu-id="b9431-271">Указывает, следует ли разрешить изменения секретный код.</span><span class="sxs-lookup"><span data-stu-id="b9431-271">Indicates whether or not to allow passcode modification.</span></span>|
|<span data-ttu-id="b9431-272">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="b9431-272">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="b9431-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9431-273">Boolean</span></span>|<span data-ttu-id="b9431-274">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="b9431-274">Indicates whether or not to block fingerprint unlock.</span></span>|



## <a name="response"></a><span data-ttu-id="b9431-275">Ответ</span><span class="sxs-lookup"><span data-stu-id="b9431-275">Response</span></span>
<span data-ttu-id="b9431-276">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b9431-276">If successful, this method returns a `200 OK` response code and an updated [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9431-277">Пример</span><span class="sxs-lookup"><span data-stu-id="b9431-277">Example</span></span>
### <a name="request"></a><span data-ttu-id="b9431-278">Запрос</span><span class="sxs-lookup"><span data-stu-id="b9431-278">Request</span></span>
<span data-ttu-id="b9431-279">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b9431-279">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1747

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  "passwordBlockFingerprintUnlock": true
}
```

### <a name="response"></a><span data-ttu-id="b9431-280">Ответ</span><span class="sxs-lookup"><span data-stu-id="b9431-280">Response</span></span>
<span data-ttu-id="b9431-p116">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b9431-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1925

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
  "passwordBlockFingerprintUnlock": true
}
```





