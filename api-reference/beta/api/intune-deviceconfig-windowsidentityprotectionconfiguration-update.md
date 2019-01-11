---
title: Обновление windowsIdentityProtectionConfiguration
description: Обновление свойства объекта windowsIdentityProtectionConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 77f93941d7b8eb3153d376eb3d3314842672e10a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27881587"
---
# <a name="update-windowsidentityprotectionconfiguration"></a><span data-ttu-id="5b47a-103">Обновление windowsIdentityProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="5b47a-103">Update windowsIdentityProtectionConfiguration</span></span>

> <span data-ttu-id="5b47a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5b47a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5b47a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b47a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5b47a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5b47a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5b47a-107">Обновление свойства объекта [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="5b47a-107">Update the properties of a [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5b47a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5b47a-108">Prerequisites</span></span>
<span data-ttu-id="5b47a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b47a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b47a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5b47a-111">Permission type</span></span>|<span data-ttu-id="5b47a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5b47a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b47a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b47a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5b47a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b47a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5b47a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b47a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b47a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b47a-116">Not supported.</span></span>|
|<span data-ttu-id="5b47a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5b47a-117">Application</span></span>|<span data-ttu-id="5b47a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b47a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b47a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b47a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="5b47a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5b47a-120">Request headers</span></span>
|<span data-ttu-id="5b47a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5b47a-121">Header</span></span>|<span data-ttu-id="5b47a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5b47a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b47a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b47a-123">Authorization</span></span>|<span data-ttu-id="5b47a-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="5b47a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b47a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5b47a-125">Accept</span></span>|<span data-ttu-id="5b47a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5b47a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b47a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5b47a-127">Request body</span></span>
<span data-ttu-id="5b47a-128">В тексте запроса укажите представление JSON для объекта [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="5b47a-128">In the request body, supply a JSON representation for the [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="5b47a-129">В следующей таблице показаны свойства, которые необходимы для создания [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b47a-129">The following table shows the properties that are required when you create the [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md).</span></span>

|<span data-ttu-id="5b47a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5b47a-130">Property</span></span>|<span data-ttu-id="5b47a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5b47a-131">Type</span></span>|<span data-ttu-id="5b47a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5b47a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b47a-133">id</span><span class="sxs-lookup"><span data-stu-id="5b47a-133">id</span></span>|<span data-ttu-id="5b47a-134">Строка</span><span class="sxs-lookup"><span data-stu-id="5b47a-134">String</span></span>|<span data-ttu-id="5b47a-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5b47a-135">Key of the entity.</span></span> <span data-ttu-id="5b47a-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b47a-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b47a-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5b47a-137">lastModifiedDateTime</span></span>|<span data-ttu-id="5b47a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b47a-138">DateTimeOffset</span></span>|<span data-ttu-id="5b47a-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="5b47a-139">DateTime the object was last modified.</span></span> <span data-ttu-id="5b47a-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b47a-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b47a-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5b47a-141">roleScopeTagIds</span></span>|<span data-ttu-id="5b47a-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5b47a-142">String collection</span></span>|<span data-ttu-id="5b47a-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="5b47a-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5b47a-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b47a-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b47a-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="5b47a-145">supportsScopeTags</span></span>|<span data-ttu-id="5b47a-146">Логический</span><span class="sxs-lookup"><span data-stu-id="5b47a-146">Boolean</span></span>|<span data-ttu-id="5b47a-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="5b47a-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5b47a-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="5b47a-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5b47a-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="5b47a-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5b47a-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5b47a-150">This property is read-only.</span></span> <span data-ttu-id="5b47a-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b47a-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b47a-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5b47a-152">createdDateTime</span></span>|<span data-ttu-id="5b47a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b47a-153">DateTimeOffset</span></span>|<span data-ttu-id="5b47a-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="5b47a-154">DateTime the object was created.</span></span> <span data-ttu-id="5b47a-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b47a-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b47a-156">описание</span><span class="sxs-lookup"><span data-stu-id="5b47a-156">description</span></span>|<span data-ttu-id="5b47a-157">Строка</span><span class="sxs-lookup"><span data-stu-id="5b47a-157">String</span></span>|<span data-ttu-id="5b47a-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5b47a-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5b47a-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b47a-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b47a-160">displayName</span><span class="sxs-lookup"><span data-stu-id="5b47a-160">displayName</span></span>|<span data-ttu-id="5b47a-161">Строка</span><span class="sxs-lookup"><span data-stu-id="5b47a-161">String</span></span>|<span data-ttu-id="5b47a-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5b47a-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5b47a-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b47a-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b47a-164">version</span><span class="sxs-lookup"><span data-stu-id="5b47a-164">version</span></span>|<span data-ttu-id="5b47a-165">Int32</span><span class="sxs-lookup"><span data-stu-id="5b47a-165">Int32</span></span>|<span data-ttu-id="5b47a-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5b47a-166">Version of the device configuration.</span></span> <span data-ttu-id="5b47a-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b47a-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b47a-168">enhancedAntiSpoofingForFacialFeaturesEnabled</span><span class="sxs-lookup"><span data-stu-id="5b47a-168">enhancedAntiSpoofingForFacialFeaturesEnabled</span></span>|<span data-ttu-id="5b47a-169">Логический</span><span class="sxs-lookup"><span data-stu-id="5b47a-169">Boolean</span></span>|<span data-ttu-id="5b47a-170">Логическое значение, используемое для включения усовершенствованные спуфинг anti для распознавания лица компонента на Windows Hello лицевой проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="5b47a-170">Boolean value used to enable enhanced anti-spoofing for facial feature recognition on Windows Hello face authentication.</span></span>|
|<span data-ttu-id="5b47a-171">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="5b47a-171">pinMinimumLength</span></span>|<span data-ttu-id="5b47a-172">Int32</span><span class="sxs-lookup"><span data-stu-id="5b47a-172">Int32</span></span>|<span data-ttu-id="5b47a-173">Целое значение, задает минимальное число символов, необходимое для Windows Hello для бизнеса ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="5b47a-173">Integer value that sets the minimum number of characters required for the Windows Hello for Business PIN.</span></span> <span data-ttu-id="5b47a-174">Допустимые значения: 4 до 127 включительно и меньше или равно значению набор для максимального ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="5b47a-174">Valid values are 4 to 127 inclusive and less than or equal to the value set for the maximum PIN.</span></span> <span data-ttu-id="5b47a-175">Допустимые значения 4 до 127</span><span class="sxs-lookup"><span data-stu-id="5b47a-175">Valid values 4 to 127</span></span>|
|<span data-ttu-id="5b47a-176">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="5b47a-176">pinMaximumLength</span></span>|<span data-ttu-id="5b47a-177">Int32</span><span class="sxs-lookup"><span data-stu-id="5b47a-177">Int32</span></span>|<span data-ttu-id="5b47a-178">Целое значение, которое задает максимальное число символов, допустимое для работы ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="5b47a-178">Integer value that sets the maximum number of characters allowed for the work PIN.</span></span> <span data-ttu-id="5b47a-179">Допустимые значения: 4 до 127 включительно и больше или равно значение, установленное для минимальные ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="5b47a-179">Valid values are 4 to 127 inclusive and greater than or equal to the value set for the minimum PIN.</span></span> <span data-ttu-id="5b47a-180">Допустимые значения 4 до 127</span><span class="sxs-lookup"><span data-stu-id="5b47a-180">Valid values 4 to 127</span></span>|
|<span data-ttu-id="5b47a-181">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="5b47a-181">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="5b47a-182">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="5b47a-182">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="5b47a-183">Это значение настраивается использование прописные буквы в Windows Hello для бизнеса ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="5b47a-183">This value configures the use of uppercase characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="5b47a-184">Возможные значения: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="5b47a-184">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="5b47a-185">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="5b47a-185">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="5b47a-186">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="5b47a-186">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="5b47a-187">Это значение настраивается использование строчные буквы в Windows Hello для бизнеса ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="5b47a-187">This value configures the use of lowercase characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="5b47a-188">Возможные значения: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="5b47a-188">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="5b47a-189">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="5b47a-189">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="5b47a-190">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="5b47a-190">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="5b47a-191">Определяет возможность использования специальных символов в Windows Hello для бизнеса ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="5b47a-191">Controls the ability to use special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="5b47a-192">Возможные значения: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="5b47a-192">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="5b47a-193">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="5b47a-193">pinExpirationInDays</span></span>|<span data-ttu-id="5b47a-194">Int32</span><span class="sxs-lookup"><span data-stu-id="5b47a-194">Int32</span></span>|<span data-ttu-id="5b47a-195">Целое значение указывает период (в днях), можно ли использовать ПИН-код до его обязательного изменения пользователем.</span><span class="sxs-lookup"><span data-stu-id="5b47a-195">Integer value specifies the period (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="5b47a-196">Допустимые значения: 0 для 730 включительно.</span><span class="sxs-lookup"><span data-stu-id="5b47a-196">Valid values are 0 to 730 inclusive.</span></span> <span data-ttu-id="5b47a-197">Допустимые значения: от 0 до 730.</span><span class="sxs-lookup"><span data-stu-id="5b47a-197">Valid values 0 to 730</span></span>|
|<span data-ttu-id="5b47a-198">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="5b47a-198">pinPreviousBlockCount</span></span>|<span data-ttu-id="5b47a-199">Int32</span><span class="sxs-lookup"><span data-stu-id="5b47a-199">Int32</span></span>|<span data-ttu-id="5b47a-200">Определяет возможность запретить пользователям с помощью предыдущих ПИН-коды.</span><span class="sxs-lookup"><span data-stu-id="5b47a-200">Controls the ability to prevent users from using past PINs.</span></span> <span data-ttu-id="5b47a-201">Это должно иметь значение от 0 до 50, включительно, и текущий ПИН-код пользователя включается в этот счетчик.</span><span class="sxs-lookup"><span data-stu-id="5b47a-201">This must be set between 0 and 50, inclusive, and the current PIN of the user is included in that count.</span></span> <span data-ttu-id="5b47a-202">Если значение 0, предыдущих ПИН-коды не сохраняются.</span><span class="sxs-lookup"><span data-stu-id="5b47a-202">If set to 0, previous PINs are not stored.</span></span> <span data-ttu-id="5b47a-203">ПИН-код не сохраняется через ПИН-код сбросить.</span><span class="sxs-lookup"><span data-stu-id="5b47a-203">PIN history is not preserved through a PIN reset.</span></span> <span data-ttu-id="5b47a-204">Допустимые значения: от 0 до 50.</span><span class="sxs-lookup"><span data-stu-id="5b47a-204">Valid values 0 to 50</span></span>|
|<span data-ttu-id="5b47a-205">pinRecoveryEnabled</span><span class="sxs-lookup"><span data-stu-id="5b47a-205">pinRecoveryEnabled</span></span>|<span data-ttu-id="5b47a-206">Логический</span><span class="sxs-lookup"><span data-stu-id="5b47a-206">Boolean</span></span>|<span data-ttu-id="5b47a-207">Логическое значение, которое позволяет пользователям изменять свой ПИН-код с помощью Windows Hello для восстановления службы Business ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="5b47a-207">Boolean value that enables a user to change their PIN by using the Windows Hello for Business PIN recovery service.</span></span>|
|<span data-ttu-id="5b47a-208">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="5b47a-208">securityDeviceRequired</span></span>|<span data-ttu-id="5b47a-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b47a-209">Boolean</span></span>|<span data-ttu-id="5b47a-210">Определяет необходимость доверенного платформы модуля (TPM) для подготовки Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="5b47a-210">Controls whether to require a Trusted Platform Module (TPM) for provisioning Windows Hello for Business.</span></span> <span data-ttu-id="5b47a-211">TPM обеспечивает дополнительных преимуществ для безопасности, в том, что данные, хранящиеся на его нельзя использовать на других устройствах.</span><span class="sxs-lookup"><span data-stu-id="5b47a-211">A TPM provides an additional security benefit in that data stored on it cannot be used on other devices.</span></span> <span data-ttu-id="5b47a-212">Если задано значение False, все устройства можно подготовить Windows Hello для бизнеса даже в том случае, если не могут использоваться TPM.</span><span class="sxs-lookup"><span data-stu-id="5b47a-212">If set to False, all devices can provision Windows Hello for Business even if there is not a usable TPM.</span></span>|
|<span data-ttu-id="5b47a-213">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="5b47a-213">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="5b47a-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b47a-214">Boolean</span></span>|<span data-ttu-id="5b47a-215">Управляет Биометрическая жестов, таких как начертание и отпечаток, как альтернативы Windows Hello для бизнеса ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="5b47a-215">Controls the use of biometric gestures, such as face and fingerprint, as an alternative to the Windows Hello for Business PIN.</span></span>  <span data-ttu-id="5b47a-216">Если параметр имеет значение False, Биометрическая жесты не разрешены.</span><span class="sxs-lookup"><span data-stu-id="5b47a-216">If set to False, biometric gestures are not allowed.</span></span> <span data-ttu-id="5b47a-217">Пользователи по-прежнему необходимо настроить ПИН-код для резервного копирования в случае сбоев.</span><span class="sxs-lookup"><span data-stu-id="5b47a-217">Users must still configure a PIN as a backup in case of failures.</span></span>|
|<span data-ttu-id="5b47a-218">useCertificatesForOnPremisesAuthEnabled</span><span class="sxs-lookup"><span data-stu-id="5b47a-218">useCertificatesForOnPremisesAuthEnabled</span></span>|<span data-ttu-id="5b47a-219">Логический</span><span class="sxs-lookup"><span data-stu-id="5b47a-219">Boolean</span></span>|<span data-ttu-id="5b47a-220">Логическое значение, включающее Windows Hello для бизнеса для использования сертификатов для проверки подлинности локальным ресурсам.</span><span class="sxs-lookup"><span data-stu-id="5b47a-220">Boolean value that enables Windows Hello for Business to use certificates to authenticate on-premise resources.</span></span>|
|<span data-ttu-id="5b47a-221">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="5b47a-221">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="5b47a-222">Логический</span><span class="sxs-lookup"><span data-stu-id="5b47a-222">Boolean</span></span>|<span data-ttu-id="5b47a-223">Логическое значение, которое блокирует Windows Hello для бизнеса, как метод для входа в Windows.</span><span class="sxs-lookup"><span data-stu-id="5b47a-223">Boolean value that blocks Windows Hello for Business as a method for signing into Windows.</span></span>|



## <a name="response"></a><span data-ttu-id="5b47a-224">Ответ</span><span class="sxs-lookup"><span data-stu-id="5b47a-224">Response</span></span>
<span data-ttu-id="5b47a-225">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5b47a-225">If successful, this method returns a `200 OK` response code and an updated [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b47a-226">Пример</span><span class="sxs-lookup"><span data-stu-id="5b47a-226">Example</span></span>
### <a name="request"></a><span data-ttu-id="5b47a-227">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b47a-227">Request</span></span>
<span data-ttu-id="5b47a-228">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5b47a-228">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 761

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
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

### <a name="response"></a><span data-ttu-id="5b47a-229">Ответ</span><span class="sxs-lookup"><span data-stu-id="5b47a-229">Response</span></span>
<span data-ttu-id="5b47a-p120">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5b47a-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 946

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





