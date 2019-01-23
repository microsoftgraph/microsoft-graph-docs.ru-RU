---
title: Update windows81GeneralConfiguration
description: Обновление свойств объекта windows81GeneralConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 285b568ec1a7ee9da00d8dd54eac507c4f39755f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416228"
---
# <a name="update-windows81generalconfiguration"></a><span data-ttu-id="8f622-103">Update windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="8f622-103">Update windows81GeneralConfiguration</span></span>

> <span data-ttu-id="8f622-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8f622-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8f622-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f622-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8f622-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8f622-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f622-107">Обновление свойств объекта [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8f622-107">Update the properties of a [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8f622-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="8f622-108">Prerequisites</span></span>
<span data-ttu-id="8f622-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="8f622-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8f622-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8f622-111">Permission type</span></span>|<span data-ttu-id="8f622-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8f622-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f622-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8f622-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8f622-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f622-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8f622-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8f622-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f622-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f622-116">Not supported.</span></span>|
|<span data-ttu-id="8f622-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8f622-117">Application</span></span>|<span data-ttu-id="8f622-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f622-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f622-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8f622-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="8f622-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8f622-120">Request headers</span></span>
|<span data-ttu-id="8f622-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8f622-121">Header</span></span>|<span data-ttu-id="8f622-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8f622-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8f622-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f622-123">Authorization</span></span>|<span data-ttu-id="8f622-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8f622-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8f622-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8f622-125">Accept</span></span>|<span data-ttu-id="8f622-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8f622-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f622-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8f622-127">Request body</span></span>
<span data-ttu-id="8f622-128">В тексте запроса добавьте представление объекта [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8f622-128">In the request body, supply a JSON representation for the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

<span data-ttu-id="8f622-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8f622-129">The following table shows the properties that are required when you create the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span></span>

|<span data-ttu-id="8f622-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8f622-130">Property</span></span>|<span data-ttu-id="8f622-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8f622-131">Type</span></span>|<span data-ttu-id="8f622-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8f622-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f622-133">id</span><span class="sxs-lookup"><span data-stu-id="8f622-133">id</span></span>|<span data-ttu-id="8f622-134">String</span><span class="sxs-lookup"><span data-stu-id="8f622-134">String</span></span>|<span data-ttu-id="8f622-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8f622-135">Key of the entity.</span></span> <span data-ttu-id="8f622-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8f622-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f622-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8f622-137">lastModifiedDateTime</span></span>|<span data-ttu-id="8f622-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f622-138">DateTimeOffset</span></span>|<span data-ttu-id="8f622-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="8f622-139">DateTime the object was last modified.</span></span> <span data-ttu-id="8f622-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8f622-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f622-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8f622-141">roleScopeTagIds</span></span>|<span data-ttu-id="8f622-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8f622-142">String collection</span></span>|<span data-ttu-id="8f622-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="8f622-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8f622-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8f622-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f622-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="8f622-145">supportsScopeTags</span></span>|<span data-ttu-id="8f622-146">Логический</span><span class="sxs-lookup"><span data-stu-id="8f622-146">Boolean</span></span>|<span data-ttu-id="8f622-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="8f622-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8f622-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="8f622-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8f622-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="8f622-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8f622-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8f622-150">This property is read-only.</span></span> <span data-ttu-id="8f622-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8f622-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f622-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8f622-152">createdDateTime</span></span>|<span data-ttu-id="8f622-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f622-153">DateTimeOffset</span></span>|<span data-ttu-id="8f622-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="8f622-154">DateTime the object was created.</span></span> <span data-ttu-id="8f622-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8f622-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f622-156">description</span><span class="sxs-lookup"><span data-stu-id="8f622-156">description</span></span>|<span data-ttu-id="8f622-157">String</span><span class="sxs-lookup"><span data-stu-id="8f622-157">String</span></span>|<span data-ttu-id="8f622-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8f622-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8f622-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8f622-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f622-160">displayName</span><span class="sxs-lookup"><span data-stu-id="8f622-160">displayName</span></span>|<span data-ttu-id="8f622-161">String</span><span class="sxs-lookup"><span data-stu-id="8f622-161">String</span></span>|<span data-ttu-id="8f622-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8f622-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8f622-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8f622-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f622-164">version</span><span class="sxs-lookup"><span data-stu-id="8f622-164">version</span></span>|<span data-ttu-id="8f622-165">Int32</span><span class="sxs-lookup"><span data-stu-id="8f622-165">Int32</span></span>|<span data-ttu-id="8f622-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8f622-166">Version of the device configuration.</span></span> <span data-ttu-id="8f622-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8f622-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f622-168">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="8f622-168">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="8f622-169">Логический</span><span class="sxs-lookup"><span data-stu-id="8f622-169">Boolean</span></span>|<span data-ttu-id="8f622-170">Указывает, следует ли запретить пользователю добавлять учетные записи электронной почты на устройства, не связанные с учетной записью Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="8f622-170">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="8f622-171">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="8f622-171">applyOnlyToWindows81</span></span>|<span data-ttu-id="8f622-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f622-172">Boolean</span></span>|<span data-ttu-id="8f622-173">Указывает, применяется ли эта политика только к Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="8f622-173">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="8f622-174">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8f622-174">This property is read-only.</span></span>|
|<span data-ttu-id="8f622-175">browserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="8f622-175">browserBlockAutofill</span></span>|<span data-ttu-id="8f622-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f622-176">Boolean</span></span>|<span data-ttu-id="8f622-177">Указывает, следует ли заблокировать автозаполнение.</span><span class="sxs-lookup"><span data-stu-id="8f622-177">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="8f622-178">browserBlockAutomaticDetectionOfIntranetSites</span><span class="sxs-lookup"><span data-stu-id="8f622-178">browserBlockAutomaticDetectionOfIntranetSites</span></span>|<span data-ttu-id="8f622-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f622-179">Boolean</span></span>|<span data-ttu-id="8f622-180">Указывает, следует ли заблокировать автоматическое обнаружение сайтов интрасети.</span><span class="sxs-lookup"><span data-stu-id="8f622-180">Indicates whether or not to block automatic detection of Intranet sites.</span></span>|
|<span data-ttu-id="8f622-181">browserBlockEnterpriseModeAccess</span><span class="sxs-lookup"><span data-stu-id="8f622-181">browserBlockEnterpriseModeAccess</span></span>|<span data-ttu-id="8f622-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f622-182">Boolean</span></span>|<span data-ttu-id="8f622-183">Указывает, следует ли заблокировать доступ к корпоративному режиму.</span><span class="sxs-lookup"><span data-stu-id="8f622-183">Indicates whether or not to block enterprise mode access.</span></span>|
|<span data-ttu-id="8f622-184">browserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="8f622-184">browserBlockJavaScript</span></span>|<span data-ttu-id="8f622-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f622-185">Boolean</span></span>|<span data-ttu-id="8f622-186">Указывает, следует ли запретить использование JavaScript.</span><span class="sxs-lookup"><span data-stu-id="8f622-186">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="8f622-187">browserBlockPlugins</span><span class="sxs-lookup"><span data-stu-id="8f622-187">browserBlockPlugins</span></span>|<span data-ttu-id="8f622-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f622-188">Boolean</span></span>|<span data-ttu-id="8f622-189">Указывает, следует ли заблокировать подключаемые модули.</span><span class="sxs-lookup"><span data-stu-id="8f622-189">Indicates whether or not to block plug-ins.</span></span>|
|<span data-ttu-id="8f622-190">browserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="8f622-190">browserBlockPopups</span></span>|<span data-ttu-id="8f622-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f622-191">Boolean</span></span>|<span data-ttu-id="8f622-192">Указывает, следует ли блокировать всплывающие окна.</span><span class="sxs-lookup"><span data-stu-id="8f622-192">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="8f622-193">browserBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="8f622-193">browserBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="8f622-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f622-194">Boolean</span></span>|<span data-ttu-id="8f622-195">Указывает, следует ли запретить пользователю отправлять заголовок DNT.</span><span class="sxs-lookup"><span data-stu-id="8f622-195">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="8f622-196">browserBlockSingleWordEntryOnIntranetSites</span><span class="sxs-lookup"><span data-stu-id="8f622-196">browserBlockSingleWordEntryOnIntranetSites</span></span>|<span data-ttu-id="8f622-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f622-197">Boolean</span></span>|<span data-ttu-id="8f622-198">Указывает, следует ли блокировать переход на сайты интрасети при вводе одного слова.</span><span class="sxs-lookup"><span data-stu-id="8f622-198">Indicates whether or not to block a single word entry on Intranet sites.</span></span>|
|<span data-ttu-id="8f622-199">browserRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="8f622-199">browserRequireSmartScreen</span></span>|<span data-ttu-id="8f622-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f622-200">Boolean</span></span>|<span data-ttu-id="8f622-201">Указывает, обязательно ли использовать фильтр Smart Screen.</span><span class="sxs-lookup"><span data-stu-id="8f622-201">Indicates whether or not to require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="8f622-202">browserEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="8f622-202">browserEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="8f622-203">String</span><span class="sxs-lookup"><span data-stu-id="8f622-203">String</span></span>|<span data-ttu-id="8f622-204">Расположение списка сайтов, запускаемых в корпоративном режиме.</span><span class="sxs-lookup"><span data-stu-id="8f622-204">The enterprise mode site list location.</span></span> <span data-ttu-id="8f622-205">Это может быть локальный файл, локальная сеть или HTTP-адрес.</span><span class="sxs-lookup"><span data-stu-id="8f622-205">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="8f622-206">browserInternetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="8f622-206">browserInternetSecurityLevel</span></span>|[<span data-ttu-id="8f622-207">internetSiteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="8f622-207">internetSiteSecurityLevel</span></span>](../resources/intune-deviceconfig-internetsitesecuritylevel.md)|<span data-ttu-id="8f622-208">Уровень интернет-безопасности.</span><span class="sxs-lookup"><span data-stu-id="8f622-208">The internet security level.</span></span> <span data-ttu-id="8f622-209">Возможные значения: `userDefined`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="8f622-209">Possible values are: `userDefined`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="8f622-210">browserIntranetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="8f622-210">browserIntranetSecurityLevel</span></span>|[<span data-ttu-id="8f622-211">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="8f622-211">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="8f622-212">Уровень безопасности интрасети.</span><span class="sxs-lookup"><span data-stu-id="8f622-212">The Intranet security level.</span></span> <span data-ttu-id="8f622-213">Возможные значения: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="8f622-213">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="8f622-214">browserLoggingReportLocation</span><span class="sxs-lookup"><span data-stu-id="8f622-214">browserLoggingReportLocation</span></span>|<span data-ttu-id="8f622-215">String</span><span class="sxs-lookup"><span data-stu-id="8f622-215">String</span></span>|<span data-ttu-id="8f622-216">Расположение хранения отчетов.</span><span class="sxs-lookup"><span data-stu-id="8f622-216">The logging report location.</span></span>|
|<span data-ttu-id="8f622-217">browserRequireHighSecurityForRestrictedSites</span><span class="sxs-lookup"><span data-stu-id="8f622-217">browserRequireHighSecurityForRestrictedSites</span></span>|<span data-ttu-id="8f622-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f622-218">Boolean</span></span>|<span data-ttu-id="8f622-219">Указывает, обязателен ли высокий уровень безопасности для опасных сайтов.</span><span class="sxs-lookup"><span data-stu-id="8f622-219">Indicates whether or not to require high security for restricted sites.</span></span>|
|<span data-ttu-id="8f622-220">browserRequireFirewall</span><span class="sxs-lookup"><span data-stu-id="8f622-220">browserRequireFirewall</span></span>|<span data-ttu-id="8f622-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f622-221">Boolean</span></span>|<span data-ttu-id="8f622-222">Указывает, обязательно ли использовать брандмауэр.</span><span class="sxs-lookup"><span data-stu-id="8f622-222">Indicates whether or not to require a firewall.</span></span>|
|<span data-ttu-id="8f622-223">browserRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="8f622-223">browserRequireFraudWarning</span></span>|<span data-ttu-id="8f622-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f622-224">Boolean</span></span>|<span data-ttu-id="8f622-225">Указывает, обязательно ли предупреждение о мошенничестве.</span><span class="sxs-lookup"><span data-stu-id="8f622-225">Indicates whether or not to require fraud warning.</span></span>|
|<span data-ttu-id="8f622-226">browserTrustedSitesSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="8f622-226">browserTrustedSitesSecurityLevel</span></span>|[<span data-ttu-id="8f622-227">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="8f622-227">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="8f622-228">Уровень безопасности надежных сайтов.</span><span class="sxs-lookup"><span data-stu-id="8f622-228">The trusted sites security level.</span></span> <span data-ttu-id="8f622-229">Возможные значения: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="8f622-229">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="8f622-230">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="8f622-230">cellularBlockDataRoaming</span></span>|<span data-ttu-id="8f622-231">Логический</span><span class="sxs-lookup"><span data-stu-id="8f622-231">Boolean</span></span>|<span data-ttu-id="8f622-232">Указывает, следует ли блокировать передачу данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="8f622-232">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="8f622-233">diagnosticsBlockDataSubmission</span><span class="sxs-lookup"><span data-stu-id="8f622-233">diagnosticsBlockDataSubmission</span></span>|<span data-ttu-id="8f622-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f622-234">Boolean</span></span>|<span data-ttu-id="8f622-235">Указывает, следует ли блокировать отправку диагностических данных.</span><span class="sxs-lookup"><span data-stu-id="8f622-235">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="8f622-236">passwordBlockPicturePasswordAndPin</span><span class="sxs-lookup"><span data-stu-id="8f622-236">passwordBlockPicturePasswordAndPin</span></span>|<span data-ttu-id="8f622-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f622-237">Boolean</span></span>|<span data-ttu-id="8f622-238">Указывает, следует ли запретить использование графического пароля и ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="8f622-238">Indicates whether or not to Block the user from using a pictures password and pin.</span></span>|
|<span data-ttu-id="8f622-239">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="8f622-239">passwordExpirationDays</span></span>|<span data-ttu-id="8f622-240">Int32</span><span class="sxs-lookup"><span data-stu-id="8f622-240">Int32</span></span>|<span data-ttu-id="8f622-241">Срок действия пароля (в днях).</span><span class="sxs-lookup"><span data-stu-id="8f622-241">Password expiration in days.</span></span>|
|<span data-ttu-id="8f622-242">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="8f622-242">passwordMinimumLength</span></span>|<span data-ttu-id="8f622-243">Int32</span><span class="sxs-lookup"><span data-stu-id="8f622-243">Int32</span></span>|<span data-ttu-id="8f622-244">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="8f622-244">The minimum password length.</span></span>|
|<span data-ttu-id="8f622-245">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="8f622-245">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="8f622-246">Int32</span><span class="sxs-lookup"><span data-stu-id="8f622-246">Int32</span></span>|<span data-ttu-id="8f622-247">Время бездействия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="8f622-247">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="8f622-248">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="8f622-248">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="8f622-249">Int32</span><span class="sxs-lookup"><span data-stu-id="8f622-249">Int32</span></span>|<span data-ttu-id="8f622-250">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="8f622-250">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="8f622-251">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="8f622-251">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="8f622-252">Int32</span><span class="sxs-lookup"><span data-stu-id="8f622-252">Int32</span></span>|<span data-ttu-id="8f622-253">Количество предыдущих паролей, повторное использование которых следует запретить.</span><span class="sxs-lookup"><span data-stu-id="8f622-253">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="8f622-254">Допустимые значения: от 0 до 24</span><span class="sxs-lookup"><span data-stu-id="8f622-254">Valid values 0 to 24</span></span>|
|<span data-ttu-id="8f622-255">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="8f622-255">passwordRequiredType</span></span>|[<span data-ttu-id="8f622-256">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="8f622-256">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="8f622-257">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="8f622-257">The required password type.</span></span> <span data-ttu-id="8f622-258">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="8f622-258">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="8f622-259">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="8f622-259">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="8f622-260">Int32</span><span class="sxs-lookup"><span data-stu-id="8f622-260">Int32</span></span>|<span data-ttu-id="8f622-261">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="8f622-261">The number of sign in failures before factory reset.</span></span>|
|<span data-ttu-id="8f622-262">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="8f622-262">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="8f622-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f622-263">Boolean</span></span>|<span data-ttu-id="8f622-264">Указывает, обязательно ли шифрование данных на мобильном устройстве.</span><span class="sxs-lookup"><span data-stu-id="8f622-264">Indicates whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="8f622-265">minimumAutoInstallClassification</span><span class="sxs-lookup"><span data-stu-id="8f622-265">minimumAutoInstallClassification</span></span>|[<span data-ttu-id="8f622-266">updateClassification</span><span class="sxs-lookup"><span data-stu-id="8f622-266">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="8f622-267">Как минимум обновление классификации для автоматической установки.</span><span class="sxs-lookup"><span data-stu-id="8f622-267">The minimum update classification to install automatically.</span></span> <span data-ttu-id="8f622-268">Возможные значения: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span><span class="sxs-lookup"><span data-stu-id="8f622-268">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="8f622-269">updatesMinimumAutoInstallClassification</span><span class="sxs-lookup"><span data-stu-id="8f622-269">updatesMinimumAutoInstallClassification</span></span>|[<span data-ttu-id="8f622-270">updateClassification</span><span class="sxs-lookup"><span data-stu-id="8f622-270">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="8f622-271">Как минимум обновление классификации для автоматической установки.</span><span class="sxs-lookup"><span data-stu-id="8f622-271">The minimum update classification to install automatically.</span></span> <span data-ttu-id="8f622-272">Возможные значения: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span><span class="sxs-lookup"><span data-stu-id="8f622-272">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="8f622-273">updatesRequireAutomaticUpdates</span><span class="sxs-lookup"><span data-stu-id="8f622-273">updatesRequireAutomaticUpdates</span></span>|<span data-ttu-id="8f622-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f622-274">Boolean</span></span>|<span data-ttu-id="8f622-275">Указывает, обязательно ли автоматическое обновление.</span><span class="sxs-lookup"><span data-stu-id="8f622-275">Indicates whether or not to require automatic updates.</span></span>|
|<span data-ttu-id="8f622-276">userAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="8f622-276">userAccountControlSettings</span></span>|[<span data-ttu-id="8f622-277">windowsUserAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="8f622-277">windowsUserAccountControlSettings</span></span>](../resources/intune-deviceconfig-windowsuseraccountcontrolsettings.md)|<span data-ttu-id="8f622-278">Настройки контроля учетных записей.</span><span class="sxs-lookup"><span data-stu-id="8f622-278">The user account control settings.</span></span> <span data-ttu-id="8f622-279">Возможные значения: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span><span class="sxs-lookup"><span data-stu-id="8f622-279">Possible values are: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span></span>|
|<span data-ttu-id="8f622-280">workFoldersUrl</span><span class="sxs-lookup"><span data-stu-id="8f622-280">workFoldersUrl</span></span>|<span data-ttu-id="8f622-281">String</span><span class="sxs-lookup"><span data-stu-id="8f622-281">String</span></span>|<span data-ttu-id="8f622-282">URL-адрес рабочей папки.</span><span class="sxs-lookup"><span data-stu-id="8f622-282">The work folders url.</span></span>|



## <a name="response"></a><span data-ttu-id="8f622-283">Ответ</span><span class="sxs-lookup"><span data-stu-id="8f622-283">Response</span></span>
<span data-ttu-id="8f622-284">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="8f622-284">If successful, this method returns a `200 OK` response code and an updated [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f622-285">Пример</span><span class="sxs-lookup"><span data-stu-id="8f622-285">Example</span></span>

### <a name="request"></a><span data-ttu-id="8f622-286">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f622-286">Request</span></span>
<span data-ttu-id="8f622-287">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8f622-287">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1924

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "applyOnlyToWindows81": true,
  "browserBlockAutofill": true,
  "browserBlockAutomaticDetectionOfIntranetSites": true,
  "browserBlockEnterpriseModeAccess": true,
  "browserBlockJavaScript": true,
  "browserBlockPlugins": true,
  "browserBlockPopups": true,
  "browserBlockSendingDoNotTrackHeader": true,
  "browserBlockSingleWordEntryOnIntranetSites": true,
  "browserRequireSmartScreen": true,
  "browserEnterpriseModeSiteListLocation": "Browser Enterprise Mode Site List Location value",
  "browserInternetSecurityLevel": "medium",
  "browserIntranetSecurityLevel": "low",
  "browserLoggingReportLocation": "Browser Logging Report Location value",
  "browserRequireHighSecurityForRestrictedSites": true,
  "browserRequireFirewall": true,
  "browserRequireFraudWarning": true,
  "browserTrustedSitesSecurityLevel": "low",
  "cellularBlockDataRoaming": true,
  "diagnosticsBlockDataSubmission": true,
  "passwordBlockPicturePasswordAndPin": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "storageRequireDeviceEncryption": true,
  "minimumAutoInstallClassification": "recommendedAndImportant",
  "updatesMinimumAutoInstallClassification": "recommendedAndImportant",
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "alwaysNotify",
  "workFoldersUrl": "https://example.com/workFoldersUrl/"
}
```

### <a name="response"></a><span data-ttu-id="8f622-288">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f622-288">Response</span></span>
<span data-ttu-id="8f622-p121">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8f622-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2096

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "id": "0e9285b5-85b5-0e92-b585-920eb585920e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "applyOnlyToWindows81": true,
  "browserBlockAutofill": true,
  "browserBlockAutomaticDetectionOfIntranetSites": true,
  "browserBlockEnterpriseModeAccess": true,
  "browserBlockJavaScript": true,
  "browserBlockPlugins": true,
  "browserBlockPopups": true,
  "browserBlockSendingDoNotTrackHeader": true,
  "browserBlockSingleWordEntryOnIntranetSites": true,
  "browserRequireSmartScreen": true,
  "browserEnterpriseModeSiteListLocation": "Browser Enterprise Mode Site List Location value",
  "browserInternetSecurityLevel": "medium",
  "browserIntranetSecurityLevel": "low",
  "browserLoggingReportLocation": "Browser Logging Report Location value",
  "browserRequireHighSecurityForRestrictedSites": true,
  "browserRequireFirewall": true,
  "browserRequireFraudWarning": true,
  "browserTrustedSitesSecurityLevel": "low",
  "cellularBlockDataRoaming": true,
  "diagnosticsBlockDataSubmission": true,
  "passwordBlockPicturePasswordAndPin": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "storageRequireDeviceEncryption": true,
  "minimumAutoInstallClassification": "recommendedAndImportant",
  "updatesMinimumAutoInstallClassification": "recommendedAndImportant",
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "alwaysNotify",
  "workFoldersUrl": "https://example.com/workFoldersUrl/"
}
```




