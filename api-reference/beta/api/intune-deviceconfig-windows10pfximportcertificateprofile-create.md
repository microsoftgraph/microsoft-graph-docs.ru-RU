---
title: Создание windows10PFXImportCertificateProfile
description: Создание нового объекта windows10PFXImportCertificateProfile.
author: tfitzmac
ms.openlocfilehash: f98970b0159e98f101b99e6694fa552b57e203b9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27338306"
---
# <a name="create-windows10pfximportcertificateprofile"></a><span data-ttu-id="09e20-103">Создание windows10PFXImportCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="09e20-103">Create windows10PFXImportCertificateProfile</span></span>

> <span data-ttu-id="09e20-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="09e20-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="09e20-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09e20-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="09e20-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="09e20-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="09e20-107">Создание нового объекта [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="09e20-107">Create a new [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="09e20-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="09e20-108">Prerequisites</span></span>
<span data-ttu-id="09e20-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09e20-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09e20-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="09e20-111">Permission type</span></span>|<span data-ttu-id="09e20-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="09e20-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09e20-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="09e20-113">Delegated (work or school account)</span></span>|<span data-ttu-id="09e20-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09e20-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="09e20-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="09e20-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09e20-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09e20-116">Not supported.</span></span>|
|<span data-ttu-id="09e20-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="09e20-117">Application</span></span>|<span data-ttu-id="09e20-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09e20-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="09e20-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="09e20-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="09e20-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="09e20-120">Request headers</span></span>
|<span data-ttu-id="09e20-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="09e20-121">Header</span></span>|<span data-ttu-id="09e20-122">Значение</span><span class="sxs-lookup"><span data-stu-id="09e20-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="09e20-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="09e20-123">Authorization</span></span>|<span data-ttu-id="09e20-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="09e20-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="09e20-125">Accept</span><span class="sxs-lookup"><span data-stu-id="09e20-125">Accept</span></span>|<span data-ttu-id="09e20-126">application/json</span><span class="sxs-lookup"><span data-stu-id="09e20-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="09e20-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="09e20-127">Request body</span></span>
<span data-ttu-id="09e20-128">В тексте запроса укажите представление JSON для объекта windows10PFXImportCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="09e20-128">In the request body, supply a JSON representation for the windows10PFXImportCertificateProfile object.</span></span>

<span data-ttu-id="09e20-129">В следующей таблице показаны свойства, которые необходимы для создания windows10PFXImportCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="09e20-129">The following table shows the properties that are required when you create the windows10PFXImportCertificateProfile.</span></span>

|<span data-ttu-id="09e20-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="09e20-130">Property</span></span>|<span data-ttu-id="09e20-131">Тип</span><span class="sxs-lookup"><span data-stu-id="09e20-131">Type</span></span>|<span data-ttu-id="09e20-132">Описание</span><span class="sxs-lookup"><span data-stu-id="09e20-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09e20-133">id</span><span class="sxs-lookup"><span data-stu-id="09e20-133">id</span></span>|<span data-ttu-id="09e20-134">Строка</span><span class="sxs-lookup"><span data-stu-id="09e20-134">String</span></span>|<span data-ttu-id="09e20-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="09e20-135">Key of the entity.</span></span> <span data-ttu-id="09e20-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="09e20-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09e20-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="09e20-137">lastModifiedDateTime</span></span>|<span data-ttu-id="09e20-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09e20-138">DateTimeOffset</span></span>|<span data-ttu-id="09e20-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="09e20-139">DateTime the object was last modified.</span></span> <span data-ttu-id="09e20-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="09e20-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09e20-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="09e20-141">roleScopeTagIds</span></span>|<span data-ttu-id="09e20-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="09e20-142">String collection</span></span>|<span data-ttu-id="09e20-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="09e20-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="09e20-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="09e20-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09e20-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="09e20-145">supportsScopeTags</span></span>|<span data-ttu-id="09e20-146">Boolean.</span><span class="sxs-lookup"><span data-stu-id="09e20-146">Boolean</span></span>|<span data-ttu-id="09e20-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="09e20-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="09e20-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="09e20-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="09e20-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="09e20-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="09e20-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="09e20-150">This property is read-only.</span></span> <span data-ttu-id="09e20-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="09e20-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09e20-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="09e20-152">createdDateTime</span></span>|<span data-ttu-id="09e20-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09e20-153">DateTimeOffset</span></span>|<span data-ttu-id="09e20-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="09e20-154">DateTime the object was created.</span></span> <span data-ttu-id="09e20-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="09e20-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09e20-156">описание</span><span class="sxs-lookup"><span data-stu-id="09e20-156">description</span></span>|<span data-ttu-id="09e20-157">Строка</span><span class="sxs-lookup"><span data-stu-id="09e20-157">String</span></span>|<span data-ttu-id="09e20-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="09e20-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="09e20-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="09e20-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09e20-160">displayName</span><span class="sxs-lookup"><span data-stu-id="09e20-160">displayName</span></span>|<span data-ttu-id="09e20-161">Строка</span><span class="sxs-lookup"><span data-stu-id="09e20-161">String</span></span>|<span data-ttu-id="09e20-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="09e20-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="09e20-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="09e20-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09e20-164">version</span><span class="sxs-lookup"><span data-stu-id="09e20-164">version</span></span>|<span data-ttu-id="09e20-165">Int32</span><span class="sxs-lookup"><span data-stu-id="09e20-165">Int32</span></span>|<span data-ttu-id="09e20-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="09e20-166">Version of the device configuration.</span></span> <span data-ttu-id="09e20-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="09e20-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09e20-168">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="09e20-168">keyStorageProvider</span></span>|[<span data-ttu-id="09e20-169">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="09e20-169">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="09e20-170">Еще не документированы.</span><span class="sxs-lookup"><span data-stu-id="09e20-170">Not yet documented.</span></span> <span data-ttu-id="09e20-171">Возможные значения: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="09e20-171">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|



## <a name="response"></a><span data-ttu-id="09e20-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="09e20-172">Response</span></span>
<span data-ttu-id="09e20-173">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="09e20-173">If successful, this method returns a `201 Created` response code and a [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09e20-174">Пример</span><span class="sxs-lookup"><span data-stu-id="09e20-174">Example</span></span>
### <a name="request"></a><span data-ttu-id="09e20-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="09e20-175">Request</span></span>
<span data-ttu-id="09e20-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="09e20-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 381

{
  "@odata.type": "#microsoft.graph.windows10PFXImportCertificateProfile",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "keyStorageProvider": "useTpmKspOtherwiseFail"
}
```

### <a name="response"></a><span data-ttu-id="09e20-177">Ответ</span><span class="sxs-lookup"><span data-stu-id="09e20-177">Response</span></span>
<span data-ttu-id="09e20-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="09e20-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 489

{
  "@odata.type": "#microsoft.graph.windows10PFXImportCertificateProfile",
  "id": "4244277a-277a-4244-7a27-44427a274442",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "keyStorageProvider": "useTpmKspOtherwiseFail"
}
```





