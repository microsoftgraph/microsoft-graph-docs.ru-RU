---
title: Создание объекта macOSCustomConfiguration
description: Создание объекта macOSCustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d6047eec063d85114fc27a246e39af2d6b791587
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807583"
---
# <a name="create-macoscustomconfiguration"></a><span data-ttu-id="6f7b7-103">Создание объекта macOSCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="6f7b7-103">Create macOSCustomConfiguration</span></span>

> <span data-ttu-id="6f7b7-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6f7b7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6f7b7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f7b7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6f7b7-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6f7b7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6f7b7-107">Создание объекта [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f7b7-107">Create a new [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6f7b7-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6f7b7-108">Prerequisites</span></span>
<span data-ttu-id="6f7b7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f7b7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f7b7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f7b7-111">Permission type</span></span>|<span data-ttu-id="6f7b7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f7b7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f7b7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f7b7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6f7b7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f7b7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6f7b7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f7b7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f7b7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f7b7-116">Not supported.</span></span>|
|<span data-ttu-id="6f7b7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6f7b7-117">Application</span></span>|<span data-ttu-id="6f7b7-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f7b7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f7b7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f7b7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6f7b7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6f7b7-120">Request headers</span></span>
|<span data-ttu-id="6f7b7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6f7b7-121">Header</span></span>|<span data-ttu-id="6f7b7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6f7b7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f7b7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f7b7-123">Authorization</span></span>|<span data-ttu-id="6f7b7-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6f7b7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f7b7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6f7b7-125">Accept</span></span>|<span data-ttu-id="6f7b7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6f7b7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f7b7-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6f7b7-127">Request body</span></span>
<span data-ttu-id="6f7b7-128">В теле запроса добавьте представление объекта macOSCustomConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6f7b7-128">In the request body, supply a JSON representation for the macOSCustomConfiguration object.</span></span>

<span data-ttu-id="6f7b7-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта macOSCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="6f7b7-129">The following table shows the properties that are required when you create the macOSCustomConfiguration.</span></span>

|<span data-ttu-id="6f7b7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f7b7-130">Property</span></span>|<span data-ttu-id="6f7b7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6f7b7-131">Type</span></span>|<span data-ttu-id="6f7b7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6f7b7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f7b7-133">id</span><span class="sxs-lookup"><span data-stu-id="6f7b7-133">id</span></span>|<span data-ttu-id="6f7b7-134">Строка</span><span class="sxs-lookup"><span data-stu-id="6f7b7-134">String</span></span>|<span data-ttu-id="6f7b7-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6f7b7-135">Key of the entity.</span></span> <span data-ttu-id="6f7b7-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f7b7-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f7b7-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6f7b7-137">lastModifiedDateTime</span></span>|<span data-ttu-id="6f7b7-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f7b7-138">DateTimeOffset</span></span>|<span data-ttu-id="6f7b7-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="6f7b7-139">DateTime the object was last modified.</span></span> <span data-ttu-id="6f7b7-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f7b7-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f7b7-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6f7b7-141">roleScopeTagIds</span></span>|<span data-ttu-id="6f7b7-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6f7b7-142">String collection</span></span>|<span data-ttu-id="6f7b7-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="6f7b7-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6f7b7-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f7b7-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f7b7-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6f7b7-145">supportsScopeTags</span></span>|<span data-ttu-id="6f7b7-146">Логический</span><span class="sxs-lookup"><span data-stu-id="6f7b7-146">Boolean</span></span>|<span data-ttu-id="6f7b7-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="6f7b7-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6f7b7-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="6f7b7-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6f7b7-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="6f7b7-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6f7b7-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6f7b7-150">This property is read-only.</span></span> <span data-ttu-id="6f7b7-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f7b7-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f7b7-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6f7b7-152">createdDateTime</span></span>|<span data-ttu-id="6f7b7-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f7b7-153">DateTimeOffset</span></span>|<span data-ttu-id="6f7b7-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="6f7b7-154">DateTime the object was created.</span></span> <span data-ttu-id="6f7b7-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f7b7-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f7b7-156">описание</span><span class="sxs-lookup"><span data-stu-id="6f7b7-156">description</span></span>|<span data-ttu-id="6f7b7-157">Строка</span><span class="sxs-lookup"><span data-stu-id="6f7b7-157">String</span></span>|<span data-ttu-id="6f7b7-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6f7b7-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6f7b7-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f7b7-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f7b7-160">displayName</span><span class="sxs-lookup"><span data-stu-id="6f7b7-160">displayName</span></span>|<span data-ttu-id="6f7b7-161">Строка</span><span class="sxs-lookup"><span data-stu-id="6f7b7-161">String</span></span>|<span data-ttu-id="6f7b7-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6f7b7-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6f7b7-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f7b7-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f7b7-164">version</span><span class="sxs-lookup"><span data-stu-id="6f7b7-164">version</span></span>|<span data-ttu-id="6f7b7-165">Int32</span><span class="sxs-lookup"><span data-stu-id="6f7b7-165">Int32</span></span>|<span data-ttu-id="6f7b7-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6f7b7-166">Version of the device configuration.</span></span> <span data-ttu-id="6f7b7-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f7b7-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f7b7-168">payloadName</span><span class="sxs-lookup"><span data-stu-id="6f7b7-168">payloadName</span></span>|<span data-ttu-id="6f7b7-169">String</span><span class="sxs-lookup"><span data-stu-id="6f7b7-169">String</span></span>|<span data-ttu-id="6f7b7-170">Имя, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="6f7b7-170">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="6f7b7-171">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="6f7b7-171">payloadFileName</span></span>|<span data-ttu-id="6f7b7-172">String</span><span class="sxs-lookup"><span data-stu-id="6f7b7-172">String</span></span>|<span data-ttu-id="6f7b7-173">Имя файла полезных данных (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="6f7b7-173">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="6f7b7-174">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="6f7b7-174">\*.xml).</span></span>|
|<span data-ttu-id="6f7b7-175">payload</span><span class="sxs-lookup"><span data-stu-id="6f7b7-175">payload</span></span>|<span data-ttu-id="6f7b7-176">Binary</span><span class="sxs-lookup"><span data-stu-id="6f7b7-176">Binary</span></span>|<span data-ttu-id="6f7b7-177">Полезные данные</span><span class="sxs-lookup"><span data-stu-id="6f7b7-177">Payload.</span></span> <span data-ttu-id="6f7b7-178">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="6f7b7-178">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="6f7b7-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f7b7-179">Response</span></span>
<span data-ttu-id="6f7b7-180">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6f7b7-180">If successful, this method returns a `201 Created` response code and a [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f7b7-181">Пример</span><span class="sxs-lookup"><span data-stu-id="6f7b7-181">Example</span></span>
### <a name="request"></a><span data-ttu-id="6f7b7-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f7b7-182">Request</span></span>
<span data-ttu-id="6f7b7-183">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f7b7-183">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 437

{
  "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="6f7b7-184">Ответ</span><span class="sxs-lookup"><span data-stu-id="6f7b7-184">Response</span></span>
<span data-ttu-id="6f7b7-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="6f7b7-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





