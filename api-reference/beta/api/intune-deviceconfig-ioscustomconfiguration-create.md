---
title: Создание объекта iosCustomConfiguration
description: Создание объекта iosCustomConfiguration.
author: tfitzmac
ms.openlocfilehash: e22a670316ca7ffb4216c45cab5e8f3e6d7f3d65
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343311"
---
# <a name="create-ioscustomconfiguration"></a><span data-ttu-id="2f388-103">Создание объекта iosCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="2f388-103">Create iosCustomConfiguration</span></span>

> <span data-ttu-id="2f388-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2f388-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2f388-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f388-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2f388-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2f388-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2f388-107">Создание объекта [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2f388-107">Create a new [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2f388-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2f388-108">Prerequisites</span></span>
<span data-ttu-id="2f388-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f388-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f388-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2f388-111">Permission type</span></span>|<span data-ttu-id="2f388-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2f388-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f388-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2f388-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2f388-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f388-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2f388-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2f388-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f388-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f388-116">Not supported.</span></span>|
|<span data-ttu-id="2f388-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2f388-117">Application</span></span>|<span data-ttu-id="2f388-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f388-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f388-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2f388-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2f388-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2f388-120">Request headers</span></span>
|<span data-ttu-id="2f388-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2f388-121">Header</span></span>|<span data-ttu-id="2f388-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2f388-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f388-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2f388-123">Authorization</span></span>|<span data-ttu-id="2f388-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2f388-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f388-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2f388-125">Accept</span></span>|<span data-ttu-id="2f388-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2f388-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f388-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2f388-127">Request body</span></span>
<span data-ttu-id="2f388-128">В теле запроса добавьте представление объекта iosCustomConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2f388-128">In the request body, supply a JSON representation for the iosCustomConfiguration object.</span></span>

<span data-ttu-id="2f388-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта iosCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="2f388-129">The following table shows the properties that are required when you create the iosCustomConfiguration.</span></span>

|<span data-ttu-id="2f388-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2f388-130">Property</span></span>|<span data-ttu-id="2f388-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2f388-131">Type</span></span>|<span data-ttu-id="2f388-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2f388-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f388-133">id</span><span class="sxs-lookup"><span data-stu-id="2f388-133">id</span></span>|<span data-ttu-id="2f388-134">Строка</span><span class="sxs-lookup"><span data-stu-id="2f388-134">String</span></span>|<span data-ttu-id="2f388-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2f388-135">Key of the entity.</span></span> <span data-ttu-id="2f388-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2f388-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f388-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2f388-137">lastModifiedDateTime</span></span>|<span data-ttu-id="2f388-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f388-138">DateTimeOffset</span></span>|<span data-ttu-id="2f388-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="2f388-139">DateTime the object was last modified.</span></span> <span data-ttu-id="2f388-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2f388-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f388-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2f388-141">roleScopeTagIds</span></span>|<span data-ttu-id="2f388-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2f388-142">String collection</span></span>|<span data-ttu-id="2f388-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="2f388-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2f388-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2f388-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f388-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="2f388-145">supportsScopeTags</span></span>|<span data-ttu-id="2f388-146">Boolean.</span><span class="sxs-lookup"><span data-stu-id="2f388-146">Boolean</span></span>|<span data-ttu-id="2f388-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="2f388-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2f388-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="2f388-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2f388-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="2f388-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2f388-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2f388-150">This property is read-only.</span></span> <span data-ttu-id="2f388-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2f388-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f388-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2f388-152">createdDateTime</span></span>|<span data-ttu-id="2f388-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f388-153">DateTimeOffset</span></span>|<span data-ttu-id="2f388-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="2f388-154">DateTime the object was created.</span></span> <span data-ttu-id="2f388-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2f388-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f388-156">описание</span><span class="sxs-lookup"><span data-stu-id="2f388-156">description</span></span>|<span data-ttu-id="2f388-157">Строка</span><span class="sxs-lookup"><span data-stu-id="2f388-157">String</span></span>|<span data-ttu-id="2f388-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2f388-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2f388-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2f388-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f388-160">displayName</span><span class="sxs-lookup"><span data-stu-id="2f388-160">displayName</span></span>|<span data-ttu-id="2f388-161">Строка</span><span class="sxs-lookup"><span data-stu-id="2f388-161">String</span></span>|<span data-ttu-id="2f388-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2f388-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2f388-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2f388-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f388-164">version</span><span class="sxs-lookup"><span data-stu-id="2f388-164">version</span></span>|<span data-ttu-id="2f388-165">Int32</span><span class="sxs-lookup"><span data-stu-id="2f388-165">Int32</span></span>|<span data-ttu-id="2f388-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2f388-166">Version of the device configuration.</span></span> <span data-ttu-id="2f388-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2f388-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f388-168">payloadName</span><span class="sxs-lookup"><span data-stu-id="2f388-168">payloadName</span></span>|<span data-ttu-id="2f388-169">String</span><span class="sxs-lookup"><span data-stu-id="2f388-169">String</span></span>|<span data-ttu-id="2f388-170">Имя, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="2f388-170">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="2f388-171">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="2f388-171">payloadFileName</span></span>|<span data-ttu-id="2f388-172">String</span><span class="sxs-lookup"><span data-stu-id="2f388-172">String</span></span>|<span data-ttu-id="2f388-173">Имя файла полезных данных (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="2f388-173">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="2f388-174">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="2f388-174">\*.xml).</span></span>|
|<span data-ttu-id="2f388-175">payload</span><span class="sxs-lookup"><span data-stu-id="2f388-175">payload</span></span>|<span data-ttu-id="2f388-176">Binary</span><span class="sxs-lookup"><span data-stu-id="2f388-176">Binary</span></span>|<span data-ttu-id="2f388-177">Полезные данные</span><span class="sxs-lookup"><span data-stu-id="2f388-177">Payload.</span></span> <span data-ttu-id="2f388-178">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="2f388-178">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="2f388-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f388-179">Response</span></span>
<span data-ttu-id="2f388-180">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2f388-180">If successful, this method returns a `201 Created` response code and a [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f388-181">Пример</span><span class="sxs-lookup"><span data-stu-id="2f388-181">Example</span></span>
### <a name="request"></a><span data-ttu-id="2f388-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f388-182">Request</span></span>
<span data-ttu-id="2f388-183">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2f388-183">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2f388-184">Ответ</span><span class="sxs-lookup"><span data-stu-id="2f388-184">Response</span></span>
<span data-ttu-id="2f388-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2f388-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





