---
title: Обновление объекта iosCustomConfiguration
description: Обновление свойств объекта iosCustomConfiguration.
author: tfitzmac
ms.openlocfilehash: d79b50003f1a60c3cc0074abefbf0e1907042351
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321975"
---
# <a name="update-ioscustomconfiguration"></a><span data-ttu-id="89d15-103">Обновление объекта iosCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="89d15-103">Update iosCustomConfiguration</span></span>

> <span data-ttu-id="89d15-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="89d15-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="89d15-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89d15-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="89d15-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="89d15-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="89d15-107">Обновление свойств объекта [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="89d15-107">Update the properties of a [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="89d15-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="89d15-108">Prerequisites</span></span>
<span data-ttu-id="89d15-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89d15-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89d15-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="89d15-111">Permission type</span></span>|<span data-ttu-id="89d15-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="89d15-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89d15-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="89d15-113">Delegated (work or school account)</span></span>|<span data-ttu-id="89d15-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89d15-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="89d15-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="89d15-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89d15-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89d15-116">Not supported.</span></span>|
|<span data-ttu-id="89d15-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="89d15-117">Application</span></span>|<span data-ttu-id="89d15-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89d15-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="89d15-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="89d15-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="89d15-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="89d15-120">Request headers</span></span>
|<span data-ttu-id="89d15-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="89d15-121">Header</span></span>|<span data-ttu-id="89d15-122">Значение</span><span class="sxs-lookup"><span data-stu-id="89d15-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89d15-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="89d15-123">Authorization</span></span>|<span data-ttu-id="89d15-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="89d15-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89d15-125">Accept</span><span class="sxs-lookup"><span data-stu-id="89d15-125">Accept</span></span>|<span data-ttu-id="89d15-126">application/json</span><span class="sxs-lookup"><span data-stu-id="89d15-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89d15-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="89d15-127">Request body</span></span>
<span data-ttu-id="89d15-128">В теле запроса добавьте представление объекта [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="89d15-128">In the request body, supply a JSON representation for the [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>

<span data-ttu-id="89d15-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="89d15-129">The following table shows the properties that are required when you create the [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span></span>

|<span data-ttu-id="89d15-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="89d15-130">Property</span></span>|<span data-ttu-id="89d15-131">Тип</span><span class="sxs-lookup"><span data-stu-id="89d15-131">Type</span></span>|<span data-ttu-id="89d15-132">Описание</span><span class="sxs-lookup"><span data-stu-id="89d15-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89d15-133">id</span><span class="sxs-lookup"><span data-stu-id="89d15-133">id</span></span>|<span data-ttu-id="89d15-134">Строка</span><span class="sxs-lookup"><span data-stu-id="89d15-134">String</span></span>|<span data-ttu-id="89d15-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="89d15-135">Key of the entity.</span></span> <span data-ttu-id="89d15-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="89d15-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89d15-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="89d15-137">lastModifiedDateTime</span></span>|<span data-ttu-id="89d15-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89d15-138">DateTimeOffset</span></span>|<span data-ttu-id="89d15-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="89d15-139">DateTime the object was last modified.</span></span> <span data-ttu-id="89d15-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="89d15-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89d15-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="89d15-141">roleScopeTagIds</span></span>|<span data-ttu-id="89d15-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="89d15-142">String collection</span></span>|<span data-ttu-id="89d15-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="89d15-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="89d15-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="89d15-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89d15-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="89d15-145">supportsScopeTags</span></span>|<span data-ttu-id="89d15-146">Boolean.</span><span class="sxs-lookup"><span data-stu-id="89d15-146">Boolean</span></span>|<span data-ttu-id="89d15-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="89d15-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="89d15-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="89d15-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="89d15-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="89d15-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="89d15-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89d15-150">This property is read-only.</span></span> <span data-ttu-id="89d15-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="89d15-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89d15-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="89d15-152">createdDateTime</span></span>|<span data-ttu-id="89d15-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89d15-153">DateTimeOffset</span></span>|<span data-ttu-id="89d15-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="89d15-154">DateTime the object was created.</span></span> <span data-ttu-id="89d15-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="89d15-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89d15-156">описание</span><span class="sxs-lookup"><span data-stu-id="89d15-156">description</span></span>|<span data-ttu-id="89d15-157">Строка</span><span class="sxs-lookup"><span data-stu-id="89d15-157">String</span></span>|<span data-ttu-id="89d15-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="89d15-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="89d15-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="89d15-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89d15-160">displayName</span><span class="sxs-lookup"><span data-stu-id="89d15-160">displayName</span></span>|<span data-ttu-id="89d15-161">Строка</span><span class="sxs-lookup"><span data-stu-id="89d15-161">String</span></span>|<span data-ttu-id="89d15-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="89d15-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="89d15-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="89d15-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89d15-164">version</span><span class="sxs-lookup"><span data-stu-id="89d15-164">version</span></span>|<span data-ttu-id="89d15-165">Int32</span><span class="sxs-lookup"><span data-stu-id="89d15-165">Int32</span></span>|<span data-ttu-id="89d15-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="89d15-166">Version of the device configuration.</span></span> <span data-ttu-id="89d15-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="89d15-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89d15-168">payloadName</span><span class="sxs-lookup"><span data-stu-id="89d15-168">payloadName</span></span>|<span data-ttu-id="89d15-169">String</span><span class="sxs-lookup"><span data-stu-id="89d15-169">String</span></span>|<span data-ttu-id="89d15-170">Имя, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="89d15-170">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="89d15-171">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="89d15-171">payloadFileName</span></span>|<span data-ttu-id="89d15-172">String</span><span class="sxs-lookup"><span data-stu-id="89d15-172">String</span></span>|<span data-ttu-id="89d15-173">Имя файла полезных данных (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="89d15-173">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="89d15-174">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="89d15-174">\*.xml).</span></span>|
|<span data-ttu-id="89d15-175">payload</span><span class="sxs-lookup"><span data-stu-id="89d15-175">payload</span></span>|<span data-ttu-id="89d15-176">Binary</span><span class="sxs-lookup"><span data-stu-id="89d15-176">Binary</span></span>|<span data-ttu-id="89d15-177">Полезные данные</span><span class="sxs-lookup"><span data-stu-id="89d15-177">Payload.</span></span> <span data-ttu-id="89d15-178">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="89d15-178">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="89d15-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="89d15-179">Response</span></span>
<span data-ttu-id="89d15-180">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="89d15-180">If successful, this method returns a `200 OK` response code and an updated [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89d15-181">Пример</span><span class="sxs-lookup"><span data-stu-id="89d15-181">Example</span></span>
### <a name="request"></a><span data-ttu-id="89d15-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="89d15-182">Request</span></span>
<span data-ttu-id="89d15-183">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="89d15-183">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 374

{
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

### <a name="response"></a><span data-ttu-id="89d15-184">Ответ</span><span class="sxs-lookup"><span data-stu-id="89d15-184">Response</span></span>
<span data-ttu-id="89d15-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="89d15-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





