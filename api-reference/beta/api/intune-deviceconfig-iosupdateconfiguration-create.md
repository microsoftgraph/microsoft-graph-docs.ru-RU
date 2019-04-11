---
title: Create iosUpdateConfiguration
description: Создание объекта iosUpdateConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 43a48f494c37af8722bbf209a2c41e4ef1e902fc
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31797167"
---
# <a name="create-iosupdateconfiguration"></a><span data-ttu-id="6ba60-103">Create iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="6ba60-103">Create iosUpdateConfiguration</span></span>

> <span data-ttu-id="6ba60-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ba60-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ba60-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6ba60-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ba60-106">Создание объекта [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ba60-106">Create a new [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6ba60-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="6ba60-107">Prerequisites</span></span>
<span data-ttu-id="6ba60-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ba60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ba60-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6ba60-110">Permission type</span></span>|<span data-ttu-id="6ba60-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6ba60-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ba60-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6ba60-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6ba60-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ba60-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6ba60-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6ba60-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ba60-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ba60-115">Not supported.</span></span>|
|<span data-ttu-id="6ba60-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6ba60-116">Application</span></span>|<span data-ttu-id="6ba60-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ba60-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ba60-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6ba60-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6ba60-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6ba60-119">Request headers</span></span>
|<span data-ttu-id="6ba60-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6ba60-120">Header</span></span>|<span data-ttu-id="6ba60-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6ba60-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6ba60-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6ba60-122">Authorization</span></span>|<span data-ttu-id="6ba60-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6ba60-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6ba60-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6ba60-124">Accept</span></span>|<span data-ttu-id="6ba60-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6ba60-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ba60-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6ba60-126">Request body</span></span>
<span data-ttu-id="6ba60-127">В теле запроса добавьте представление объекта iosUpdateConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6ba60-127">In the request body, supply a JSON representation for the iosUpdateConfiguration object.</span></span>

<span data-ttu-id="6ba60-128">Ниже показаны свойства, которые необходимо указывать при создании объекта iosUpdateConfiguration.</span><span class="sxs-lookup"><span data-stu-id="6ba60-128">The following table shows the properties that are required when you create the iosUpdateConfiguration.</span></span>

|<span data-ttu-id="6ba60-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="6ba60-129">Property</span></span>|<span data-ttu-id="6ba60-130">Тип</span><span class="sxs-lookup"><span data-stu-id="6ba60-130">Type</span></span>|<span data-ttu-id="6ba60-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6ba60-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ba60-132">id</span><span class="sxs-lookup"><span data-stu-id="6ba60-132">id</span></span>|<span data-ttu-id="6ba60-133">Строка</span><span class="sxs-lookup"><span data-stu-id="6ba60-133">String</span></span>|<span data-ttu-id="6ba60-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6ba60-134">Key of the entity.</span></span> <span data-ttu-id="6ba60-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ba60-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ba60-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6ba60-136">lastModifiedDateTime</span></span>|<span data-ttu-id="6ba60-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ba60-137">DateTimeOffset</span></span>|<span data-ttu-id="6ba60-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="6ba60-138">DateTime the object was last modified.</span></span> <span data-ttu-id="6ba60-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ba60-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ba60-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6ba60-140">roleScopeTagIds</span></span>|<span data-ttu-id="6ba60-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6ba60-141">String collection</span></span>|<span data-ttu-id="6ba60-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="6ba60-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6ba60-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ba60-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ba60-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="6ba60-144">supportsScopeTags</span></span>|<span data-ttu-id="6ba60-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ba60-145">Boolean</span></span>|<span data-ttu-id="6ba60-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="6ba60-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6ba60-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="6ba60-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6ba60-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="6ba60-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6ba60-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6ba60-149">This property is read-only.</span></span> <span data-ttu-id="6ba60-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ba60-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ba60-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6ba60-151">createdDateTime</span></span>|<span data-ttu-id="6ba60-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ba60-152">DateTimeOffset</span></span>|<span data-ttu-id="6ba60-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="6ba60-153">DateTime the object was created.</span></span> <span data-ttu-id="6ba60-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ba60-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ba60-155">description</span><span class="sxs-lookup"><span data-stu-id="6ba60-155">description</span></span>|<span data-ttu-id="6ba60-156">String</span><span class="sxs-lookup"><span data-stu-id="6ba60-156">String</span></span>|<span data-ttu-id="6ba60-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6ba60-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6ba60-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ba60-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ba60-159">displayName</span><span class="sxs-lookup"><span data-stu-id="6ba60-159">displayName</span></span>|<span data-ttu-id="6ba60-160">String</span><span class="sxs-lookup"><span data-stu-id="6ba60-160">String</span></span>|<span data-ttu-id="6ba60-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6ba60-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6ba60-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ba60-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ba60-163">version</span><span class="sxs-lookup"><span data-stu-id="6ba60-163">version</span></span>|<span data-ttu-id="6ba60-164">Int32</span><span class="sxs-lookup"><span data-stu-id="6ba60-164">Int32</span></span>|<span data-ttu-id="6ba60-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6ba60-165">Version of the device configuration.</span></span> <span data-ttu-id="6ba60-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ba60-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ba60-167">isEnabled</span><span class="sxs-lookup"><span data-stu-id="6ba60-167">isEnabled</span></span>|<span data-ttu-id="6ba60-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ba60-168">Boolean</span></span>|<span data-ttu-id="6ba60-169">Включен параметр в ПОЛЬЗОВАТЕЛЬСКОМ ИНТЕРФЕЙСе</span><span class="sxs-lookup"><span data-stu-id="6ba60-169">Is setting enabled in UI</span></span>|
|<span data-ttu-id="6ba60-170">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="6ba60-170">activeHoursStart</span></span>|<span data-ttu-id="6ba60-171">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="6ba60-171">TimeOfDay</span></span>|<span data-ttu-id="6ba60-172">Начало периода активности (период активности — временной промежуток, в течение которого не должны устанавливаться обновления).</span><span class="sxs-lookup"><span data-stu-id="6ba60-172">Active Hours Start (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="6ba60-173">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="6ba60-173">activeHoursEnd</span></span>|<span data-ttu-id="6ba60-174">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="6ba60-174">TimeOfDay</span></span>|<span data-ttu-id="6ba60-175">Завершение периода активности (период активности — временной промежуток, в течение которого не должны устанавливаться обновления).</span><span class="sxs-lookup"><span data-stu-id="6ba60-175">Active Hours End (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="6ba60-176">scheduledInstallDays</span><span class="sxs-lookup"><span data-stu-id="6ba60-176">scheduledInstallDays</span></span>|<span data-ttu-id="6ba60-177">Коллекция [DayOfWeek](../resources/intune-deviceconfig-dayofweek.md)</span><span class="sxs-lookup"><span data-stu-id="6ba60-177">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md) collection</span></span>|<span data-ttu-id="6ba60-178">Дни недели, для которых настраивается период активности.</span><span class="sxs-lookup"><span data-stu-id="6ba60-178">Days in week for which active hours are configured.</span></span> <span data-ttu-id="6ba60-179">Эта коллекция может содержать не более 7 элементов.</span><span class="sxs-lookup"><span data-stu-id="6ba60-179">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="6ba60-180">Возможные значения: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="6ba60-180">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="6ba60-181">utcTimeOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="6ba60-181">utcTimeOffsetInMinutes</span></span>|<span data-ttu-id="6ba60-182">Int32</span><span class="sxs-lookup"><span data-stu-id="6ba60-182">Int32</span></span>|<span data-ttu-id="6ba60-183">Сдвиг по времени от UTC (в минутах).</span><span class="sxs-lookup"><span data-stu-id="6ba60-183">UTC Time Offset indicated in minutes</span></span>|
|<span data-ttu-id="6ba60-184">Енфорцедсофтвареупдатеделайиндайс</span><span class="sxs-lookup"><span data-stu-id="6ba60-184">enforcedSoftwareUpdateDelayInDays</span></span>|<span data-ttu-id="6ba60-185">Int32</span><span class="sxs-lookup"><span data-stu-id="6ba60-185">Int32</span></span>|<span data-ttu-id="6ba60-186">Дней до отображения обновлений программного обеспечения для устройств с iOS в диапазоне от 0 до 90 включительно</span><span class="sxs-lookup"><span data-stu-id="6ba60-186">Days before software updates are visible to iOS devices ranging from 0 to 90 inclusive</span></span>|



## <a name="response"></a><span data-ttu-id="6ba60-187">Ответ</span><span class="sxs-lookup"><span data-stu-id="6ba60-187">Response</span></span>
<span data-ttu-id="6ba60-188">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6ba60-188">If successful, this method returns a `201 Created` response code and a [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ba60-189">Пример</span><span class="sxs-lookup"><span data-stu-id="6ba60-189">Example</span></span>

### <a name="request"></a><span data-ttu-id="6ba60-190">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ba60-190">Request</span></span>
<span data-ttu-id="6ba60-191">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6ba60-191">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 482

{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "isEnabled": true,
  "activeHoursStart": "12:00:05.5020000",
  "activeHoursEnd": "11:59:00.8990000",
  "scheduledInstallDays": [
    "monday"
  ],
  "utcTimeOffsetInMinutes": 6,
  "enforcedSoftwareUpdateDelayInDays": 1
}
```

### <a name="response"></a><span data-ttu-id="6ba60-192">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ba60-192">Response</span></span>
<span data-ttu-id="6ba60-p111">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6ba60-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 654

{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
  "id": "321aef09-ef09-321a-09ef-1a3209ef1a32",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "isEnabled": true,
  "activeHoursStart": "12:00:05.5020000",
  "activeHoursEnd": "11:59:00.8990000",
  "scheduledInstallDays": [
    "monday"
  ],
  "utcTimeOffsetInMinutes": 6,
  "enforcedSoftwareUpdateDelayInDays": 1
}
```





