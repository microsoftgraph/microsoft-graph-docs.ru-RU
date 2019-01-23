---
title: Создание объекта windowsPhone81CustomConfiguration
description: Создание объекта windowsPhone81CustomConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 07a3ad1e5986fb9d971ffd7f1b1a08babf319454
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422903"
---
# <a name="create-windowsphone81customconfiguration"></a><span data-ttu-id="7b709-103">Создание объекта windowsPhone81CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="7b709-103">Create windowsPhone81CustomConfiguration</span></span>

> <span data-ttu-id="7b709-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7b709-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7b709-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b709-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7b709-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7b709-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b709-107">Создание объекта [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7b709-107">Create a new [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7b709-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7b709-108">Prerequisites</span></span>
<span data-ttu-id="7b709-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7b709-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7b709-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7b709-111">Permission type</span></span>|<span data-ttu-id="7b709-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7b709-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b709-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7b709-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7b709-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b709-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7b709-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7b709-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b709-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b709-116">Not supported.</span></span>|
|<span data-ttu-id="7b709-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7b709-117">Application</span></span>|<span data-ttu-id="7b709-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b709-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b709-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7b709-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7b709-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7b709-120">Request headers</span></span>
|<span data-ttu-id="7b709-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7b709-121">Header</span></span>|<span data-ttu-id="7b709-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7b709-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b709-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7b709-123">Authorization</span></span>|<span data-ttu-id="7b709-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="7b709-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b709-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7b709-125">Accept</span></span>|<span data-ttu-id="7b709-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7b709-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b709-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7b709-127">Request body</span></span>
<span data-ttu-id="7b709-128">В теле запроса добавьте представление объекта windowsPhone81CustomConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7b709-128">In the request body, supply a JSON representation for the windowsPhone81CustomConfiguration object.</span></span>

<span data-ttu-id="7b709-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windowsPhone81CustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="7b709-129">The following table shows the properties that are required when you create the windowsPhone81CustomConfiguration.</span></span>

|<span data-ttu-id="7b709-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7b709-130">Property</span></span>|<span data-ttu-id="7b709-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7b709-131">Type</span></span>|<span data-ttu-id="7b709-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7b709-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b709-133">id</span><span class="sxs-lookup"><span data-stu-id="7b709-133">id</span></span>|<span data-ttu-id="7b709-134">String</span><span class="sxs-lookup"><span data-stu-id="7b709-134">String</span></span>|<span data-ttu-id="7b709-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7b709-135">Key of the entity.</span></span> <span data-ttu-id="7b709-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7b709-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b709-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7b709-137">lastModifiedDateTime</span></span>|<span data-ttu-id="7b709-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b709-138">DateTimeOffset</span></span>|<span data-ttu-id="7b709-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="7b709-139">DateTime the object was last modified.</span></span> <span data-ttu-id="7b709-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7b709-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b709-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7b709-141">roleScopeTagIds</span></span>|<span data-ttu-id="7b709-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="7b709-142">String collection</span></span>|<span data-ttu-id="7b709-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="7b709-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7b709-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7b709-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b709-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="7b709-145">supportsScopeTags</span></span>|<span data-ttu-id="7b709-146">Логический</span><span class="sxs-lookup"><span data-stu-id="7b709-146">Boolean</span></span>|<span data-ttu-id="7b709-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="7b709-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7b709-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="7b709-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7b709-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="7b709-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7b709-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7b709-150">This property is read-only.</span></span> <span data-ttu-id="7b709-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7b709-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b709-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7b709-152">createdDateTime</span></span>|<span data-ttu-id="7b709-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b709-153">DateTimeOffset</span></span>|<span data-ttu-id="7b709-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="7b709-154">DateTime the object was created.</span></span> <span data-ttu-id="7b709-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7b709-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b709-156">description</span><span class="sxs-lookup"><span data-stu-id="7b709-156">description</span></span>|<span data-ttu-id="7b709-157">String</span><span class="sxs-lookup"><span data-stu-id="7b709-157">String</span></span>|<span data-ttu-id="7b709-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7b709-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7b709-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7b709-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b709-160">displayName</span><span class="sxs-lookup"><span data-stu-id="7b709-160">displayName</span></span>|<span data-ttu-id="7b709-161">String</span><span class="sxs-lookup"><span data-stu-id="7b709-161">String</span></span>|<span data-ttu-id="7b709-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7b709-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7b709-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7b709-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b709-164">version</span><span class="sxs-lookup"><span data-stu-id="7b709-164">version</span></span>|<span data-ttu-id="7b709-165">Int32</span><span class="sxs-lookup"><span data-stu-id="7b709-165">Int32</span></span>|<span data-ttu-id="7b709-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7b709-166">Version of the device configuration.</span></span> <span data-ttu-id="7b709-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7b709-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b709-168">omaSettings</span><span class="sxs-lookup"><span data-stu-id="7b709-168">omaSettings</span></span>|<span data-ttu-id="7b709-169">Коллекция [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="7b709-169">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="7b709-170">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="7b709-170">OMA settings.</span></span> <span data-ttu-id="7b709-171">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="7b709-171">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="7b709-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b709-172">Response</span></span>
<span data-ttu-id="7b709-173">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7b709-173">If successful, this method returns a `201 Created` response code and a [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b709-174">Пример</span><span class="sxs-lookup"><span data-stu-id="7b709-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="7b709-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="7b709-175">Request</span></span>
<span data-ttu-id="7b709-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7b709-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 501

{
  "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="7b709-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b709-177">Response</span></span>
<span data-ttu-id="7b709-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7b709-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 673

{
  "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
  "id": "0d98693c-693c-0d98-3c69-980d3c69980d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```




