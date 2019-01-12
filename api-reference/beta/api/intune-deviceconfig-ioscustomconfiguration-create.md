---
title: Создание объекта iosCustomConfiguration
description: Создание объекта iosCustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 04855f4aa7c95f714248c17f36126a7afd87c4b6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955263"
---
# <a name="create-ioscustomconfiguration"></a><span data-ttu-id="71c32-103">Создание объекта iosCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="71c32-103">Create iosCustomConfiguration</span></span>

> <span data-ttu-id="71c32-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="71c32-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="71c32-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71c32-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="71c32-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="71c32-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="71c32-107">Создание объекта [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71c32-107">Create a new [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="71c32-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="71c32-108">Prerequisites</span></span>
<span data-ttu-id="71c32-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71c32-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71c32-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71c32-111">Permission type</span></span>|<span data-ttu-id="71c32-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="71c32-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71c32-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71c32-113">Delegated (work or school account)</span></span>|<span data-ttu-id="71c32-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71c32-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="71c32-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71c32-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71c32-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71c32-116">Not supported.</span></span>|
|<span data-ttu-id="71c32-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="71c32-117">Application</span></span>|<span data-ttu-id="71c32-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71c32-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="71c32-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71c32-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="71c32-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="71c32-120">Request headers</span></span>
|<span data-ttu-id="71c32-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="71c32-121">Header</span></span>|<span data-ttu-id="71c32-122">Значение</span><span class="sxs-lookup"><span data-stu-id="71c32-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71c32-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="71c32-123">Authorization</span></span>|<span data-ttu-id="71c32-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="71c32-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71c32-125">Accept</span><span class="sxs-lookup"><span data-stu-id="71c32-125">Accept</span></span>|<span data-ttu-id="71c32-126">application/json</span><span class="sxs-lookup"><span data-stu-id="71c32-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71c32-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="71c32-127">Request body</span></span>
<span data-ttu-id="71c32-128">В теле запроса добавьте представление объекта iosCustomConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="71c32-128">In the request body, supply a JSON representation for the iosCustomConfiguration object.</span></span>

<span data-ttu-id="71c32-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта iosCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="71c32-129">The following table shows the properties that are required when you create the iosCustomConfiguration.</span></span>

|<span data-ttu-id="71c32-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="71c32-130">Property</span></span>|<span data-ttu-id="71c32-131">Тип</span><span class="sxs-lookup"><span data-stu-id="71c32-131">Type</span></span>|<span data-ttu-id="71c32-132">Описание</span><span class="sxs-lookup"><span data-stu-id="71c32-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71c32-133">id</span><span class="sxs-lookup"><span data-stu-id="71c32-133">id</span></span>|<span data-ttu-id="71c32-134">String</span><span class="sxs-lookup"><span data-stu-id="71c32-134">String</span></span>|<span data-ttu-id="71c32-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="71c32-135">Key of the entity.</span></span> <span data-ttu-id="71c32-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71c32-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71c32-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="71c32-137">lastModifiedDateTime</span></span>|<span data-ttu-id="71c32-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71c32-138">DateTimeOffset</span></span>|<span data-ttu-id="71c32-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="71c32-139">DateTime the object was last modified.</span></span> <span data-ttu-id="71c32-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71c32-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71c32-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="71c32-141">roleScopeTagIds</span></span>|<span data-ttu-id="71c32-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="71c32-142">String collection</span></span>|<span data-ttu-id="71c32-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="71c32-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="71c32-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71c32-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71c32-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="71c32-145">supportsScopeTags</span></span>|<span data-ttu-id="71c32-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="71c32-146">Boolean</span></span>|<span data-ttu-id="71c32-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="71c32-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="71c32-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="71c32-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="71c32-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="71c32-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="71c32-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="71c32-150">This property is read-only.</span></span> <span data-ttu-id="71c32-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71c32-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71c32-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="71c32-152">createdDateTime</span></span>|<span data-ttu-id="71c32-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71c32-153">DateTimeOffset</span></span>|<span data-ttu-id="71c32-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="71c32-154">DateTime the object was created.</span></span> <span data-ttu-id="71c32-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71c32-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71c32-156">описание</span><span class="sxs-lookup"><span data-stu-id="71c32-156">description</span></span>|<span data-ttu-id="71c32-157">String</span><span class="sxs-lookup"><span data-stu-id="71c32-157">String</span></span>|<span data-ttu-id="71c32-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="71c32-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="71c32-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71c32-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71c32-160">displayName</span><span class="sxs-lookup"><span data-stu-id="71c32-160">displayName</span></span>|<span data-ttu-id="71c32-161">String</span><span class="sxs-lookup"><span data-stu-id="71c32-161">String</span></span>|<span data-ttu-id="71c32-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="71c32-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="71c32-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71c32-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71c32-164">version</span><span class="sxs-lookup"><span data-stu-id="71c32-164">version</span></span>|<span data-ttu-id="71c32-165">Int32</span><span class="sxs-lookup"><span data-stu-id="71c32-165">Int32</span></span>|<span data-ttu-id="71c32-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="71c32-166">Version of the device configuration.</span></span> <span data-ttu-id="71c32-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71c32-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71c32-168">payloadName</span><span class="sxs-lookup"><span data-stu-id="71c32-168">payloadName</span></span>|<span data-ttu-id="71c32-169">String</span><span class="sxs-lookup"><span data-stu-id="71c32-169">String</span></span>|<span data-ttu-id="71c32-170">Имя, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="71c32-170">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="71c32-171">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="71c32-171">payloadFileName</span></span>|<span data-ttu-id="71c32-172">String</span><span class="sxs-lookup"><span data-stu-id="71c32-172">String</span></span>|<span data-ttu-id="71c32-173">Имя файла полезных данных (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="71c32-173">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="71c32-174">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="71c32-174">\*.xml).</span></span>|
|<span data-ttu-id="71c32-175">payload</span><span class="sxs-lookup"><span data-stu-id="71c32-175">payload</span></span>|<span data-ttu-id="71c32-176">Binary</span><span class="sxs-lookup"><span data-stu-id="71c32-176">Binary</span></span>|<span data-ttu-id="71c32-177">Полезные данные</span><span class="sxs-lookup"><span data-stu-id="71c32-177">Payload.</span></span> <span data-ttu-id="71c32-178">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="71c32-178">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="71c32-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="71c32-179">Response</span></span>
<span data-ttu-id="71c32-180">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="71c32-180">If successful, this method returns a `201 Created` response code and a [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71c32-181">Пример</span><span class="sxs-lookup"><span data-stu-id="71c32-181">Example</span></span>
### <a name="request"></a><span data-ttu-id="71c32-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="71c32-182">Request</span></span>
<span data-ttu-id="71c32-183">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="71c32-183">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 435

{
  "@odata.type": "#microsoft.graph.iosCustomConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="71c32-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="71c32-184">Response</span></span>
<span data-ttu-id="71c32-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="71c32-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





