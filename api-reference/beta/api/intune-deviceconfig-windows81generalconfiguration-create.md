---
title: Создание windows81GeneralConfiguration
description: Создание объекта windows81GeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: fe44f2ec8473c8164157c8da2f4a7354e270e75f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982738"
---
# <a name="create-windows81generalconfiguration"></a><span data-ttu-id="a9435-103">Создание windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="a9435-103">Create windows81GeneralConfiguration</span></span>

> <span data-ttu-id="a9435-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a9435-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a9435-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9435-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a9435-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a9435-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a9435-107">Создание объекта [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a9435-107">Create a new [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a9435-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a9435-108">Prerequisites</span></span>
<span data-ttu-id="a9435-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9435-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9435-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a9435-111">Permission type</span></span>|<span data-ttu-id="a9435-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a9435-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9435-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a9435-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a9435-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9435-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a9435-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a9435-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9435-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9435-116">Not supported.</span></span>|
|<span data-ttu-id="a9435-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a9435-117">Application</span></span>|<span data-ttu-id="a9435-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9435-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9435-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a9435-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a9435-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a9435-120">Request headers</span></span>
|<span data-ttu-id="a9435-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a9435-121">Header</span></span>|<span data-ttu-id="a9435-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a9435-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9435-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9435-123">Authorization</span></span>|<span data-ttu-id="a9435-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a9435-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9435-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a9435-125">Accept</span></span>|<span data-ttu-id="a9435-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a9435-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9435-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a9435-127">Request body</span></span>
<span data-ttu-id="a9435-128">В теле запроса добавьте представление объекта windows81GeneralConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a9435-128">In the request body, supply a JSON representation for the windows81GeneralConfiguration object.</span></span>

<span data-ttu-id="a9435-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта windows81GeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a9435-129">The following table shows the properties that are required when you create the windows81GeneralConfiguration.</span></span>

|<span data-ttu-id="a9435-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a9435-130">Property</span></span>|<span data-ttu-id="a9435-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a9435-131">Type</span></span>|<span data-ttu-id="a9435-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a9435-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9435-133">id</span><span class="sxs-lookup"><span data-stu-id="a9435-133">id</span></span>|<span data-ttu-id="a9435-134">String</span><span class="sxs-lookup"><span data-stu-id="a9435-134">String</span></span>|<span data-ttu-id="a9435-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a9435-135">Key of the entity.</span></span> <span data-ttu-id="a9435-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a9435-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9435-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a9435-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a9435-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9435-138">DateTimeOffset</span></span>|<span data-ttu-id="a9435-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a9435-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a9435-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a9435-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9435-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a9435-141">roleScopeTagIds</span></span>|<span data-ttu-id="a9435-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a9435-142">String collection</span></span>|<span data-ttu-id="a9435-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="a9435-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a9435-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a9435-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9435-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a9435-145">supportsScopeTags</span></span>|<span data-ttu-id="a9435-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9435-146">Boolean</span></span>|<span data-ttu-id="a9435-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="a9435-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a9435-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="a9435-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a9435-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="a9435-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a9435-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a9435-150">This property is read-only.</span></span> <span data-ttu-id="a9435-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a9435-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9435-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a9435-152">createdDateTime</span></span>|<span data-ttu-id="a9435-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9435-153">DateTimeOffset</span></span>|<span data-ttu-id="a9435-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="a9435-154">DateTime the object was created.</span></span> <span data-ttu-id="a9435-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a9435-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9435-156">описание</span><span class="sxs-lookup"><span data-stu-id="a9435-156">description</span></span>|<span data-ttu-id="a9435-157">String</span><span class="sxs-lookup"><span data-stu-id="a9435-157">String</span></span>|<span data-ttu-id="a9435-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a9435-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a9435-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a9435-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9435-160">displayName</span><span class="sxs-lookup"><span data-stu-id="a9435-160">displayName</span></span>|<span data-ttu-id="a9435-161">String</span><span class="sxs-lookup"><span data-stu-id="a9435-161">String</span></span>|<span data-ttu-id="a9435-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a9435-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a9435-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a9435-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9435-164">version</span><span class="sxs-lookup"><span data-stu-id="a9435-164">version</span></span>|<span data-ttu-id="a9435-165">Int32</span><span class="sxs-lookup"><span data-stu-id="a9435-165">Int32</span></span>|<span data-ttu-id="a9435-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a9435-166">Version of the device configuration.</span></span> <span data-ttu-id="a9435-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a9435-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9435-168">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="a9435-168">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="a9435-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9435-169">Boolean</span></span>|<span data-ttu-id="a9435-170">Указывает, следует ли запретить пользователю добавлять учетные записи электронной почты на устройства, не связанные с учетной записью Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="a9435-170">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="a9435-171">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="a9435-171">applyOnlyToWindows81</span></span>|<span data-ttu-id="a9435-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9435-172">Boolean</span></span>|<span data-ttu-id="a9435-173">Указывает, применяется ли эта политика только к Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="a9435-173">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="a9435-174">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a9435-174">This property is read-only.</span></span>|
|<span data-ttu-id="a9435-175">browserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="a9435-175">browserBlockAutofill</span></span>|<span data-ttu-id="a9435-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9435-176">Boolean</span></span>|<span data-ttu-id="a9435-177">Указывает, следует ли заблокировать автозаполнение.</span><span class="sxs-lookup"><span data-stu-id="a9435-177">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="a9435-178">browserBlockAutomaticDetectionOfIntranetSites</span><span class="sxs-lookup"><span data-stu-id="a9435-178">browserBlockAutomaticDetectionOfIntranetSites</span></span>|<span data-ttu-id="a9435-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9435-179">Boolean</span></span>|<span data-ttu-id="a9435-180">Указывает, следует ли заблокировать автоматическое обнаружение сайтов интрасети.</span><span class="sxs-lookup"><span data-stu-id="a9435-180">Indicates whether or not to block automatic detection of Intranet sites.</span></span>|
|<span data-ttu-id="a9435-181">browserBlockEnterpriseModeAccess</span><span class="sxs-lookup"><span data-stu-id="a9435-181">browserBlockEnterpriseModeAccess</span></span>|<span data-ttu-id="a9435-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9435-182">Boolean</span></span>|<span data-ttu-id="a9435-183">Указывает, следует ли заблокировать доступ к корпоративному режиму.</span><span class="sxs-lookup"><span data-stu-id="a9435-183">Indicates whether or not to block enterprise mode access.</span></span>|
|<span data-ttu-id="a9435-184">browserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="a9435-184">browserBlockJavaScript</span></span>|<span data-ttu-id="a9435-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9435-185">Boolean</span></span>|<span data-ttu-id="a9435-186">Указывает, следует ли запретить использование JavaScript.</span><span class="sxs-lookup"><span data-stu-id="a9435-186">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="a9435-187">browserBlockPlugins</span><span class="sxs-lookup"><span data-stu-id="a9435-187">browserBlockPlugins</span></span>|<span data-ttu-id="a9435-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9435-188">Boolean</span></span>|<span data-ttu-id="a9435-189">Указывает, следует ли заблокировать подключаемые модули.</span><span class="sxs-lookup"><span data-stu-id="a9435-189">Indicates whether or not to block plug-ins.</span></span>|
|<span data-ttu-id="a9435-190">browserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="a9435-190">browserBlockPopups</span></span>|<span data-ttu-id="a9435-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9435-191">Boolean</span></span>|<span data-ttu-id="a9435-192">Указывает, следует ли блокировать всплывающие окна.</span><span class="sxs-lookup"><span data-stu-id="a9435-192">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="a9435-193">browserBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="a9435-193">browserBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="a9435-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9435-194">Boolean</span></span>|<span data-ttu-id="a9435-195">Указывает, следует ли запретить пользователю отправлять заголовок DNT.</span><span class="sxs-lookup"><span data-stu-id="a9435-195">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="a9435-196">browserBlockSingleWordEntryOnIntranetSites</span><span class="sxs-lookup"><span data-stu-id="a9435-196">browserBlockSingleWordEntryOnIntranetSites</span></span>|<span data-ttu-id="a9435-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9435-197">Boolean</span></span>|<span data-ttu-id="a9435-198">Указывает, следует ли блокировать переход на сайты интрасети при вводе одного слова.</span><span class="sxs-lookup"><span data-stu-id="a9435-198">Indicates whether or not to block a single word entry on Intranet sites.</span></span>|
|<span data-ttu-id="a9435-199">browserRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="a9435-199">browserRequireSmartScreen</span></span>|<span data-ttu-id="a9435-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9435-200">Boolean</span></span>|<span data-ttu-id="a9435-201">Указывает, обязательно ли использовать фильтр Smart Screen.</span><span class="sxs-lookup"><span data-stu-id="a9435-201">Indicates whether or not to require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="a9435-202">browserEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="a9435-202">browserEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="a9435-203">String</span><span class="sxs-lookup"><span data-stu-id="a9435-203">String</span></span>|<span data-ttu-id="a9435-204">Расположение списка сайтов, запускаемых в корпоративном режиме.</span><span class="sxs-lookup"><span data-stu-id="a9435-204">The enterprise mode site list location.</span></span> <span data-ttu-id="a9435-205">Это может быть локальный файл, локальная сеть или HTTP-адрес.</span><span class="sxs-lookup"><span data-stu-id="a9435-205">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="a9435-206">browserInternetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="a9435-206">browserInternetSecurityLevel</span></span>|[<span data-ttu-id="a9435-207">internetSiteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="a9435-207">internetSiteSecurityLevel</span></span>](../resources/intune-deviceconfig-internetsitesecuritylevel.md)|<span data-ttu-id="a9435-208">Уровень интернет-безопасности.</span><span class="sxs-lookup"><span data-stu-id="a9435-208">The internet security level.</span></span> <span data-ttu-id="a9435-209">Возможные значения: `userDefined`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="a9435-209">Possible values are: `userDefined`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="a9435-210">browserIntranetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="a9435-210">browserIntranetSecurityLevel</span></span>|[<span data-ttu-id="a9435-211">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="a9435-211">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="a9435-212">Уровень безопасности интрасети.</span><span class="sxs-lookup"><span data-stu-id="a9435-212">The Intranet security level.</span></span> <span data-ttu-id="a9435-213">Возможные значения: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="a9435-213">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="a9435-214">browserLoggingReportLocation</span><span class="sxs-lookup"><span data-stu-id="a9435-214">browserLoggingReportLocation</span></span>|<span data-ttu-id="a9435-215">String</span><span class="sxs-lookup"><span data-stu-id="a9435-215">String</span></span>|<span data-ttu-id="a9435-216">Расположение хранения отчетов.</span><span class="sxs-lookup"><span data-stu-id="a9435-216">The logging report location.</span></span>|
|<span data-ttu-id="a9435-217">browserRequireHighSecurityForRestrictedSites</span><span class="sxs-lookup"><span data-stu-id="a9435-217">browserRequireHighSecurityForRestrictedSites</span></span>|<span data-ttu-id="a9435-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9435-218">Boolean</span></span>|<span data-ttu-id="a9435-219">Указывает, обязателен ли высокий уровень безопасности для опасных сайтов.</span><span class="sxs-lookup"><span data-stu-id="a9435-219">Indicates whether or not to require high security for restricted sites.</span></span>|
|<span data-ttu-id="a9435-220">browserRequireFirewall</span><span class="sxs-lookup"><span data-stu-id="a9435-220">browserRequireFirewall</span></span>|<span data-ttu-id="a9435-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9435-221">Boolean</span></span>|<span data-ttu-id="a9435-222">Указывает, обязательно ли использовать брандмауэр.</span><span class="sxs-lookup"><span data-stu-id="a9435-222">Indicates whether or not to require a firewall.</span></span>|
|<span data-ttu-id="a9435-223">browserRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="a9435-223">browserRequireFraudWarning</span></span>|<span data-ttu-id="a9435-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9435-224">Boolean</span></span>|<span data-ttu-id="a9435-225">Указывает, обязательно ли предупреждение о мошенничестве.</span><span class="sxs-lookup"><span data-stu-id="a9435-225">Indicates whether or not to require fraud warning.</span></span>|
|<span data-ttu-id="a9435-226">browserTrustedSitesSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="a9435-226">browserTrustedSitesSecurityLevel</span></span>|[<span data-ttu-id="a9435-227">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="a9435-227">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="a9435-228">Уровень безопасности надежных сайтов.</span><span class="sxs-lookup"><span data-stu-id="a9435-228">The trusted sites security level.</span></span> <span data-ttu-id="a9435-229">Возможные значения: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="a9435-229">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="a9435-230">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="a9435-230">cellularBlockDataRoaming</span></span>|<span data-ttu-id="a9435-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9435-231">Boolean</span></span>|<span data-ttu-id="a9435-232">Указывает, следует ли блокировать передачу данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="a9435-232">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="a9435-233">diagnosticsBlockDataSubmission</span><span class="sxs-lookup"><span data-stu-id="a9435-233">diagnosticsBlockDataSubmission</span></span>|<span data-ttu-id="a9435-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9435-234">Boolean</span></span>|<span data-ttu-id="a9435-235">Указывает, следует ли блокировать отправку диагностических данных.</span><span class="sxs-lookup"><span data-stu-id="a9435-235">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="a9435-236">passwordBlockPicturePasswordAndPin</span><span class="sxs-lookup"><span data-stu-id="a9435-236">passwordBlockPicturePasswordAndPin</span></span>|<span data-ttu-id="a9435-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9435-237">Boolean</span></span>|<span data-ttu-id="a9435-238">Указывает, следует ли запретить использование графического пароля и ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="a9435-238">Indicates whether or not to Block the user from using a pictures password and pin.</span></span>|
|<span data-ttu-id="a9435-239">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="a9435-239">passwordExpirationDays</span></span>|<span data-ttu-id="a9435-240">Int32</span><span class="sxs-lookup"><span data-stu-id="a9435-240">Int32</span></span>|<span data-ttu-id="a9435-241">Срок действия пароля (в днях).</span><span class="sxs-lookup"><span data-stu-id="a9435-241">Password expiration in days.</span></span>|
|<span data-ttu-id="a9435-242">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="a9435-242">passwordMinimumLength</span></span>|<span data-ttu-id="a9435-243">Int32</span><span class="sxs-lookup"><span data-stu-id="a9435-243">Int32</span></span>|<span data-ttu-id="a9435-244">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="a9435-244">The minimum password length.</span></span>|
|<span data-ttu-id="a9435-245">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="a9435-245">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="a9435-246">Int32</span><span class="sxs-lookup"><span data-stu-id="a9435-246">Int32</span></span>|<span data-ttu-id="a9435-247">Время бездействия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="a9435-247">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="a9435-248">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="a9435-248">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="a9435-249">Int32</span><span class="sxs-lookup"><span data-stu-id="a9435-249">Int32</span></span>|<span data-ttu-id="a9435-250">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="a9435-250">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="a9435-251">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="a9435-251">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="a9435-252">Int32</span><span class="sxs-lookup"><span data-stu-id="a9435-252">Int32</span></span>|<span data-ttu-id="a9435-253">Количество предыдущих паролей, повторное использование которых следует запретить.</span><span class="sxs-lookup"><span data-stu-id="a9435-253">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="a9435-254">Допустимые значения: от 0 до 24</span><span class="sxs-lookup"><span data-stu-id="a9435-254">Valid values 0 to 24</span></span>|
|<span data-ttu-id="a9435-255">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="a9435-255">passwordRequiredType</span></span>|[<span data-ttu-id="a9435-256">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="a9435-256">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="a9435-257">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="a9435-257">The required password type.</span></span> <span data-ttu-id="a9435-258">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="a9435-258">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="a9435-259">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="a9435-259">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="a9435-260">Int32</span><span class="sxs-lookup"><span data-stu-id="a9435-260">Int32</span></span>|<span data-ttu-id="a9435-261">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="a9435-261">The number of sign in failures before factory reset.</span></span>|
|<span data-ttu-id="a9435-262">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="a9435-262">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="a9435-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9435-263">Boolean</span></span>|<span data-ttu-id="a9435-264">Указывает, обязательно ли шифрование данных на мобильном устройстве.</span><span class="sxs-lookup"><span data-stu-id="a9435-264">Indicates whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="a9435-265">minimumAutoInstallClassification</span><span class="sxs-lookup"><span data-stu-id="a9435-265">minimumAutoInstallClassification</span></span>|[<span data-ttu-id="a9435-266">updateClassification</span><span class="sxs-lookup"><span data-stu-id="a9435-266">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="a9435-267">Как минимум обновление классификации для автоматической установки.</span><span class="sxs-lookup"><span data-stu-id="a9435-267">The minimum update classification to install automatically.</span></span> <span data-ttu-id="a9435-268">Возможные значения: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span><span class="sxs-lookup"><span data-stu-id="a9435-268">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="a9435-269">updatesMinimumAutoInstallClassification</span><span class="sxs-lookup"><span data-stu-id="a9435-269">updatesMinimumAutoInstallClassification</span></span>|[<span data-ttu-id="a9435-270">updateClassification</span><span class="sxs-lookup"><span data-stu-id="a9435-270">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="a9435-271">Как минимум обновление классификации для автоматической установки.</span><span class="sxs-lookup"><span data-stu-id="a9435-271">The minimum update classification to install automatically.</span></span> <span data-ttu-id="a9435-272">Возможные значения: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span><span class="sxs-lookup"><span data-stu-id="a9435-272">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="a9435-273">updatesRequireAutomaticUpdates</span><span class="sxs-lookup"><span data-stu-id="a9435-273">updatesRequireAutomaticUpdates</span></span>|<span data-ttu-id="a9435-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9435-274">Boolean</span></span>|<span data-ttu-id="a9435-275">Указывает, обязательно ли автоматическое обновление.</span><span class="sxs-lookup"><span data-stu-id="a9435-275">Indicates whether or not to require automatic updates.</span></span>|
|<span data-ttu-id="a9435-276">userAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="a9435-276">userAccountControlSettings</span></span>|[<span data-ttu-id="a9435-277">windowsUserAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="a9435-277">windowsUserAccountControlSettings</span></span>](../resources/intune-deviceconfig-windowsuseraccountcontrolsettings.md)|<span data-ttu-id="a9435-278">Настройки контроля учетных записей.</span><span class="sxs-lookup"><span data-stu-id="a9435-278">The user account control settings.</span></span> <span data-ttu-id="a9435-279">Возможные значения: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span><span class="sxs-lookup"><span data-stu-id="a9435-279">Possible values are: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span></span>|
|<span data-ttu-id="a9435-280">workFoldersUrl</span><span class="sxs-lookup"><span data-stu-id="a9435-280">workFoldersUrl</span></span>|<span data-ttu-id="a9435-281">String</span><span class="sxs-lookup"><span data-stu-id="a9435-281">String</span></span>|<span data-ttu-id="a9435-282">URL-адрес рабочей папки.</span><span class="sxs-lookup"><span data-stu-id="a9435-282">The work folders url.</span></span>|



## <a name="response"></a><span data-ttu-id="a9435-283">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9435-283">Response</span></span>
<span data-ttu-id="a9435-284">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a9435-284">If successful, this method returns a `201 Created` response code and a [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9435-285">Пример</span><span class="sxs-lookup"><span data-stu-id="a9435-285">Example</span></span>
### <a name="request"></a><span data-ttu-id="a9435-286">Запрос</span><span class="sxs-lookup"><span data-stu-id="a9435-286">Request</span></span>
<span data-ttu-id="a9435-287">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a9435-287">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a9435-288">Ответ</span><span class="sxs-lookup"><span data-stu-id="a9435-288">Response</span></span>
<span data-ttu-id="a9435-p121">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a9435-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





