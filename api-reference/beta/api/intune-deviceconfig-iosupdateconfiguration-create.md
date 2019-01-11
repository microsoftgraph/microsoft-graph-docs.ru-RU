---
title: Create iosUpdateConfiguration
description: Создание объекта iosUpdateConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: cab02b7a3788f55d657b93453fc074bd63d4d918
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852341"
---
# <a name="create-iosupdateconfiguration"></a><span data-ttu-id="155c5-103">Create iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="155c5-103">Create iosUpdateConfiguration</span></span>

> <span data-ttu-id="155c5-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="155c5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="155c5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="155c5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="155c5-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="155c5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="155c5-107">Создание объекта [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="155c5-107">Create a new [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="155c5-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="155c5-108">Prerequisites</span></span>
<span data-ttu-id="155c5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="155c5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="155c5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="155c5-111">Permission type</span></span>|<span data-ttu-id="155c5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="155c5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="155c5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="155c5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="155c5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="155c5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="155c5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="155c5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="155c5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="155c5-116">Not supported.</span></span>|
|<span data-ttu-id="155c5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="155c5-117">Application</span></span>|<span data-ttu-id="155c5-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="155c5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="155c5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="155c5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="155c5-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="155c5-120">Request headers</span></span>
|<span data-ttu-id="155c5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="155c5-121">Header</span></span>|<span data-ttu-id="155c5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="155c5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="155c5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="155c5-123">Authorization</span></span>|<span data-ttu-id="155c5-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="155c5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="155c5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="155c5-125">Accept</span></span>|<span data-ttu-id="155c5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="155c5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="155c5-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="155c5-127">Request body</span></span>
<span data-ttu-id="155c5-128">В теле запроса добавьте представление объекта iosUpdateConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="155c5-128">In the request body, supply a JSON representation for the iosUpdateConfiguration object.</span></span>

<span data-ttu-id="155c5-129">Ниже показаны свойства, которые необходимо указывать при создании объекта iosUpdateConfiguration.</span><span class="sxs-lookup"><span data-stu-id="155c5-129">The following table shows the properties that are required when you create the iosUpdateConfiguration.</span></span>

|<span data-ttu-id="155c5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="155c5-130">Property</span></span>|<span data-ttu-id="155c5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="155c5-131">Type</span></span>|<span data-ttu-id="155c5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="155c5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="155c5-133">id</span><span class="sxs-lookup"><span data-stu-id="155c5-133">id</span></span>|<span data-ttu-id="155c5-134">Строка</span><span class="sxs-lookup"><span data-stu-id="155c5-134">String</span></span>|<span data-ttu-id="155c5-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="155c5-135">Key of the entity.</span></span> <span data-ttu-id="155c5-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="155c5-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="155c5-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="155c5-137">lastModifiedDateTime</span></span>|<span data-ttu-id="155c5-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="155c5-138">DateTimeOffset</span></span>|<span data-ttu-id="155c5-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="155c5-139">DateTime the object was last modified.</span></span> <span data-ttu-id="155c5-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="155c5-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="155c5-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="155c5-141">roleScopeTagIds</span></span>|<span data-ttu-id="155c5-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="155c5-142">String collection</span></span>|<span data-ttu-id="155c5-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="155c5-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="155c5-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="155c5-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="155c5-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="155c5-145">supportsScopeTags</span></span>|<span data-ttu-id="155c5-146">Логический</span><span class="sxs-lookup"><span data-stu-id="155c5-146">Boolean</span></span>|<span data-ttu-id="155c5-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="155c5-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="155c5-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="155c5-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="155c5-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="155c5-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="155c5-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="155c5-150">This property is read-only.</span></span> <span data-ttu-id="155c5-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="155c5-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="155c5-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="155c5-152">createdDateTime</span></span>|<span data-ttu-id="155c5-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="155c5-153">DateTimeOffset</span></span>|<span data-ttu-id="155c5-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="155c5-154">DateTime the object was created.</span></span> <span data-ttu-id="155c5-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="155c5-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="155c5-156">описание</span><span class="sxs-lookup"><span data-stu-id="155c5-156">description</span></span>|<span data-ttu-id="155c5-157">Строка</span><span class="sxs-lookup"><span data-stu-id="155c5-157">String</span></span>|<span data-ttu-id="155c5-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="155c5-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="155c5-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="155c5-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="155c5-160">displayName</span><span class="sxs-lookup"><span data-stu-id="155c5-160">displayName</span></span>|<span data-ttu-id="155c5-161">Строка</span><span class="sxs-lookup"><span data-stu-id="155c5-161">String</span></span>|<span data-ttu-id="155c5-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="155c5-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="155c5-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="155c5-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="155c5-164">version</span><span class="sxs-lookup"><span data-stu-id="155c5-164">version</span></span>|<span data-ttu-id="155c5-165">Int32</span><span class="sxs-lookup"><span data-stu-id="155c5-165">Int32</span></span>|<span data-ttu-id="155c5-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="155c5-166">Version of the device configuration.</span></span> <span data-ttu-id="155c5-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="155c5-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="155c5-168">isEnabled</span><span class="sxs-lookup"><span data-stu-id="155c5-168">isEnabled</span></span>|<span data-ttu-id="155c5-169">Логический</span><span class="sxs-lookup"><span data-stu-id="155c5-169">Boolean</span></span>|<span data-ttu-id="155c5-170">Включен ли параметр в пользовательском Интерфейсе</span><span class="sxs-lookup"><span data-stu-id="155c5-170">Is setting enabled in UI</span></span>|
|<span data-ttu-id="155c5-171">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="155c5-171">activeHoursStart</span></span>|<span data-ttu-id="155c5-172">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="155c5-172">TimeOfDay</span></span>|<span data-ttu-id="155c5-173">Начало периода активности (период активности — временной промежуток, в течение которого не должны устанавливаться обновления).</span><span class="sxs-lookup"><span data-stu-id="155c5-173">Active Hours Start (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="155c5-174">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="155c5-174">activeHoursEnd</span></span>|<span data-ttu-id="155c5-175">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="155c5-175">TimeOfDay</span></span>|<span data-ttu-id="155c5-176">Завершение периода активности (период активности — временной промежуток, в течение которого не должны устанавливаться обновления).</span><span class="sxs-lookup"><span data-stu-id="155c5-176">Active Hours End (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="155c5-177">scheduledInstallDays</span><span class="sxs-lookup"><span data-stu-id="155c5-177">scheduledInstallDays</span></span>|<span data-ttu-id="155c5-178">Коллекция [dayOfWeek](../resources/intune-deviceconfig-dayofweek.md)</span><span class="sxs-lookup"><span data-stu-id="155c5-178">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md) collection</span></span>|<span data-ttu-id="155c5-179">Дни недели, для которых настраивается период активности.</span><span class="sxs-lookup"><span data-stu-id="155c5-179">Days in week for which active hours are configured.</span></span> <span data-ttu-id="155c5-180">Эта коллекция может содержать не более 7 элементов.</span><span class="sxs-lookup"><span data-stu-id="155c5-180">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="155c5-181">Возможные значения: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="155c5-181">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="155c5-182">utcTimeOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="155c5-182">utcTimeOffsetInMinutes</span></span>|<span data-ttu-id="155c5-183">Int32</span><span class="sxs-lookup"><span data-stu-id="155c5-183">Int32</span></span>|<span data-ttu-id="155c5-184">Сдвиг по времени от UTC (в минутах).</span><span class="sxs-lookup"><span data-stu-id="155c5-184">UTC Time Offset indicated in minutes</span></span>|
|<span data-ttu-id="155c5-185">enforcedSoftwareUpdateDelayInDays</span><span class="sxs-lookup"><span data-stu-id="155c5-185">enforcedSoftwareUpdateDelayInDays</span></span>|<span data-ttu-id="155c5-186">Int32</span><span class="sxs-lookup"><span data-stu-id="155c5-186">Int32</span></span>|<span data-ttu-id="155c5-187">От 0 до 90 включительно устройства iOS видны дней до обновления программного обеспечения</span><span class="sxs-lookup"><span data-stu-id="155c5-187">Days before software updates are visible to iOS devices ranging from 0 to 90 inclusive</span></span>|



## <a name="response"></a><span data-ttu-id="155c5-188">Ответ</span><span class="sxs-lookup"><span data-stu-id="155c5-188">Response</span></span>
<span data-ttu-id="155c5-189">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="155c5-189">If successful, this method returns a `201 Created` response code and a [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="155c5-190">Пример</span><span class="sxs-lookup"><span data-stu-id="155c5-190">Example</span></span>
### <a name="request"></a><span data-ttu-id="155c5-191">Запрос</span><span class="sxs-lookup"><span data-stu-id="155c5-191">Request</span></span>
<span data-ttu-id="155c5-192">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="155c5-192">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 546

{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="155c5-193">Ответ</span><span class="sxs-lookup"><span data-stu-id="155c5-193">Response</span></span>
<span data-ttu-id="155c5-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="155c5-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





