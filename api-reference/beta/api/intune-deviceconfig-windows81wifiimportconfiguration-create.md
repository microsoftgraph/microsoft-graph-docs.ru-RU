---
title: Создание windows81WifiImportConfiguration
description: Создание нового объекта windows81WifiImportConfiguration.
author: tfitzmac
ms.openlocfilehash: 377f7e44becbcc6e4e3816a843a8898700ac67b7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356499"
---
# <a name="create-windows81wifiimportconfiguration"></a><span data-ttu-id="6195a-103">Создание windows81WifiImportConfiguration</span><span class="sxs-lookup"><span data-stu-id="6195a-103">Create windows81WifiImportConfiguration</span></span>

> <span data-ttu-id="6195a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6195a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6195a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6195a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6195a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6195a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6195a-107">Создание нового объекта [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="6195a-107">Create a new [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6195a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6195a-108">Prerequisites</span></span>
<span data-ttu-id="6195a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6195a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6195a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6195a-111">Permission type</span></span>|<span data-ttu-id="6195a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6195a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6195a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6195a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6195a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6195a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6195a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6195a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6195a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6195a-116">Not supported.</span></span>|
|<span data-ttu-id="6195a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6195a-117">Application</span></span>|<span data-ttu-id="6195a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6195a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6195a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6195a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6195a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6195a-120">Request headers</span></span>
|<span data-ttu-id="6195a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6195a-121">Header</span></span>|<span data-ttu-id="6195a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6195a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6195a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6195a-123">Authorization</span></span>|<span data-ttu-id="6195a-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6195a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6195a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6195a-125">Accept</span></span>|<span data-ttu-id="6195a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6195a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6195a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6195a-127">Request body</span></span>
<span data-ttu-id="6195a-128">В тексте запроса укажите представление JSON для объекта windows81WifiImportConfiguration.</span><span class="sxs-lookup"><span data-stu-id="6195a-128">In the request body, supply a JSON representation for the windows81WifiImportConfiguration object.</span></span>

<span data-ttu-id="6195a-129">В следующей таблице показаны свойства, которые необходимы для создания windows81WifiImportConfiguration.</span><span class="sxs-lookup"><span data-stu-id="6195a-129">The following table shows the properties that are required when you create the windows81WifiImportConfiguration.</span></span>

|<span data-ttu-id="6195a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6195a-130">Property</span></span>|<span data-ttu-id="6195a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6195a-131">Type</span></span>|<span data-ttu-id="6195a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6195a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6195a-133">id</span><span class="sxs-lookup"><span data-stu-id="6195a-133">id</span></span>|<span data-ttu-id="6195a-134">Строка</span><span class="sxs-lookup"><span data-stu-id="6195a-134">String</span></span>|<span data-ttu-id="6195a-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6195a-135">Key of the entity.</span></span> <span data-ttu-id="6195a-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6195a-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6195a-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6195a-137">lastModifiedDateTime</span></span>|<span data-ttu-id="6195a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6195a-138">DateTimeOffset</span></span>|<span data-ttu-id="6195a-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="6195a-139">DateTime the object was last modified.</span></span> <span data-ttu-id="6195a-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6195a-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6195a-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6195a-141">roleScopeTagIds</span></span>|<span data-ttu-id="6195a-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6195a-142">String collection</span></span>|<span data-ttu-id="6195a-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="6195a-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6195a-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6195a-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6195a-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6195a-145">supportsScopeTags</span></span>|<span data-ttu-id="6195a-146">Boolean.</span><span class="sxs-lookup"><span data-stu-id="6195a-146">Boolean</span></span>|<span data-ttu-id="6195a-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="6195a-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6195a-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="6195a-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6195a-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="6195a-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6195a-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6195a-150">This property is read-only.</span></span> <span data-ttu-id="6195a-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6195a-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6195a-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6195a-152">createdDateTime</span></span>|<span data-ttu-id="6195a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6195a-153">DateTimeOffset</span></span>|<span data-ttu-id="6195a-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="6195a-154">DateTime the object was created.</span></span> <span data-ttu-id="6195a-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6195a-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6195a-156">описание</span><span class="sxs-lookup"><span data-stu-id="6195a-156">description</span></span>|<span data-ttu-id="6195a-157">Строка</span><span class="sxs-lookup"><span data-stu-id="6195a-157">String</span></span>|<span data-ttu-id="6195a-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6195a-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6195a-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6195a-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6195a-160">displayName</span><span class="sxs-lookup"><span data-stu-id="6195a-160">displayName</span></span>|<span data-ttu-id="6195a-161">Строка</span><span class="sxs-lookup"><span data-stu-id="6195a-161">String</span></span>|<span data-ttu-id="6195a-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6195a-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6195a-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6195a-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6195a-164">version</span><span class="sxs-lookup"><span data-stu-id="6195a-164">version</span></span>|<span data-ttu-id="6195a-165">Int32</span><span class="sxs-lookup"><span data-stu-id="6195a-165">Int32</span></span>|<span data-ttu-id="6195a-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6195a-166">Version of the device configuration.</span></span> <span data-ttu-id="6195a-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6195a-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6195a-168">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="6195a-168">payloadFileName</span></span>|<span data-ttu-id="6195a-169">String</span><span class="sxs-lookup"><span data-stu-id="6195a-169">String</span></span>|<span data-ttu-id="6195a-170">Имя файла полезной нагрузки (\*.xml).</span><span class="sxs-lookup"><span data-stu-id="6195a-170">Payload file name (\*.xml).</span></span>|
|<span data-ttu-id="6195a-171">Имя_профиля</span><span class="sxs-lookup"><span data-stu-id="6195a-171">profileName</span></span>|<span data-ttu-id="6195a-172">String.</span><span class="sxs-lookup"><span data-stu-id="6195a-172">String</span></span>|<span data-ttu-id="6195a-173">Имя профиля, отображаемое в пользовательском Интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="6195a-173">Profile name displayed in the UI.</span></span>|
|<span data-ttu-id="6195a-174">payload</span><span class="sxs-lookup"><span data-stu-id="6195a-174">payload</span></span>|<span data-ttu-id="6195a-175">Binary</span><span class="sxs-lookup"><span data-stu-id="6195a-175">Binary</span></span>|<span data-ttu-id="6195a-176">Полезные данные</span><span class="sxs-lookup"><span data-stu-id="6195a-176">Payload.</span></span> <span data-ttu-id="6195a-177">(UTF8 закодированный массив байтов).</span><span class="sxs-lookup"><span data-stu-id="6195a-177">(UTF8 encoded byte array).</span></span> <span data-ttu-id="6195a-178">Это XML-файл, сохраненный на устройство, используемое для подключения к конечной точке Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="6195a-178">This is the XML file saved on the device you used to connect to the Wi-Fi endpoint.</span></span>|



## <a name="response"></a><span data-ttu-id="6195a-179">Ответ</span><span class="sxs-lookup"><span data-stu-id="6195a-179">Response</span></span>
<span data-ttu-id="6195a-180">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6195a-180">If successful, this method returns a `201 Created` response code and a [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6195a-181">Пример</span><span class="sxs-lookup"><span data-stu-id="6195a-181">Example</span></span>
### <a name="request"></a><span data-ttu-id="6195a-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="6195a-182">Request</span></span>
<span data-ttu-id="6195a-183">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6195a-183">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 445

{
  "@odata.type": "#microsoft.graph.windows81WifiImportConfiguration",
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

### <a name="response"></a><span data-ttu-id="6195a-184">Ответ</span><span class="sxs-lookup"><span data-stu-id="6195a-184">Response</span></span>
<span data-ttu-id="6195a-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="6195a-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





