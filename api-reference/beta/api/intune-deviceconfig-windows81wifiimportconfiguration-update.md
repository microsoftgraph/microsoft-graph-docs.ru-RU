---
title: Обновление windows81WifiImportConfiguration
description: Обновление свойства объекта windows81WifiImportConfiguration.
author: tfitzmac
ms.openlocfilehash: 043d68ef67d495ddde96bb7dc4066a7e122e718d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27327918"
---
# <a name="update-windows81wifiimportconfiguration"></a><span data-ttu-id="53bae-103">Обновление windows81WifiImportConfiguration</span><span class="sxs-lookup"><span data-stu-id="53bae-103">Update windows81WifiImportConfiguration</span></span>

> <span data-ttu-id="53bae-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="53bae-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="53bae-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53bae-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="53bae-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="53bae-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="53bae-107">Обновление свойства объекта [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="53bae-107">Update the properties of a [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="53bae-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="53bae-108">Prerequisites</span></span>
<span data-ttu-id="53bae-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53bae-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53bae-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="53bae-111">Permission type</span></span>|<span data-ttu-id="53bae-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="53bae-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53bae-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="53bae-113">Delegated (work or school account)</span></span>|<span data-ttu-id="53bae-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53bae-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="53bae-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="53bae-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53bae-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53bae-116">Not supported.</span></span>|
|<span data-ttu-id="53bae-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="53bae-117">Application</span></span>|<span data-ttu-id="53bae-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53bae-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="53bae-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53bae-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="53bae-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="53bae-120">Request headers</span></span>
|<span data-ttu-id="53bae-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="53bae-121">Header</span></span>|<span data-ttu-id="53bae-122">Значение</span><span class="sxs-lookup"><span data-stu-id="53bae-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53bae-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="53bae-123">Authorization</span></span>|<span data-ttu-id="53bae-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="53bae-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53bae-125">Accept</span><span class="sxs-lookup"><span data-stu-id="53bae-125">Accept</span></span>|<span data-ttu-id="53bae-126">application/json</span><span class="sxs-lookup"><span data-stu-id="53bae-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53bae-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="53bae-127">Request body</span></span>
<span data-ttu-id="53bae-128">В тексте запроса укажите представление JSON для объекта [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="53bae-128">In the request body, supply a JSON representation for the [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object.</span></span>

<span data-ttu-id="53bae-129">В следующей таблице показаны свойства, которые необходимы для создания [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="53bae-129">The following table shows the properties that are required when you create the [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md).</span></span>

|<span data-ttu-id="53bae-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="53bae-130">Property</span></span>|<span data-ttu-id="53bae-131">Тип</span><span class="sxs-lookup"><span data-stu-id="53bae-131">Type</span></span>|<span data-ttu-id="53bae-132">Описание</span><span class="sxs-lookup"><span data-stu-id="53bae-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53bae-133">id</span><span class="sxs-lookup"><span data-stu-id="53bae-133">id</span></span>|<span data-ttu-id="53bae-134">Строка</span><span class="sxs-lookup"><span data-stu-id="53bae-134">String</span></span>|<span data-ttu-id="53bae-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="53bae-135">Key of the entity.</span></span> <span data-ttu-id="53bae-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="53bae-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="53bae-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="53bae-137">lastModifiedDateTime</span></span>|<span data-ttu-id="53bae-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53bae-138">DateTimeOffset</span></span>|<span data-ttu-id="53bae-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="53bae-139">DateTime the object was last modified.</span></span> <span data-ttu-id="53bae-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="53bae-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="53bae-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="53bae-141">roleScopeTagIds</span></span>|<span data-ttu-id="53bae-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="53bae-142">String collection</span></span>|<span data-ttu-id="53bae-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="53bae-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="53bae-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="53bae-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="53bae-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="53bae-145">supportsScopeTags</span></span>|<span data-ttu-id="53bae-146">Boolean.</span><span class="sxs-lookup"><span data-stu-id="53bae-146">Boolean</span></span>|<span data-ttu-id="53bae-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="53bae-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="53bae-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="53bae-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="53bae-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="53bae-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="53bae-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="53bae-150">This property is read-only.</span></span> <span data-ttu-id="53bae-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="53bae-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="53bae-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="53bae-152">createdDateTime</span></span>|<span data-ttu-id="53bae-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53bae-153">DateTimeOffset</span></span>|<span data-ttu-id="53bae-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="53bae-154">DateTime the object was created.</span></span> <span data-ttu-id="53bae-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="53bae-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="53bae-156">описание</span><span class="sxs-lookup"><span data-stu-id="53bae-156">description</span></span>|<span data-ttu-id="53bae-157">Строка</span><span class="sxs-lookup"><span data-stu-id="53bae-157">String</span></span>|<span data-ttu-id="53bae-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="53bae-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="53bae-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="53bae-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="53bae-160">displayName</span><span class="sxs-lookup"><span data-stu-id="53bae-160">displayName</span></span>|<span data-ttu-id="53bae-161">Строка</span><span class="sxs-lookup"><span data-stu-id="53bae-161">String</span></span>|<span data-ttu-id="53bae-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="53bae-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="53bae-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="53bae-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="53bae-164">version</span><span class="sxs-lookup"><span data-stu-id="53bae-164">version</span></span>|<span data-ttu-id="53bae-165">Int32</span><span class="sxs-lookup"><span data-stu-id="53bae-165">Int32</span></span>|<span data-ttu-id="53bae-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="53bae-166">Version of the device configuration.</span></span> <span data-ttu-id="53bae-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="53bae-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="53bae-168">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="53bae-168">payloadFileName</span></span>|<span data-ttu-id="53bae-169">String</span><span class="sxs-lookup"><span data-stu-id="53bae-169">String</span></span>|<span data-ttu-id="53bae-170">Имя файла полезной нагрузки (\*.xml).</span><span class="sxs-lookup"><span data-stu-id="53bae-170">Payload file name (\*.xml).</span></span>|
|<span data-ttu-id="53bae-171">Имя_профиля</span><span class="sxs-lookup"><span data-stu-id="53bae-171">profileName</span></span>|<span data-ttu-id="53bae-172">String.</span><span class="sxs-lookup"><span data-stu-id="53bae-172">String</span></span>|<span data-ttu-id="53bae-173">Имя профиля, отображаемое в пользовательском Интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="53bae-173">Profile name displayed in the UI.</span></span>|
|<span data-ttu-id="53bae-174">payload</span><span class="sxs-lookup"><span data-stu-id="53bae-174">payload</span></span>|<span data-ttu-id="53bae-175">Binary</span><span class="sxs-lookup"><span data-stu-id="53bae-175">Binary</span></span>|<span data-ttu-id="53bae-176">Полезные данные</span><span class="sxs-lookup"><span data-stu-id="53bae-176">Payload.</span></span> <span data-ttu-id="53bae-177">(UTF8 закодированный массив байтов).</span><span class="sxs-lookup"><span data-stu-id="53bae-177">(UTF8 encoded byte array).</span></span> <span data-ttu-id="53bae-178">Это XML-файл, сохраненный на устройство, используемое для подключения к конечной точке Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="53bae-178">This is the XML file saved on the device you used to connect to the Wi-Fi endpoint.</span></span>|



## <a name="response"></a><span data-ttu-id="53bae-179">Ответ</span><span class="sxs-lookup"><span data-stu-id="53bae-179">Response</span></span>
<span data-ttu-id="53bae-180">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="53bae-180">If successful, this method returns a `200 OK` response code and an updated [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53bae-181">Пример</span><span class="sxs-lookup"><span data-stu-id="53bae-181">Example</span></span>
### <a name="request"></a><span data-ttu-id="53bae-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="53bae-182">Request</span></span>
<span data-ttu-id="53bae-183">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="53bae-183">Here is an example of the request.</span></span>
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
  "payloadFileName": "Payload File Name value",
  "profileName": "Profile Name value",
  "payload": "cGF5bG9hZA=="
}
```

### <a name="response"></a><span data-ttu-id="53bae-184">Ответ</span><span class="sxs-lookup"><span data-stu-id="53bae-184">Response</span></span>
<span data-ttu-id="53bae-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="53bae-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 553

{
  "@odata.type": "#microsoft.graph.windows81WifiImportConfiguration",
  "id": "534a2f07-2f07-534a-072f-4a53072f4a53",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadFileName": "Payload File Name value",
  "profileName": "Profile Name value",
  "payload": "cGF5bG9hZA=="
}
```





