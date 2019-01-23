---
title: Обновление объекта macOSCustomConfiguration
description: Обновление свойств объекта macOSCustomConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c0fc777a86b751a187cd15b651a9bd4d352486e9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405165"
---
# <a name="update-macoscustomconfiguration"></a><span data-ttu-id="4c5c7-103">Обновление объекта macOSCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="4c5c7-103">Update macOSCustomConfiguration</span></span>

> <span data-ttu-id="4c5c7-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4c5c7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4c5c7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c5c7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4c5c7-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4c5c7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c5c7-107">Обновление свойств объекта [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4c5c7-107">Update the properties of a [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4c5c7-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4c5c7-108">Prerequisites</span></span>
<span data-ttu-id="4c5c7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4c5c7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4c5c7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c5c7-111">Permission type</span></span>|<span data-ttu-id="4c5c7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c5c7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c5c7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c5c7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4c5c7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c5c7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4c5c7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c5c7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c5c7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c5c7-116">Not supported.</span></span>|
|<span data-ttu-id="4c5c7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4c5c7-117">Application</span></span>|<span data-ttu-id="4c5c7-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c5c7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c5c7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c5c7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="4c5c7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c5c7-120">Request headers</span></span>
|<span data-ttu-id="4c5c7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4c5c7-121">Header</span></span>|<span data-ttu-id="4c5c7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4c5c7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c5c7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c5c7-123">Authorization</span></span>|<span data-ttu-id="4c5c7-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4c5c7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c5c7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4c5c7-125">Accept</span></span>|<span data-ttu-id="4c5c7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4c5c7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c5c7-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4c5c7-127">Request body</span></span>
<span data-ttu-id="4c5c7-128">В теле запроса добавьте представление объекта [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4c5c7-128">In the request body, supply a JSON representation for the [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object.</span></span>

<span data-ttu-id="4c5c7-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4c5c7-129">The following table shows the properties that are required when you create the [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span></span>

|<span data-ttu-id="4c5c7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c5c7-130">Property</span></span>|<span data-ttu-id="4c5c7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4c5c7-131">Type</span></span>|<span data-ttu-id="4c5c7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4c5c7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c5c7-133">id</span><span class="sxs-lookup"><span data-stu-id="4c5c7-133">id</span></span>|<span data-ttu-id="4c5c7-134">String</span><span class="sxs-lookup"><span data-stu-id="4c5c7-134">String</span></span>|<span data-ttu-id="4c5c7-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4c5c7-135">Key of the entity.</span></span> <span data-ttu-id="4c5c7-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4c5c7-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c5c7-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4c5c7-137">lastModifiedDateTime</span></span>|<span data-ttu-id="4c5c7-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c5c7-138">DateTimeOffset</span></span>|<span data-ttu-id="4c5c7-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="4c5c7-139">DateTime the object was last modified.</span></span> <span data-ttu-id="4c5c7-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4c5c7-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c5c7-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4c5c7-141">roleScopeTagIds</span></span>|<span data-ttu-id="4c5c7-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4c5c7-142">String collection</span></span>|<span data-ttu-id="4c5c7-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="4c5c7-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4c5c7-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4c5c7-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c5c7-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="4c5c7-145">supportsScopeTags</span></span>|<span data-ttu-id="4c5c7-146">Логический</span><span class="sxs-lookup"><span data-stu-id="4c5c7-146">Boolean</span></span>|<span data-ttu-id="4c5c7-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="4c5c7-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4c5c7-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="4c5c7-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4c5c7-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="4c5c7-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4c5c7-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4c5c7-150">This property is read-only.</span></span> <span data-ttu-id="4c5c7-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4c5c7-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c5c7-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4c5c7-152">createdDateTime</span></span>|<span data-ttu-id="4c5c7-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c5c7-153">DateTimeOffset</span></span>|<span data-ttu-id="4c5c7-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="4c5c7-154">DateTime the object was created.</span></span> <span data-ttu-id="4c5c7-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4c5c7-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c5c7-156">description</span><span class="sxs-lookup"><span data-stu-id="4c5c7-156">description</span></span>|<span data-ttu-id="4c5c7-157">String</span><span class="sxs-lookup"><span data-stu-id="4c5c7-157">String</span></span>|<span data-ttu-id="4c5c7-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4c5c7-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4c5c7-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4c5c7-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c5c7-160">displayName</span><span class="sxs-lookup"><span data-stu-id="4c5c7-160">displayName</span></span>|<span data-ttu-id="4c5c7-161">String</span><span class="sxs-lookup"><span data-stu-id="4c5c7-161">String</span></span>|<span data-ttu-id="4c5c7-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4c5c7-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4c5c7-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4c5c7-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c5c7-164">version</span><span class="sxs-lookup"><span data-stu-id="4c5c7-164">version</span></span>|<span data-ttu-id="4c5c7-165">Int32</span><span class="sxs-lookup"><span data-stu-id="4c5c7-165">Int32</span></span>|<span data-ttu-id="4c5c7-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4c5c7-166">Version of the device configuration.</span></span> <span data-ttu-id="4c5c7-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4c5c7-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c5c7-168">payloadName</span><span class="sxs-lookup"><span data-stu-id="4c5c7-168">payloadName</span></span>|<span data-ttu-id="4c5c7-169">String</span><span class="sxs-lookup"><span data-stu-id="4c5c7-169">String</span></span>|<span data-ttu-id="4c5c7-170">Имя, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="4c5c7-170">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="4c5c7-171">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="4c5c7-171">payloadFileName</span></span>|<span data-ttu-id="4c5c7-172">String</span><span class="sxs-lookup"><span data-stu-id="4c5c7-172">String</span></span>|<span data-ttu-id="4c5c7-173">Имя файла полезных данных (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="4c5c7-173">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="4c5c7-174">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="4c5c7-174">\*.xml).</span></span>|
|<span data-ttu-id="4c5c7-175">payload</span><span class="sxs-lookup"><span data-stu-id="4c5c7-175">payload</span></span>|<span data-ttu-id="4c5c7-176">Binary</span><span class="sxs-lookup"><span data-stu-id="4c5c7-176">Binary</span></span>|<span data-ttu-id="4c5c7-177">Полезные данные</span><span class="sxs-lookup"><span data-stu-id="4c5c7-177">Payload.</span></span> <span data-ttu-id="4c5c7-178">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="4c5c7-178">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="4c5c7-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c5c7-179">Response</span></span>
<span data-ttu-id="4c5c7-180">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4c5c7-180">If successful, this method returns a `200 OK` response code and an updated [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c5c7-181">Пример</span><span class="sxs-lookup"><span data-stu-id="4c5c7-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="4c5c7-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c5c7-182">Request</span></span>
<span data-ttu-id="4c5c7-183">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c5c7-183">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 373

{
  "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="4c5c7-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c5c7-184">Response</span></span>
<span data-ttu-id="4c5c7-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4c5c7-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 545

{
  "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
  "id": "a253835d-835d-a253-5d83-53a25d8353a2",
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




