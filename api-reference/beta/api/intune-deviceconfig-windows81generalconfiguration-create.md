---
title: Создание windows81GeneralConfiguration
description: Создание объекта windows81GeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 486b21ac0e420188dac738f9c8c2e53c78dbe30d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863864"
---
# <a name="create-windows81generalconfiguration"></a><span data-ttu-id="e2cfd-103">Создание windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="e2cfd-103">Create windows81GeneralConfiguration</span></span>

> <span data-ttu-id="e2cfd-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e2cfd-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e2cfd-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e2cfd-107">Создание объекта [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2cfd-107">Create a new [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e2cfd-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e2cfd-108">Prerequisites</span></span>
<span data-ttu-id="e2cfd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2cfd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2cfd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e2cfd-111">Permission type</span></span>|<span data-ttu-id="e2cfd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e2cfd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2cfd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e2cfd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e2cfd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2cfd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e2cfd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e2cfd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2cfd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-116">Not supported.</span></span>|
|<span data-ttu-id="e2cfd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e2cfd-117">Application</span></span>|<span data-ttu-id="e2cfd-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2cfd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e2cfd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e2cfd-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e2cfd-120">Request headers</span></span>
|<span data-ttu-id="e2cfd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e2cfd-121">Header</span></span>|<span data-ttu-id="e2cfd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e2cfd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2cfd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2cfd-123">Authorization</span></span>|<span data-ttu-id="e2cfd-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e2cfd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2cfd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e2cfd-125">Accept</span></span>|<span data-ttu-id="e2cfd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e2cfd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2cfd-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e2cfd-127">Request body</span></span>
<span data-ttu-id="e2cfd-128">В теле запроса добавьте представление объекта windows81GeneralConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-128">In the request body, supply a JSON representation for the windows81GeneralConfiguration object.</span></span>

<span data-ttu-id="e2cfd-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта windows81GeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-129">The following table shows the properties that are required when you create the windows81GeneralConfiguration.</span></span>

|<span data-ttu-id="e2cfd-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e2cfd-130">Property</span></span>|<span data-ttu-id="e2cfd-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e2cfd-131">Type</span></span>|<span data-ttu-id="e2cfd-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e2cfd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2cfd-133">id</span><span class="sxs-lookup"><span data-stu-id="e2cfd-133">id</span></span>|<span data-ttu-id="e2cfd-134">Строка</span><span class="sxs-lookup"><span data-stu-id="e2cfd-134">String</span></span>|<span data-ttu-id="e2cfd-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-135">Key of the entity.</span></span> <span data-ttu-id="e2cfd-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2cfd-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2cfd-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e2cfd-137">lastModifiedDateTime</span></span>|<span data-ttu-id="e2cfd-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2cfd-138">DateTimeOffset</span></span>|<span data-ttu-id="e2cfd-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-139">DateTime the object was last modified.</span></span> <span data-ttu-id="e2cfd-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2cfd-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2cfd-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e2cfd-141">roleScopeTagIds</span></span>|<span data-ttu-id="e2cfd-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e2cfd-142">String collection</span></span>|<span data-ttu-id="e2cfd-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e2cfd-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2cfd-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2cfd-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e2cfd-145">supportsScopeTags</span></span>|<span data-ttu-id="e2cfd-146">Логический</span><span class="sxs-lookup"><span data-stu-id="e2cfd-146">Boolean</span></span>|<span data-ttu-id="e2cfd-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e2cfd-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e2cfd-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e2cfd-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-150">This property is read-only.</span></span> <span data-ttu-id="e2cfd-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2cfd-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2cfd-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e2cfd-152">createdDateTime</span></span>|<span data-ttu-id="e2cfd-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2cfd-153">DateTimeOffset</span></span>|<span data-ttu-id="e2cfd-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-154">DateTime the object was created.</span></span> <span data-ttu-id="e2cfd-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2cfd-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2cfd-156">описание</span><span class="sxs-lookup"><span data-stu-id="e2cfd-156">description</span></span>|<span data-ttu-id="e2cfd-157">Строка</span><span class="sxs-lookup"><span data-stu-id="e2cfd-157">String</span></span>|<span data-ttu-id="e2cfd-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e2cfd-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2cfd-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2cfd-160">displayName</span><span class="sxs-lookup"><span data-stu-id="e2cfd-160">displayName</span></span>|<span data-ttu-id="e2cfd-161">Строка</span><span class="sxs-lookup"><span data-stu-id="e2cfd-161">String</span></span>|<span data-ttu-id="e2cfd-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e2cfd-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2cfd-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2cfd-164">version</span><span class="sxs-lookup"><span data-stu-id="e2cfd-164">version</span></span>|<span data-ttu-id="e2cfd-165">Int32</span><span class="sxs-lookup"><span data-stu-id="e2cfd-165">Int32</span></span>|<span data-ttu-id="e2cfd-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-166">Version of the device configuration.</span></span> <span data-ttu-id="e2cfd-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2cfd-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2cfd-168">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="e2cfd-168">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="e2cfd-169">Логический</span><span class="sxs-lookup"><span data-stu-id="e2cfd-169">Boolean</span></span>|<span data-ttu-id="e2cfd-170">Указывает, следует ли запретить пользователю добавлять учетные записи электронной почты на устройства, не связанные с учетной записью Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-170">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="e2cfd-171">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="e2cfd-171">applyOnlyToWindows81</span></span>|<span data-ttu-id="e2cfd-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2cfd-172">Boolean</span></span>|<span data-ttu-id="e2cfd-173">Указывает, применяется ли эта политика только к Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-173">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="e2cfd-174">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-174">This property is read-only.</span></span>|
|<span data-ttu-id="e2cfd-175">browserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="e2cfd-175">browserBlockAutofill</span></span>|<span data-ttu-id="e2cfd-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2cfd-176">Boolean</span></span>|<span data-ttu-id="e2cfd-177">Указывает, следует ли заблокировать автозаполнение.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-177">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="e2cfd-178">browserBlockAutomaticDetectionOfIntranetSites</span><span class="sxs-lookup"><span data-stu-id="e2cfd-178">browserBlockAutomaticDetectionOfIntranetSites</span></span>|<span data-ttu-id="e2cfd-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2cfd-179">Boolean</span></span>|<span data-ttu-id="e2cfd-180">Указывает, следует ли заблокировать автоматическое обнаружение сайтов интрасети.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-180">Indicates whether or not to block automatic detection of Intranet sites.</span></span>|
|<span data-ttu-id="e2cfd-181">browserBlockEnterpriseModeAccess</span><span class="sxs-lookup"><span data-stu-id="e2cfd-181">browserBlockEnterpriseModeAccess</span></span>|<span data-ttu-id="e2cfd-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2cfd-182">Boolean</span></span>|<span data-ttu-id="e2cfd-183">Указывает, следует ли заблокировать доступ к корпоративному режиму.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-183">Indicates whether or not to block enterprise mode access.</span></span>|
|<span data-ttu-id="e2cfd-184">browserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="e2cfd-184">browserBlockJavaScript</span></span>|<span data-ttu-id="e2cfd-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2cfd-185">Boolean</span></span>|<span data-ttu-id="e2cfd-186">Указывает, следует ли запретить использование JavaScript.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-186">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="e2cfd-187">browserBlockPlugins</span><span class="sxs-lookup"><span data-stu-id="e2cfd-187">browserBlockPlugins</span></span>|<span data-ttu-id="e2cfd-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2cfd-188">Boolean</span></span>|<span data-ttu-id="e2cfd-189">Указывает, следует ли заблокировать подключаемые модули.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-189">Indicates whether or not to block plug-ins.</span></span>|
|<span data-ttu-id="e2cfd-190">browserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="e2cfd-190">browserBlockPopups</span></span>|<span data-ttu-id="e2cfd-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2cfd-191">Boolean</span></span>|<span data-ttu-id="e2cfd-192">Указывает, следует ли блокировать всплывающие окна.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-192">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="e2cfd-193">browserBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="e2cfd-193">browserBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="e2cfd-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2cfd-194">Boolean</span></span>|<span data-ttu-id="e2cfd-195">Указывает, следует ли запретить пользователю отправлять заголовок DNT.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-195">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="e2cfd-196">browserBlockSingleWordEntryOnIntranetSites</span><span class="sxs-lookup"><span data-stu-id="e2cfd-196">browserBlockSingleWordEntryOnIntranetSites</span></span>|<span data-ttu-id="e2cfd-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2cfd-197">Boolean</span></span>|<span data-ttu-id="e2cfd-198">Указывает, следует ли блокировать переход на сайты интрасети при вводе одного слова.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-198">Indicates whether or not to block a single word entry on Intranet sites.</span></span>|
|<span data-ttu-id="e2cfd-199">browserRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="e2cfd-199">browserRequireSmartScreen</span></span>|<span data-ttu-id="e2cfd-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2cfd-200">Boolean</span></span>|<span data-ttu-id="e2cfd-201">Указывает, обязательно ли использовать фильтр Smart Screen.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-201">Indicates whether or not to require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="e2cfd-202">browserEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="e2cfd-202">browserEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="e2cfd-203">String</span><span class="sxs-lookup"><span data-stu-id="e2cfd-203">String</span></span>|<span data-ttu-id="e2cfd-204">Расположение списка сайтов, запускаемых в корпоративном режиме.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-204">The enterprise mode site list location.</span></span> <span data-ttu-id="e2cfd-205">Это может быть локальный файл, локальная сеть или HTTP-адрес.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-205">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="e2cfd-206">browserInternetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="e2cfd-206">browserInternetSecurityLevel</span></span>|[<span data-ttu-id="e2cfd-207">internetSiteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="e2cfd-207">internetSiteSecurityLevel</span></span>](../resources/intune-deviceconfig-internetsitesecuritylevel.md)|<span data-ttu-id="e2cfd-208">Уровень интернет-безопасности.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-208">The internet security level.</span></span> <span data-ttu-id="e2cfd-209">Возможные значения: `userDefined`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-209">Possible values are: `userDefined`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="e2cfd-210">browserIntranetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="e2cfd-210">browserIntranetSecurityLevel</span></span>|[<span data-ttu-id="e2cfd-211">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="e2cfd-211">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="e2cfd-212">Уровень безопасности интрасети.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-212">The Intranet security level.</span></span> <span data-ttu-id="e2cfd-213">Возможные значения: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-213">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="e2cfd-214">browserLoggingReportLocation</span><span class="sxs-lookup"><span data-stu-id="e2cfd-214">browserLoggingReportLocation</span></span>|<span data-ttu-id="e2cfd-215">String</span><span class="sxs-lookup"><span data-stu-id="e2cfd-215">String</span></span>|<span data-ttu-id="e2cfd-216">Расположение хранения отчетов.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-216">The logging report location.</span></span>|
|<span data-ttu-id="e2cfd-217">browserRequireHighSecurityForRestrictedSites</span><span class="sxs-lookup"><span data-stu-id="e2cfd-217">browserRequireHighSecurityForRestrictedSites</span></span>|<span data-ttu-id="e2cfd-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2cfd-218">Boolean</span></span>|<span data-ttu-id="e2cfd-219">Указывает, обязателен ли высокий уровень безопасности для опасных сайтов.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-219">Indicates whether or not to require high security for restricted sites.</span></span>|
|<span data-ttu-id="e2cfd-220">browserRequireFirewall</span><span class="sxs-lookup"><span data-stu-id="e2cfd-220">browserRequireFirewall</span></span>|<span data-ttu-id="e2cfd-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2cfd-221">Boolean</span></span>|<span data-ttu-id="e2cfd-222">Указывает, обязательно ли использовать брандмауэр.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-222">Indicates whether or not to require a firewall.</span></span>|
|<span data-ttu-id="e2cfd-223">browserRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="e2cfd-223">browserRequireFraudWarning</span></span>|<span data-ttu-id="e2cfd-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2cfd-224">Boolean</span></span>|<span data-ttu-id="e2cfd-225">Указывает, обязательно ли предупреждение о мошенничестве.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-225">Indicates whether or not to require fraud warning.</span></span>|
|<span data-ttu-id="e2cfd-226">browserTrustedSitesSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="e2cfd-226">browserTrustedSitesSecurityLevel</span></span>|[<span data-ttu-id="e2cfd-227">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="e2cfd-227">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="e2cfd-228">Уровень безопасности надежных сайтов.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-228">The trusted sites security level.</span></span> <span data-ttu-id="e2cfd-229">Возможные значения: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-229">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="e2cfd-230">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="e2cfd-230">cellularBlockDataRoaming</span></span>|<span data-ttu-id="e2cfd-231">Логический</span><span class="sxs-lookup"><span data-stu-id="e2cfd-231">Boolean</span></span>|<span data-ttu-id="e2cfd-232">Указывает, следует ли блокировать передачу данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-232">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="e2cfd-233">diagnosticsBlockDataSubmission</span><span class="sxs-lookup"><span data-stu-id="e2cfd-233">diagnosticsBlockDataSubmission</span></span>|<span data-ttu-id="e2cfd-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2cfd-234">Boolean</span></span>|<span data-ttu-id="e2cfd-235">Указывает, следует ли блокировать отправку диагностических данных.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-235">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="e2cfd-236">passwordBlockPicturePasswordAndPin</span><span class="sxs-lookup"><span data-stu-id="e2cfd-236">passwordBlockPicturePasswordAndPin</span></span>|<span data-ttu-id="e2cfd-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2cfd-237">Boolean</span></span>|<span data-ttu-id="e2cfd-238">Указывает, следует ли запретить использование графического пароля и ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-238">Indicates whether or not to Block the user from using a pictures password and pin.</span></span>|
|<span data-ttu-id="e2cfd-239">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="e2cfd-239">passwordExpirationDays</span></span>|<span data-ttu-id="e2cfd-240">Int32</span><span class="sxs-lookup"><span data-stu-id="e2cfd-240">Int32</span></span>|<span data-ttu-id="e2cfd-241">Срок действия пароля (в днях).</span><span class="sxs-lookup"><span data-stu-id="e2cfd-241">Password expiration in days.</span></span>|
|<span data-ttu-id="e2cfd-242">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="e2cfd-242">passwordMinimumLength</span></span>|<span data-ttu-id="e2cfd-243">Int32</span><span class="sxs-lookup"><span data-stu-id="e2cfd-243">Int32</span></span>|<span data-ttu-id="e2cfd-244">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-244">The minimum password length.</span></span>|
|<span data-ttu-id="e2cfd-245">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="e2cfd-245">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="e2cfd-246">Int32</span><span class="sxs-lookup"><span data-stu-id="e2cfd-246">Int32</span></span>|<span data-ttu-id="e2cfd-247">Время бездействия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="e2cfd-247">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="e2cfd-248">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="e2cfd-248">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="e2cfd-249">Int32</span><span class="sxs-lookup"><span data-stu-id="e2cfd-249">Int32</span></span>|<span data-ttu-id="e2cfd-250">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-250">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="e2cfd-251">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="e2cfd-251">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="e2cfd-252">Int32</span><span class="sxs-lookup"><span data-stu-id="e2cfd-252">Int32</span></span>|<span data-ttu-id="e2cfd-253">Количество предыдущих паролей, повторное использование которых следует запретить.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-253">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="e2cfd-254">Допустимые значения: от 0 до 24</span><span class="sxs-lookup"><span data-stu-id="e2cfd-254">Valid values 0 to 24</span></span>|
|<span data-ttu-id="e2cfd-255">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="e2cfd-255">passwordRequiredType</span></span>|[<span data-ttu-id="e2cfd-256">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="e2cfd-256">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="e2cfd-257">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-257">The required password type.</span></span> <span data-ttu-id="e2cfd-258">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-258">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="e2cfd-259">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="e2cfd-259">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="e2cfd-260">Int32</span><span class="sxs-lookup"><span data-stu-id="e2cfd-260">Int32</span></span>|<span data-ttu-id="e2cfd-261">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-261">The number of sign in failures before factory reset.</span></span>|
|<span data-ttu-id="e2cfd-262">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="e2cfd-262">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="e2cfd-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2cfd-263">Boolean</span></span>|<span data-ttu-id="e2cfd-264">Указывает, обязательно ли шифрование данных на мобильном устройстве.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-264">Indicates whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="e2cfd-265">minimumAutoInstallClassification</span><span class="sxs-lookup"><span data-stu-id="e2cfd-265">minimumAutoInstallClassification</span></span>|[<span data-ttu-id="e2cfd-266">updateClassification</span><span class="sxs-lookup"><span data-stu-id="e2cfd-266">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="e2cfd-267">Как минимум обновление классификации для автоматической установки.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-267">The minimum update classification to install automatically.</span></span> <span data-ttu-id="e2cfd-268">Возможные значения: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-268">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="e2cfd-269">updatesMinimumAutoInstallClassification</span><span class="sxs-lookup"><span data-stu-id="e2cfd-269">updatesMinimumAutoInstallClassification</span></span>|[<span data-ttu-id="e2cfd-270">updateClassification</span><span class="sxs-lookup"><span data-stu-id="e2cfd-270">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="e2cfd-271">Как минимум обновление классификации для автоматической установки.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-271">The minimum update classification to install automatically.</span></span> <span data-ttu-id="e2cfd-272">Возможные значения: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-272">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="e2cfd-273">updatesRequireAutomaticUpdates</span><span class="sxs-lookup"><span data-stu-id="e2cfd-273">updatesRequireAutomaticUpdates</span></span>|<span data-ttu-id="e2cfd-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2cfd-274">Boolean</span></span>|<span data-ttu-id="e2cfd-275">Указывает, обязательно ли автоматическое обновление.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-275">Indicates whether or not to require automatic updates.</span></span>|
|<span data-ttu-id="e2cfd-276">userAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="e2cfd-276">userAccountControlSettings</span></span>|[<span data-ttu-id="e2cfd-277">windowsUserAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="e2cfd-277">windowsUserAccountControlSettings</span></span>](../resources/intune-deviceconfig-windowsuseraccountcontrolsettings.md)|<span data-ttu-id="e2cfd-278">Настройки контроля учетных записей.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-278">The user account control settings.</span></span> <span data-ttu-id="e2cfd-279">Возможные значения: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-279">Possible values are: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span></span>|
|<span data-ttu-id="e2cfd-280">workFoldersUrl</span><span class="sxs-lookup"><span data-stu-id="e2cfd-280">workFoldersUrl</span></span>|<span data-ttu-id="e2cfd-281">String</span><span class="sxs-lookup"><span data-stu-id="e2cfd-281">String</span></span>|<span data-ttu-id="e2cfd-282">URL-адрес рабочей папки.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-282">The work folders url.</span></span>|



## <a name="response"></a><span data-ttu-id="e2cfd-283">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2cfd-283">Response</span></span>
<span data-ttu-id="e2cfd-284">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-284">If successful, this method returns a `201 Created` response code and a [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2cfd-285">Пример</span><span class="sxs-lookup"><span data-stu-id="e2cfd-285">Example</span></span>
### <a name="request"></a><span data-ttu-id="e2cfd-286">Запрос</span><span class="sxs-lookup"><span data-stu-id="e2cfd-286">Request</span></span>
<span data-ttu-id="e2cfd-287">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-287">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1988

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="e2cfd-288">Ответ</span><span class="sxs-lookup"><span data-stu-id="e2cfd-288">Response</span></span>
<span data-ttu-id="e2cfd-p121">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





