---
title: Создание windowsIdentityProtectionConfiguration
description: Создание нового объекта windowsIdentityProtectionConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: be9c6ad30eb869bfd47b20863fc41e103eabe1c2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408994"
---
# <a name="create-windowsidentityprotectionconfiguration"></a><span data-ttu-id="fb47f-103">Создание windowsIdentityProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="fb47f-103">Create windowsIdentityProtectionConfiguration</span></span>

> <span data-ttu-id="fb47f-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fb47f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fb47f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb47f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fb47f-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fb47f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb47f-107">Создание нового объекта [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="fb47f-107">Create a new [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fb47f-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="fb47f-108">Prerequisites</span></span>
<span data-ttu-id="fb47f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="fb47f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fb47f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fb47f-111">Permission type</span></span>|<span data-ttu-id="fb47f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fb47f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb47f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fb47f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fb47f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb47f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fb47f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fb47f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb47f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb47f-116">Not supported.</span></span>|
|<span data-ttu-id="fb47f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fb47f-117">Application</span></span>|<span data-ttu-id="fb47f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb47f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb47f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fb47f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="fb47f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fb47f-120">Request headers</span></span>
|<span data-ttu-id="fb47f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fb47f-121">Header</span></span>|<span data-ttu-id="fb47f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fb47f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb47f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb47f-123">Authorization</span></span>|<span data-ttu-id="fb47f-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="fb47f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb47f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fb47f-125">Accept</span></span>|<span data-ttu-id="fb47f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fb47f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb47f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fb47f-127">Request body</span></span>
<span data-ttu-id="fb47f-128">В тексте запроса укажите представление JSON для объекта windowsIdentityProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="fb47f-128">In the request body, supply a JSON representation for the windowsIdentityProtectionConfiguration object.</span></span>

<span data-ttu-id="fb47f-129">В следующей таблице показаны свойства, которые необходимы для создания windowsIdentityProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="fb47f-129">The following table shows the properties that are required when you create the windowsIdentityProtectionConfiguration.</span></span>

|<span data-ttu-id="fb47f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fb47f-130">Property</span></span>|<span data-ttu-id="fb47f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fb47f-131">Type</span></span>|<span data-ttu-id="fb47f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fb47f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb47f-133">id</span><span class="sxs-lookup"><span data-stu-id="fb47f-133">id</span></span>|<span data-ttu-id="fb47f-134">String</span><span class="sxs-lookup"><span data-stu-id="fb47f-134">String</span></span>|<span data-ttu-id="fb47f-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fb47f-135">Key of the entity.</span></span> <span data-ttu-id="fb47f-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fb47f-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb47f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fb47f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="fb47f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb47f-138">DateTimeOffset</span></span>|<span data-ttu-id="fb47f-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="fb47f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="fb47f-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fb47f-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb47f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fb47f-141">roleScopeTagIds</span></span>|<span data-ttu-id="fb47f-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fb47f-142">String collection</span></span>|<span data-ttu-id="fb47f-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="fb47f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="fb47f-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fb47f-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb47f-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="fb47f-145">supportsScopeTags</span></span>|<span data-ttu-id="fb47f-146">Логический</span><span class="sxs-lookup"><span data-stu-id="fb47f-146">Boolean</span></span>|<span data-ttu-id="fb47f-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="fb47f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="fb47f-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="fb47f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="fb47f-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="fb47f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="fb47f-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fb47f-150">This property is read-only.</span></span> <span data-ttu-id="fb47f-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fb47f-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb47f-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fb47f-152">createdDateTime</span></span>|<span data-ttu-id="fb47f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb47f-153">DateTimeOffset</span></span>|<span data-ttu-id="fb47f-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="fb47f-154">DateTime the object was created.</span></span> <span data-ttu-id="fb47f-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fb47f-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb47f-156">description</span><span class="sxs-lookup"><span data-stu-id="fb47f-156">description</span></span>|<span data-ttu-id="fb47f-157">String</span><span class="sxs-lookup"><span data-stu-id="fb47f-157">String</span></span>|<span data-ttu-id="fb47f-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fb47f-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fb47f-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fb47f-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb47f-160">displayName</span><span class="sxs-lookup"><span data-stu-id="fb47f-160">displayName</span></span>|<span data-ttu-id="fb47f-161">String</span><span class="sxs-lookup"><span data-stu-id="fb47f-161">String</span></span>|<span data-ttu-id="fb47f-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fb47f-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fb47f-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fb47f-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb47f-164">version</span><span class="sxs-lookup"><span data-stu-id="fb47f-164">version</span></span>|<span data-ttu-id="fb47f-165">Int32</span><span class="sxs-lookup"><span data-stu-id="fb47f-165">Int32</span></span>|<span data-ttu-id="fb47f-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fb47f-166">Version of the device configuration.</span></span> <span data-ttu-id="fb47f-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fb47f-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb47f-168">useSecurityKeyForSignin</span><span class="sxs-lookup"><span data-stu-id="fb47f-168">useSecurityKeyForSignin</span></span>|<span data-ttu-id="fb47f-169">Логический</span><span class="sxs-lookup"><span data-stu-id="fb47f-169">Boolean</span></span>|<span data-ttu-id="fb47f-170">Логическое значение, используемое для включения Windows Hello безопасности ключа в виде учетные данные входа в систему.</span><span class="sxs-lookup"><span data-stu-id="fb47f-170">Boolean value used to enable the Windows Hello security key as a logon credential.</span></span>|
|<span data-ttu-id="fb47f-171">enhancedAntiSpoofingForFacialFeaturesEnabled</span><span class="sxs-lookup"><span data-stu-id="fb47f-171">enhancedAntiSpoofingForFacialFeaturesEnabled</span></span>|<span data-ttu-id="fb47f-172">Логический</span><span class="sxs-lookup"><span data-stu-id="fb47f-172">Boolean</span></span>|<span data-ttu-id="fb47f-173">Логическое значение, используемое для включения усовершенствованные спуфинг anti для распознавания лица компонента на Windows Hello лицевой проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="fb47f-173">Boolean value used to enable enhanced anti-spoofing for facial feature recognition on Windows Hello face authentication.</span></span>|
|<span data-ttu-id="fb47f-174">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="fb47f-174">pinMinimumLength</span></span>|<span data-ttu-id="fb47f-175">Int32</span><span class="sxs-lookup"><span data-stu-id="fb47f-175">Int32</span></span>|<span data-ttu-id="fb47f-176">Целое значение, задает минимальное число символов, необходимое для Windows Hello для бизнеса ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="fb47f-176">Integer value that sets the minimum number of characters required for the Windows Hello for Business PIN.</span></span> <span data-ttu-id="fb47f-177">Допустимые значения: 4 до 127 включительно и меньше или равно значению набор для максимального ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="fb47f-177">Valid values are 4 to 127 inclusive and less than or equal to the value set for the maximum PIN.</span></span> <span data-ttu-id="fb47f-178">Допустимые значения 4 до 127</span><span class="sxs-lookup"><span data-stu-id="fb47f-178">Valid values 4 to 127</span></span>|
|<span data-ttu-id="fb47f-179">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="fb47f-179">pinMaximumLength</span></span>|<span data-ttu-id="fb47f-180">Int32</span><span class="sxs-lookup"><span data-stu-id="fb47f-180">Int32</span></span>|<span data-ttu-id="fb47f-181">Целое значение, которое задает максимальное число символов, допустимое для работы ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="fb47f-181">Integer value that sets the maximum number of characters allowed for the work PIN.</span></span> <span data-ttu-id="fb47f-182">Допустимые значения: 4 до 127 включительно и больше или равно значение, установленное для минимальные ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="fb47f-182">Valid values are 4 to 127 inclusive and greater than or equal to the value set for the minimum PIN.</span></span> <span data-ttu-id="fb47f-183">Допустимые значения 4 до 127</span><span class="sxs-lookup"><span data-stu-id="fb47f-183">Valid values 4 to 127</span></span>|
|<span data-ttu-id="fb47f-184">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="fb47f-184">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="fb47f-185">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="fb47f-185">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="fb47f-186">Это значение настраивается использование прописные буквы в Windows Hello для бизнеса ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="fb47f-186">This value configures the use of uppercase characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="fb47f-187">Возможные значения: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="fb47f-187">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="fb47f-188">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="fb47f-188">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="fb47f-189">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="fb47f-189">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="fb47f-190">Это значение настраивается использование строчные буквы в Windows Hello для бизнеса ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="fb47f-190">This value configures the use of lowercase characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="fb47f-191">Возможные значения: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="fb47f-191">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="fb47f-192">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="fb47f-192">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="fb47f-193">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="fb47f-193">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="fb47f-194">Определяет возможность использования специальных символов в Windows Hello для бизнеса ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="fb47f-194">Controls the ability to use special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="fb47f-195">Возможные значения: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="fb47f-195">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="fb47f-196">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="fb47f-196">pinExpirationInDays</span></span>|<span data-ttu-id="fb47f-197">Int32</span><span class="sxs-lookup"><span data-stu-id="fb47f-197">Int32</span></span>|<span data-ttu-id="fb47f-198">Целое значение указывает период (в днях), можно ли использовать ПИН-код до его обязательного изменения пользователем.</span><span class="sxs-lookup"><span data-stu-id="fb47f-198">Integer value specifies the period (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="fb47f-199">Допустимые значения: 0 для 730 включительно.</span><span class="sxs-lookup"><span data-stu-id="fb47f-199">Valid values are 0 to 730 inclusive.</span></span> <span data-ttu-id="fb47f-200">Допустимые значения: от 0 до 730.</span><span class="sxs-lookup"><span data-stu-id="fb47f-200">Valid values 0 to 730</span></span>|
|<span data-ttu-id="fb47f-201">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="fb47f-201">pinPreviousBlockCount</span></span>|<span data-ttu-id="fb47f-202">Int32</span><span class="sxs-lookup"><span data-stu-id="fb47f-202">Int32</span></span>|<span data-ttu-id="fb47f-203">Определяет возможность запретить пользователям с помощью предыдущих ПИН-коды.</span><span class="sxs-lookup"><span data-stu-id="fb47f-203">Controls the ability to prevent users from using past PINs.</span></span> <span data-ttu-id="fb47f-204">Это должно иметь значение от 0 до 50, включительно, и текущий ПИН-код пользователя включается в этот счетчик.</span><span class="sxs-lookup"><span data-stu-id="fb47f-204">This must be set between 0 and 50, inclusive, and the current PIN of the user is included in that count.</span></span> <span data-ttu-id="fb47f-205">Если значение 0, предыдущих ПИН-коды не сохраняются.</span><span class="sxs-lookup"><span data-stu-id="fb47f-205">If set to 0, previous PINs are not stored.</span></span> <span data-ttu-id="fb47f-206">ПИН-код не сохраняется через ПИН-код сбросить.</span><span class="sxs-lookup"><span data-stu-id="fb47f-206">PIN history is not preserved through a PIN reset.</span></span> <span data-ttu-id="fb47f-207">Допустимые значения: от 0 до 50.</span><span class="sxs-lookup"><span data-stu-id="fb47f-207">Valid values 0 to 50</span></span>|
|<span data-ttu-id="fb47f-208">pinRecoveryEnabled</span><span class="sxs-lookup"><span data-stu-id="fb47f-208">pinRecoveryEnabled</span></span>|<span data-ttu-id="fb47f-209">Логический</span><span class="sxs-lookup"><span data-stu-id="fb47f-209">Boolean</span></span>|<span data-ttu-id="fb47f-210">Логическое значение, которое позволяет пользователям изменять свой ПИН-код с помощью Windows Hello для восстановления службы Business ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="fb47f-210">Boolean value that enables a user to change their PIN by using the Windows Hello for Business PIN recovery service.</span></span>|
|<span data-ttu-id="fb47f-211">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="fb47f-211">securityDeviceRequired</span></span>|<span data-ttu-id="fb47f-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb47f-212">Boolean</span></span>|<span data-ttu-id="fb47f-213">Определяет необходимость доверенного платформы модуля (TPM) для подготовки Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="fb47f-213">Controls whether to require a Trusted Platform Module (TPM) for provisioning Windows Hello for Business.</span></span> <span data-ttu-id="fb47f-214">TPM обеспечивает дополнительных преимуществ для безопасности, в том, что данные, хранящиеся на его нельзя использовать на других устройствах.</span><span class="sxs-lookup"><span data-stu-id="fb47f-214">A TPM provides an additional security benefit in that data stored on it cannot be used on other devices.</span></span> <span data-ttu-id="fb47f-215">Если задано значение False, все устройства можно подготовить Windows Hello для бизнеса даже в том случае, если не могут использоваться TPM.</span><span class="sxs-lookup"><span data-stu-id="fb47f-215">If set to False, all devices can provision Windows Hello for Business even if there is not a usable TPM.</span></span>|
|<span data-ttu-id="fb47f-216">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="fb47f-216">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="fb47f-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb47f-217">Boolean</span></span>|<span data-ttu-id="fb47f-218">Управляет Биометрическая жестов, таких как начертание и отпечаток, как альтернативы Windows Hello для бизнеса ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="fb47f-218">Controls the use of biometric gestures, such as face and fingerprint, as an alternative to the Windows Hello for Business PIN.</span></span>  <span data-ttu-id="fb47f-219">Если параметр имеет значение False, Биометрическая жесты не разрешены.</span><span class="sxs-lookup"><span data-stu-id="fb47f-219">If set to False, biometric gestures are not allowed.</span></span> <span data-ttu-id="fb47f-220">Пользователи по-прежнему необходимо настроить ПИН-код для резервного копирования в случае сбоев.</span><span class="sxs-lookup"><span data-stu-id="fb47f-220">Users must still configure a PIN as a backup in case of failures.</span></span>|
|<span data-ttu-id="fb47f-221">useCertificatesForOnPremisesAuthEnabled</span><span class="sxs-lookup"><span data-stu-id="fb47f-221">useCertificatesForOnPremisesAuthEnabled</span></span>|<span data-ttu-id="fb47f-222">Логический</span><span class="sxs-lookup"><span data-stu-id="fb47f-222">Boolean</span></span>|<span data-ttu-id="fb47f-223">Логическое значение, включающее Windows Hello для бизнеса для использования сертификатов для проверки подлинности локальным ресурсам.</span><span class="sxs-lookup"><span data-stu-id="fb47f-223">Boolean value that enables Windows Hello for Business to use certificates to authenticate on-premise resources.</span></span>|
|<span data-ttu-id="fb47f-224">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="fb47f-224">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="fb47f-225">Логический</span><span class="sxs-lookup"><span data-stu-id="fb47f-225">Boolean</span></span>|<span data-ttu-id="fb47f-226">Логическое значение, которое блокирует Windows Hello для бизнеса, как метод для входа в Windows.</span><span class="sxs-lookup"><span data-stu-id="fb47f-226">Boolean value that blocks Windows Hello for Business as a method for signing into Windows.</span></span>|



## <a name="response"></a><span data-ttu-id="fb47f-227">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb47f-227">Response</span></span>
<span data-ttu-id="fb47f-228">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="fb47f-228">If successful, this method returns a `201 Created` response code and a [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb47f-229">Пример</span><span class="sxs-lookup"><span data-stu-id="fb47f-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="fb47f-230">Запрос</span><span class="sxs-lookup"><span data-stu-id="fb47f-230">Request</span></span>
<span data-ttu-id="fb47f-231">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fb47f-231">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 810

{
  "@odata.type": "#microsoft.graph.windowsIdentityProtectionConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "useSecurityKeyForSignin": true,
  "enhancedAntiSpoofingForFacialFeaturesEnabled": true,
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "pinExpirationInDays": 3,
  "pinPreviousBlockCount": 5,
  "pinRecoveryEnabled": true,
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "useCertificatesForOnPremisesAuthEnabled": true,
  "windowsHelloForBusinessBlocked": true
}
```

### <a name="response"></a><span data-ttu-id="fb47f-232">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb47f-232">Response</span></span>
<span data-ttu-id="fb47f-p120">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fb47f-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 982

{
  "@odata.type": "#microsoft.graph.windowsIdentityProtectionConfiguration",
  "id": "b2e64303-4303-b2e6-0343-e6b20343e6b2",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "useSecurityKeyForSignin": true,
  "enhancedAntiSpoofingForFacialFeaturesEnabled": true,
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "pinExpirationInDays": 3,
  "pinPreviousBlockCount": 5,
  "pinRecoveryEnabled": true,
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "useCertificatesForOnPremisesAuthEnabled": true,
  "windowsHelloForBusinessBlocked": true
}
```




