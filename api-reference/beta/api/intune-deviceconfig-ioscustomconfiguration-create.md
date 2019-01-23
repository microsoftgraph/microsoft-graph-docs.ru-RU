---
title: Создание объекта iosCustomConfiguration
description: Создание объекта iosCustomConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7b5461d7267a2aa9b0d27439ee98217e82ab886c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421349"
---
# <a name="create-ioscustomconfiguration"></a><span data-ttu-id="ecd82-103">Создание объекта iosCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="ecd82-103">Create iosCustomConfiguration</span></span>

> <span data-ttu-id="ecd82-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ecd82-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ecd82-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ecd82-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ecd82-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ecd82-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ecd82-107">Создание объекта [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ecd82-107">Create a new [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ecd82-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ecd82-108">Prerequisites</span></span>
<span data-ttu-id="ecd82-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ecd82-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ecd82-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ecd82-111">Permission type</span></span>|<span data-ttu-id="ecd82-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ecd82-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ecd82-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ecd82-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ecd82-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ecd82-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ecd82-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ecd82-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ecd82-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ecd82-116">Not supported.</span></span>|
|<span data-ttu-id="ecd82-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ecd82-117">Application</span></span>|<span data-ttu-id="ecd82-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ecd82-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ecd82-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ecd82-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ecd82-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ecd82-120">Request headers</span></span>
|<span data-ttu-id="ecd82-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ecd82-121">Header</span></span>|<span data-ttu-id="ecd82-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ecd82-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ecd82-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ecd82-123">Authorization</span></span>|<span data-ttu-id="ecd82-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ecd82-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ecd82-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ecd82-125">Accept</span></span>|<span data-ttu-id="ecd82-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ecd82-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ecd82-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ecd82-127">Request body</span></span>
<span data-ttu-id="ecd82-128">В теле запроса добавьте представление объекта iosCustomConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ecd82-128">In the request body, supply a JSON representation for the iosCustomConfiguration object.</span></span>

<span data-ttu-id="ecd82-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта iosCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ecd82-129">The following table shows the properties that are required when you create the iosCustomConfiguration.</span></span>

|<span data-ttu-id="ecd82-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ecd82-130">Property</span></span>|<span data-ttu-id="ecd82-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ecd82-131">Type</span></span>|<span data-ttu-id="ecd82-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ecd82-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ecd82-133">id</span><span class="sxs-lookup"><span data-stu-id="ecd82-133">id</span></span>|<span data-ttu-id="ecd82-134">String</span><span class="sxs-lookup"><span data-stu-id="ecd82-134">String</span></span>|<span data-ttu-id="ecd82-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ecd82-135">Key of the entity.</span></span> <span data-ttu-id="ecd82-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ecd82-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ecd82-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ecd82-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ecd82-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ecd82-138">DateTimeOffset</span></span>|<span data-ttu-id="ecd82-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ecd82-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ecd82-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ecd82-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ecd82-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ecd82-141">roleScopeTagIds</span></span>|<span data-ttu-id="ecd82-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ecd82-142">String collection</span></span>|<span data-ttu-id="ecd82-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="ecd82-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ecd82-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ecd82-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ecd82-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ecd82-145">supportsScopeTags</span></span>|<span data-ttu-id="ecd82-146">Логический</span><span class="sxs-lookup"><span data-stu-id="ecd82-146">Boolean</span></span>|<span data-ttu-id="ecd82-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="ecd82-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ecd82-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="ecd82-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ecd82-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="ecd82-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ecd82-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ecd82-150">This property is read-only.</span></span> <span data-ttu-id="ecd82-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ecd82-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ecd82-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ecd82-152">createdDateTime</span></span>|<span data-ttu-id="ecd82-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ecd82-153">DateTimeOffset</span></span>|<span data-ttu-id="ecd82-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ecd82-154">DateTime the object was created.</span></span> <span data-ttu-id="ecd82-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ecd82-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ecd82-156">description</span><span class="sxs-lookup"><span data-stu-id="ecd82-156">description</span></span>|<span data-ttu-id="ecd82-157">String</span><span class="sxs-lookup"><span data-stu-id="ecd82-157">String</span></span>|<span data-ttu-id="ecd82-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ecd82-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ecd82-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ecd82-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ecd82-160">displayName</span><span class="sxs-lookup"><span data-stu-id="ecd82-160">displayName</span></span>|<span data-ttu-id="ecd82-161">String</span><span class="sxs-lookup"><span data-stu-id="ecd82-161">String</span></span>|<span data-ttu-id="ecd82-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ecd82-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ecd82-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ecd82-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ecd82-164">version</span><span class="sxs-lookup"><span data-stu-id="ecd82-164">version</span></span>|<span data-ttu-id="ecd82-165">Int32</span><span class="sxs-lookup"><span data-stu-id="ecd82-165">Int32</span></span>|<span data-ttu-id="ecd82-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ecd82-166">Version of the device configuration.</span></span> <span data-ttu-id="ecd82-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ecd82-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ecd82-168">payloadName</span><span class="sxs-lookup"><span data-stu-id="ecd82-168">payloadName</span></span>|<span data-ttu-id="ecd82-169">String</span><span class="sxs-lookup"><span data-stu-id="ecd82-169">String</span></span>|<span data-ttu-id="ecd82-170">Имя, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="ecd82-170">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="ecd82-171">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="ecd82-171">payloadFileName</span></span>|<span data-ttu-id="ecd82-172">String</span><span class="sxs-lookup"><span data-stu-id="ecd82-172">String</span></span>|<span data-ttu-id="ecd82-173">Имя файла полезных данных (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="ecd82-173">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="ecd82-174">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="ecd82-174">\*.xml).</span></span>|
|<span data-ttu-id="ecd82-175">payload</span><span class="sxs-lookup"><span data-stu-id="ecd82-175">payload</span></span>|<span data-ttu-id="ecd82-176">Binary</span><span class="sxs-lookup"><span data-stu-id="ecd82-176">Binary</span></span>|<span data-ttu-id="ecd82-177">Полезные данные</span><span class="sxs-lookup"><span data-stu-id="ecd82-177">Payload.</span></span> <span data-ttu-id="ecd82-178">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="ecd82-178">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="ecd82-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="ecd82-179">Response</span></span>
<span data-ttu-id="ecd82-180">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ecd82-180">If successful, this method returns a `201 Created` response code and a [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ecd82-181">Пример</span><span class="sxs-lookup"><span data-stu-id="ecd82-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="ecd82-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="ecd82-182">Request</span></span>
<span data-ttu-id="ecd82-183">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ecd82-183">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 371

{
  "@odata.type": "#microsoft.graph.iosCustomConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```

### <a name="response"></a><span data-ttu-id="ecd82-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="ecd82-184">Response</span></span>
<span data-ttu-id="ecd82-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ecd82-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 543

{
  "@odata.type": "#microsoft.graph.iosCustomConfiguration",
  "id": "f34428e3-28e3-f344-e328-44f3e32844f3",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```




