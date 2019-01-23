---
title: Создание windowsDeliveryOptimizationConfiguration
description: Создание нового объекта windowsDeliveryOptimizationConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1b469b93c81655ad3f071be1ffdbd36b18f32258
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430754"
---
# <a name="create-windowsdeliveryoptimizationconfiguration"></a><span data-ttu-id="bcc11-103">Создание windowsDeliveryOptimizationConfiguration</span><span class="sxs-lookup"><span data-stu-id="bcc11-103">Create windowsDeliveryOptimizationConfiguration</span></span>

> <span data-ttu-id="bcc11-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bcc11-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bcc11-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bcc11-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bcc11-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bcc11-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bcc11-107">Создание нового объекта [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="bcc11-107">Create a new [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bcc11-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="bcc11-108">Prerequisites</span></span>
<span data-ttu-id="bcc11-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="bcc11-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bcc11-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bcc11-111">Permission type</span></span>|<span data-ttu-id="bcc11-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bcc11-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bcc11-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bcc11-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bcc11-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcc11-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bcc11-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bcc11-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bcc11-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bcc11-116">Not supported.</span></span>|
|<span data-ttu-id="bcc11-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bcc11-117">Application</span></span>|<span data-ttu-id="bcc11-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bcc11-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bcc11-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bcc11-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="bcc11-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bcc11-120">Request headers</span></span>
|<span data-ttu-id="bcc11-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bcc11-121">Header</span></span>|<span data-ttu-id="bcc11-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bcc11-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bcc11-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bcc11-123">Authorization</span></span>|<span data-ttu-id="bcc11-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="bcc11-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bcc11-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bcc11-125">Accept</span></span>|<span data-ttu-id="bcc11-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bcc11-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bcc11-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bcc11-127">Request body</span></span>
<span data-ttu-id="bcc11-128">В тексте запроса укажите представление JSON для объекта windowsDeliveryOptimizationConfiguration.</span><span class="sxs-lookup"><span data-stu-id="bcc11-128">In the request body, supply a JSON representation for the windowsDeliveryOptimizationConfiguration object.</span></span>

<span data-ttu-id="bcc11-129">В следующей таблице показаны свойства, которые необходимы для создания windowsDeliveryOptimizationConfiguration.</span><span class="sxs-lookup"><span data-stu-id="bcc11-129">The following table shows the properties that are required when you create the windowsDeliveryOptimizationConfiguration.</span></span>

|<span data-ttu-id="bcc11-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="bcc11-130">Property</span></span>|<span data-ttu-id="bcc11-131">Тип</span><span class="sxs-lookup"><span data-stu-id="bcc11-131">Type</span></span>|<span data-ttu-id="bcc11-132">Описание</span><span class="sxs-lookup"><span data-stu-id="bcc11-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bcc11-133">id</span><span class="sxs-lookup"><span data-stu-id="bcc11-133">id</span></span>|<span data-ttu-id="bcc11-134">String</span><span class="sxs-lookup"><span data-stu-id="bcc11-134">String</span></span>|<span data-ttu-id="bcc11-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bcc11-135">Key of the entity.</span></span> <span data-ttu-id="bcc11-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bcc11-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bcc11-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bcc11-137">lastModifiedDateTime</span></span>|<span data-ttu-id="bcc11-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bcc11-138">DateTimeOffset</span></span>|<span data-ttu-id="bcc11-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="bcc11-139">DateTime the object was last modified.</span></span> <span data-ttu-id="bcc11-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bcc11-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bcc11-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bcc11-141">roleScopeTagIds</span></span>|<span data-ttu-id="bcc11-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="bcc11-142">String collection</span></span>|<span data-ttu-id="bcc11-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="bcc11-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="bcc11-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bcc11-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bcc11-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="bcc11-145">supportsScopeTags</span></span>|<span data-ttu-id="bcc11-146">Логический</span><span class="sxs-lookup"><span data-stu-id="bcc11-146">Boolean</span></span>|<span data-ttu-id="bcc11-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="bcc11-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="bcc11-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="bcc11-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="bcc11-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="bcc11-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="bcc11-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bcc11-150">This property is read-only.</span></span> <span data-ttu-id="bcc11-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bcc11-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bcc11-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bcc11-152">createdDateTime</span></span>|<span data-ttu-id="bcc11-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bcc11-153">DateTimeOffset</span></span>|<span data-ttu-id="bcc11-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="bcc11-154">DateTime the object was created.</span></span> <span data-ttu-id="bcc11-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bcc11-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bcc11-156">description</span><span class="sxs-lookup"><span data-stu-id="bcc11-156">description</span></span>|<span data-ttu-id="bcc11-157">String</span><span class="sxs-lookup"><span data-stu-id="bcc11-157">String</span></span>|<span data-ttu-id="bcc11-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bcc11-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bcc11-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bcc11-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bcc11-160">displayName</span><span class="sxs-lookup"><span data-stu-id="bcc11-160">displayName</span></span>|<span data-ttu-id="bcc11-161">String</span><span class="sxs-lookup"><span data-stu-id="bcc11-161">String</span></span>|<span data-ttu-id="bcc11-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bcc11-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bcc11-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bcc11-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bcc11-164">version</span><span class="sxs-lookup"><span data-stu-id="bcc11-164">version</span></span>|<span data-ttu-id="bcc11-165">Int32</span><span class="sxs-lookup"><span data-stu-id="bcc11-165">Int32</span></span>|<span data-ttu-id="bcc11-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bcc11-166">Version of the device configuration.</span></span> <span data-ttu-id="bcc11-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bcc11-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bcc11-168">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="bcc11-168">deliveryOptimizationMode</span></span>|[<span data-ttu-id="bcc11-169">windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="bcc11-169">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="bcc11-170">Указывает метод загрузки, Оптимизация доставки можно использовать для управления использования пропускной способности сети для сценариев больших распределения контента.</span><span class="sxs-lookup"><span data-stu-id="bcc11-170">Specifies the download method that delivery optimization can use to manage network bandwidth consumption for large content distribution scenarios.</span></span> <span data-ttu-id="bcc11-171">Возможные значения: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span><span class="sxs-lookup"><span data-stu-id="bcc11-171">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|



## <a name="response"></a><span data-ttu-id="bcc11-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="bcc11-172">Response</span></span>
<span data-ttu-id="bcc11-173">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="bcc11-173">If successful, this method returns a `201 Created` response code and a [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bcc11-174">Пример</span><span class="sxs-lookup"><span data-stu-id="bcc11-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="bcc11-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="bcc11-175">Request</span></span>
<span data-ttu-id="bcc11-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bcc11-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 313

{
  "@odata.type": "#microsoft.graph.windowsDeliveryOptimizationConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "deliveryOptimizationMode": "httpOnly"
}
```

### <a name="response"></a><span data-ttu-id="bcc11-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="bcc11-177">Response</span></span>
<span data-ttu-id="bcc11-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="bcc11-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 485

{
  "@odata.type": "#microsoft.graph.windowsDeliveryOptimizationConfiguration",
  "id": "5954ee9b-ee9b-5954-9bee-54599bee5459",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "deliveryOptimizationMode": "httpOnly"
}
```




