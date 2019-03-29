---
title: Создание Виндовсидентитипротектионконфигуратион
description: Создание нового объекта Виндовсидентитипротектионконфигуратион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ea50bd99870c166b4add41d5cfe41ee6e387b158
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30958174"
---
# <a name="create-windowsidentityprotectionconfiguration"></a><span data-ttu-id="a800c-103">Создание Виндовсидентитипротектионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="a800c-103">Create windowsIdentityProtectionConfiguration</span></span>

> <span data-ttu-id="a800c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a800c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a800c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a800c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a800c-106">Создание нового объекта [виндовсидентитипротектионконфигуратион](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a800c-106">Create a new [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a800c-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a800c-107">Prerequisites</span></span>
<span data-ttu-id="a800c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a800c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a800c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a800c-110">Permission type</span></span>|<span data-ttu-id="a800c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a800c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a800c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a800c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a800c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a800c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a800c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a800c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a800c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a800c-115">Not supported.</span></span>|
|<span data-ttu-id="a800c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a800c-116">Application</span></span>|<span data-ttu-id="a800c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a800c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a800c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a800c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a800c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a800c-119">Request headers</span></span>
|<span data-ttu-id="a800c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a800c-120">Header</span></span>|<span data-ttu-id="a800c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a800c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a800c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a800c-122">Authorization</span></span>|<span data-ttu-id="a800c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a800c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a800c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a800c-124">Accept</span></span>|<span data-ttu-id="a800c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a800c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a800c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a800c-126">Request body</span></span>
<span data-ttu-id="a800c-127">В тексте запроса добавьте представление объекта Виндовсидентитипротектионконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a800c-127">In the request body, supply a JSON representation for the windowsIdentityProtectionConfiguration object.</span></span>

<span data-ttu-id="a800c-128">В следующей таблице приведены свойства, необходимые при создании Виндовсидентитипротектионконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="a800c-128">The following table shows the properties that are required when you create the windowsIdentityProtectionConfiguration.</span></span>

|<span data-ttu-id="a800c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a800c-129">Property</span></span>|<span data-ttu-id="a800c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a800c-130">Type</span></span>|<span data-ttu-id="a800c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a800c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a800c-132">id</span><span class="sxs-lookup"><span data-stu-id="a800c-132">id</span></span>|<span data-ttu-id="a800c-133">Строка</span><span class="sxs-lookup"><span data-stu-id="a800c-133">String</span></span>|<span data-ttu-id="a800c-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a800c-134">Key of the entity.</span></span> <span data-ttu-id="a800c-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a800c-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a800c-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a800c-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a800c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a800c-137">DateTimeOffset</span></span>|<span data-ttu-id="a800c-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a800c-138">DateTime the object was last modified.</span></span> <span data-ttu-id="a800c-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a800c-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a800c-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a800c-140">roleScopeTagIds</span></span>|<span data-ttu-id="a800c-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="a800c-141">String collection</span></span>|<span data-ttu-id="a800c-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="a800c-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a800c-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a800c-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a800c-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="a800c-144">supportsScopeTags</span></span>|<span data-ttu-id="a800c-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="a800c-145">Boolean</span></span>|<span data-ttu-id="a800c-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="a800c-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a800c-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="a800c-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a800c-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="a800c-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a800c-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a800c-149">This property is read-only.</span></span> <span data-ttu-id="a800c-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a800c-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a800c-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a800c-151">createdDateTime</span></span>|<span data-ttu-id="a800c-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a800c-152">DateTimeOffset</span></span>|<span data-ttu-id="a800c-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="a800c-153">DateTime the object was created.</span></span> <span data-ttu-id="a800c-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a800c-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a800c-155">description</span><span class="sxs-lookup"><span data-stu-id="a800c-155">description</span></span>|<span data-ttu-id="a800c-156">String</span><span class="sxs-lookup"><span data-stu-id="a800c-156">String</span></span>|<span data-ttu-id="a800c-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a800c-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a800c-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a800c-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a800c-159">displayName</span><span class="sxs-lookup"><span data-stu-id="a800c-159">displayName</span></span>|<span data-ttu-id="a800c-160">String</span><span class="sxs-lookup"><span data-stu-id="a800c-160">String</span></span>|<span data-ttu-id="a800c-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a800c-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a800c-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a800c-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a800c-163">version</span><span class="sxs-lookup"><span data-stu-id="a800c-163">version</span></span>|<span data-ttu-id="a800c-164">Int32</span><span class="sxs-lookup"><span data-stu-id="a800c-164">Int32</span></span>|<span data-ttu-id="a800c-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a800c-165">Version of the device configuration.</span></span> <span data-ttu-id="a800c-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a800c-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a800c-167">Усесекуритикэйфорсигнин</span><span class="sxs-lookup"><span data-stu-id="a800c-167">useSecurityKeyForSignin</span></span>|<span data-ttu-id="a800c-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="a800c-168">Boolean</span></span>|<span data-ttu-id="a800c-169">Логическое значение, используемое для включения ключа безопасности Windows Hello в качестве учетных данных для входа.</span><span class="sxs-lookup"><span data-stu-id="a800c-169">Boolean value used to enable the Windows Hello security key as a logon credential.</span></span>|
|<span data-ttu-id="a800c-170">ЕнханцедантиспуфингфорфаЦиалфеатуресенаблед</span><span class="sxs-lookup"><span data-stu-id="a800c-170">enhancedAntiSpoofingForFacialFeaturesEnabled</span></span>|<span data-ttu-id="a800c-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="a800c-171">Boolean</span></span>|<span data-ttu-id="a800c-172">Логическое значение, используемое для включения расширенного средства защиты от спуфинга для распознавания функции лица при проверке подлинности Windows Hello для лиц.</span><span class="sxs-lookup"><span data-stu-id="a800c-172">Boolean value used to enable enhanced anti-spoofing for facial feature recognition on Windows Hello face authentication.</span></span>|
|<span data-ttu-id="a800c-173">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="a800c-173">pinMinimumLength</span></span>|<span data-ttu-id="a800c-174">Int32</span><span class="sxs-lookup"><span data-stu-id="a800c-174">Int32</span></span>|<span data-ttu-id="a800c-175">Целочисленное значение, задающее минимальное число символов, необходимое для ПИН-кода Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="a800c-175">Integer value that sets the minimum number of characters required for the Windows Hello for Business PIN.</span></span> <span data-ttu-id="a800c-176">Допустимые значения: от 4 до 127 включительно и меньше или равны набору значений для максимального ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="a800c-176">Valid values are 4 to 127 inclusive and less than or equal to the value set for the maximum PIN.</span></span> <span data-ttu-id="a800c-177">Допустимые значения — от 4 до 127</span><span class="sxs-lookup"><span data-stu-id="a800c-177">Valid values 4 to 127</span></span>|
|<span data-ttu-id="a800c-178">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="a800c-178">pinMaximumLength</span></span>|<span data-ttu-id="a800c-179">Int32</span><span class="sxs-lookup"><span data-stu-id="a800c-179">Int32</span></span>|<span data-ttu-id="a800c-180">Целое значение, задающее максимальное количество символов для рабочего ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="a800c-180">Integer value that sets the maximum number of characters allowed for the work PIN.</span></span> <span data-ttu-id="a800c-181">Допустимые значения: от 4 до 127 включительно и больше или равны значению, заданному для минимального ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="a800c-181">Valid values are 4 to 127 inclusive and greater than or equal to the value set for the minimum PIN.</span></span> <span data-ttu-id="a800c-182">Допустимые значения — от 4 до 127</span><span class="sxs-lookup"><span data-stu-id="a800c-182">Valid values 4 to 127</span></span>|
|<span data-ttu-id="a800c-183">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="a800c-183">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="a800c-184">Конфигуратионусаже</span><span class="sxs-lookup"><span data-stu-id="a800c-184">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="a800c-185">Это значение позволяет настроить использование символов верхнего регистра в ПИН-коде Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="a800c-185">This value configures the use of uppercase characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="a800c-186">Возможные значения: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="a800c-186">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="a800c-187">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="a800c-187">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="a800c-188">Конфигуратионусаже</span><span class="sxs-lookup"><span data-stu-id="a800c-188">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="a800c-189">Это значение позволяет настроить использование символов нижнего регистра в ПИН-коде Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="a800c-189">This value configures the use of lowercase characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="a800c-190">Возможные значения: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="a800c-190">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="a800c-191">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="a800c-191">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="a800c-192">Конфигуратионусаже</span><span class="sxs-lookup"><span data-stu-id="a800c-192">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="a800c-193">Управляет возможностью использования специальных символов в ПИН-коде Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="a800c-193">Controls the ability to use special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="a800c-194">Возможные значения: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="a800c-194">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="a800c-195">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="a800c-195">pinExpirationInDays</span></span>|<span data-ttu-id="a800c-196">Int32</span><span class="sxs-lookup"><span data-stu-id="a800c-196">Int32</span></span>|<span data-ttu-id="a800c-197">Integer value указывает период времени (в днях), в течение которого можно использовать ПИН-код, прежде чем система потребует от пользователя изменить его.</span><span class="sxs-lookup"><span data-stu-id="a800c-197">Integer value specifies the period (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="a800c-198">Допустимые значения: от 0 до 730 включительно.</span><span class="sxs-lookup"><span data-stu-id="a800c-198">Valid values are 0 to 730 inclusive.</span></span> <span data-ttu-id="a800c-199">Допустимые значения: от 0 до 730.</span><span class="sxs-lookup"><span data-stu-id="a800c-199">Valid values 0 to 730</span></span>|
|<span data-ttu-id="a800c-200">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="a800c-200">pinPreviousBlockCount</span></span>|<span data-ttu-id="a800c-201">Int32</span><span class="sxs-lookup"><span data-stu-id="a800c-201">Int32</span></span>|<span data-ttu-id="a800c-202">Управляет возможностью запретить пользователям использовать прошлые контакты.</span><span class="sxs-lookup"><span data-stu-id="a800c-202">Controls the ability to prevent users from using past PINs.</span></span> <span data-ttu-id="a800c-203">Он должен иметь значение от 0 до 50 включительно, а текущий ПИН-код пользователя включен в этот счетчик.</span><span class="sxs-lookup"><span data-stu-id="a800c-203">This must be set between 0 and 50, inclusive, and the current PIN of the user is included in that count.</span></span> <span data-ttu-id="a800c-204">Если задано значение 0, предыдущие ПИН-коды не сохраняются.</span><span class="sxs-lookup"><span data-stu-id="a800c-204">If set to 0, previous PINs are not stored.</span></span> <span data-ttu-id="a800c-205">История ПИН-кодов не сохраняется при сбросе ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="a800c-205">PIN history is not preserved through a PIN reset.</span></span> <span data-ttu-id="a800c-206">Допустимые значения: от 0 до 50.</span><span class="sxs-lookup"><span data-stu-id="a800c-206">Valid values 0 to 50</span></span>|
|<span data-ttu-id="a800c-207">Пинрековеренаблед</span><span class="sxs-lookup"><span data-stu-id="a800c-207">pinRecoveryEnabled</span></span>|<span data-ttu-id="a800c-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="a800c-208">Boolean</span></span>|<span data-ttu-id="a800c-209">Логическое значение, которое позволяет пользователю изменить свой ПИН-код с помощью службы восстановления ПИН-кода Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="a800c-209">Boolean value that enables a user to change their PIN by using the Windows Hello for Business PIN recovery service.</span></span>|
|<span data-ttu-id="a800c-210">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="a800c-210">securityDeviceRequired</span></span>|<span data-ttu-id="a800c-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="a800c-211">Boolean</span></span>|<span data-ttu-id="a800c-212">Определяет, требуется ли доверенный ПЛАТФОРМЕНный модуль для подготовки Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="a800c-212">Controls whether to require a Trusted Platform Module (TPM) for provisioning Windows Hello for Business.</span></span> <span data-ttu-id="a800c-213">TPM предоставляет дополнительные преимущества безопасности, которые хранятся на нем, не могут использоваться на других устройствах.</span><span class="sxs-lookup"><span data-stu-id="a800c-213">A TPM provides an additional security benefit in that data stored on it cannot be used on other devices.</span></span> <span data-ttu-id="a800c-214">Если задано значение false, все устройства могут подготавливать Windows Hello для бизнеса, даже если нет пригодного к использованию ДОВЕРЕНного ПЛАТФОРМЕНного модуля.</span><span class="sxs-lookup"><span data-stu-id="a800c-214">If set to False, all devices can provision Windows Hello for Business even if there is not a usable TPM.</span></span>|
|<span data-ttu-id="a800c-215">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="a800c-215">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="a800c-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="a800c-216">Boolean</span></span>|<span data-ttu-id="a800c-217">Управляет использованием биометрических жестов, таких как лицо и отпечаток, в качестве альтернативы ПИН-коду Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="a800c-217">Controls the use of biometric gestures, such as face and fingerprint, as an alternative to the Windows Hello for Business PIN.</span></span>  <span data-ttu-id="a800c-218">Если задано значение false, биометрические жесты не разрешены.</span><span class="sxs-lookup"><span data-stu-id="a800c-218">If set to False, biometric gestures are not allowed.</span></span> <span data-ttu-id="a800c-219">Пользователи по-прежнему должны настроить ПИН-код в качестве резервной копии в случае сбоев.</span><span class="sxs-lookup"><span data-stu-id="a800c-219">Users must still configure a PIN as a backup in case of failures.</span></span>|
|<span data-ttu-id="a800c-220">Усецертификатесфоронпремисесаусенаблед</span><span class="sxs-lookup"><span data-stu-id="a800c-220">useCertificatesForOnPremisesAuthEnabled</span></span>|<span data-ttu-id="a800c-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="a800c-221">Boolean</span></span>|<span data-ttu-id="a800c-222">Логическое значение, которое позволяет Windows Hello для бизнеса использовать сертификаты для проверки подлинности локальных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="a800c-222">Boolean value that enables Windows Hello for Business to use certificates to authenticate on-premise resources.</span></span>|
|<span data-ttu-id="a800c-223">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="a800c-223">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="a800c-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="a800c-224">Boolean</span></span>|<span data-ttu-id="a800c-225">Логическое значение, блокирующее Windows Hello для бизнеса в качестве способа входа в Windows.</span><span class="sxs-lookup"><span data-stu-id="a800c-225">Boolean value that blocks Windows Hello for Business as a method for signing into Windows.</span></span>|



## <a name="response"></a><span data-ttu-id="a800c-226">Отклик</span><span class="sxs-lookup"><span data-stu-id="a800c-226">Response</span></span>
<span data-ttu-id="a800c-227">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсидентитипротектионконфигуратион](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a800c-227">If successful, this method returns a `201 Created` response code and a [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a800c-228">Пример</span><span class="sxs-lookup"><span data-stu-id="a800c-228">Example</span></span>

### <a name="request"></a><span data-ttu-id="a800c-229">Запрос</span><span class="sxs-lookup"><span data-stu-id="a800c-229">Request</span></span>
<span data-ttu-id="a800c-230">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a800c-230">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a800c-231">Отклик</span><span class="sxs-lookup"><span data-stu-id="a800c-231">Response</span></span>
<span data-ttu-id="a800c-p119">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a800c-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




