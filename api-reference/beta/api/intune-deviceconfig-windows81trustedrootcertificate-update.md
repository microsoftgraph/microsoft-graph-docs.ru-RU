---
title: Обновление windows81TrustedRootCertificate
description: Обновление свойства объекта windows81TrustedRootCertificate.
author: tfitzmac
ms.openlocfilehash: ce95eda15d57a4e44b5c3c4756205638e2eb9cbb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307430"
---
# <a name="update-windows81trustedrootcertificate"></a><span data-ttu-id="ad19e-103">Обновление windows81TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="ad19e-103">Update windows81TrustedRootCertificate</span></span>

> <span data-ttu-id="ad19e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ad19e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ad19e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad19e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ad19e-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ad19e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ad19e-107">Обновление свойства объекта [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="ad19e-107">Update the properties of a [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ad19e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ad19e-108">Prerequisites</span></span>
<span data-ttu-id="ad19e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad19e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad19e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ad19e-111">Permission type</span></span>|<span data-ttu-id="ad19e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ad19e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad19e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ad19e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ad19e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad19e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ad19e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ad19e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad19e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad19e-116">Not supported.</span></span>|
|<span data-ttu-id="ad19e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ad19e-117">Application</span></span>|<span data-ttu-id="ad19e-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad19e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad19e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ad19e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/rootCertificate
```

## <a name="request-headers"></a><span data-ttu-id="ad19e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ad19e-120">Request headers</span></span>
|<span data-ttu-id="ad19e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ad19e-121">Header</span></span>|<span data-ttu-id="ad19e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ad19e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad19e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ad19e-123">Authorization</span></span>|<span data-ttu-id="ad19e-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ad19e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ad19e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ad19e-125">Accept</span></span>|<span data-ttu-id="ad19e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ad19e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad19e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ad19e-127">Request body</span></span>
<span data-ttu-id="ad19e-128">В тексте запроса укажите представление JSON для объекта [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="ad19e-128">In the request body, supply a JSON representation for the [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object.</span></span>

<span data-ttu-id="ad19e-129">В следующей таблице показаны свойства, которые необходимы для создания [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="ad19e-129">The following table shows the properties that are required when you create the [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md).</span></span>

|<span data-ttu-id="ad19e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ad19e-130">Property</span></span>|<span data-ttu-id="ad19e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ad19e-131">Type</span></span>|<span data-ttu-id="ad19e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ad19e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad19e-133">id</span><span class="sxs-lookup"><span data-stu-id="ad19e-133">id</span></span>|<span data-ttu-id="ad19e-134">Строка</span><span class="sxs-lookup"><span data-stu-id="ad19e-134">String</span></span>|<span data-ttu-id="ad19e-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ad19e-135">Key of the entity.</span></span> <span data-ttu-id="ad19e-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ad19e-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad19e-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ad19e-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ad19e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad19e-138">DateTimeOffset</span></span>|<span data-ttu-id="ad19e-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ad19e-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ad19e-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ad19e-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad19e-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ad19e-141">roleScopeTagIds</span></span>|<span data-ttu-id="ad19e-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ad19e-142">String collection</span></span>|<span data-ttu-id="ad19e-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="ad19e-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ad19e-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ad19e-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad19e-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ad19e-145">supportsScopeTags</span></span>|<span data-ttu-id="ad19e-146">Boolean.</span><span class="sxs-lookup"><span data-stu-id="ad19e-146">Boolean</span></span>|<span data-ttu-id="ad19e-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="ad19e-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ad19e-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="ad19e-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ad19e-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="ad19e-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ad19e-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ad19e-150">This property is read-only.</span></span> <span data-ttu-id="ad19e-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ad19e-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad19e-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ad19e-152">createdDateTime</span></span>|<span data-ttu-id="ad19e-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad19e-153">DateTimeOffset</span></span>|<span data-ttu-id="ad19e-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ad19e-154">DateTime the object was created.</span></span> <span data-ttu-id="ad19e-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ad19e-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad19e-156">описание</span><span class="sxs-lookup"><span data-stu-id="ad19e-156">description</span></span>|<span data-ttu-id="ad19e-157">Строка</span><span class="sxs-lookup"><span data-stu-id="ad19e-157">String</span></span>|<span data-ttu-id="ad19e-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ad19e-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ad19e-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ad19e-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad19e-160">displayName</span><span class="sxs-lookup"><span data-stu-id="ad19e-160">displayName</span></span>|<span data-ttu-id="ad19e-161">Строка</span><span class="sxs-lookup"><span data-stu-id="ad19e-161">String</span></span>|<span data-ttu-id="ad19e-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ad19e-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ad19e-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ad19e-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad19e-164">version</span><span class="sxs-lookup"><span data-stu-id="ad19e-164">version</span></span>|<span data-ttu-id="ad19e-165">Int32</span><span class="sxs-lookup"><span data-stu-id="ad19e-165">Int32</span></span>|<span data-ttu-id="ad19e-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ad19e-166">Version of the device configuration.</span></span> <span data-ttu-id="ad19e-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ad19e-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad19e-168">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="ad19e-168">trustedRootCertificate</span></span>|<span data-ttu-id="ad19e-169">Binary</span><span class="sxs-lookup"><span data-stu-id="ad19e-169">Binary</span></span>|<span data-ttu-id="ad19e-170">Доверенный корневой сертификат</span><span class="sxs-lookup"><span data-stu-id="ad19e-170">Trusted Root Certificate</span></span>|
|<span data-ttu-id="ad19e-171">certFileName</span><span class="sxs-lookup"><span data-stu-id="ad19e-171">certFileName</span></span>|<span data-ttu-id="ad19e-172">String.</span><span class="sxs-lookup"><span data-stu-id="ad19e-172">String</span></span>|<span data-ttu-id="ad19e-173">Имя файла для отображения в пользовательском Интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="ad19e-173">File name to display in UI.</span></span>|
|<span data-ttu-id="ad19e-174">destinationStore</span><span class="sxs-lookup"><span data-stu-id="ad19e-174">destinationStore</span></span>|[<span data-ttu-id="ad19e-175">certificateDestinationStore</span><span class="sxs-lookup"><span data-stu-id="ad19e-175">certificateDestinationStore</span></span>](../resources/intune-deviceconfig-certificatedestinationstore.md)|<span data-ttu-id="ad19e-176">Место размещения хранилища доверенного корневого сертификата.</span><span class="sxs-lookup"><span data-stu-id="ad19e-176">Destination store location for the Trusted Root Certificate.</span></span> <span data-ttu-id="ad19e-177">Возможные значения: `computerCertStoreRoot`, `computerCertStoreIntermediate`, `userCertStoreIntermediate`.</span><span class="sxs-lookup"><span data-stu-id="ad19e-177">Possible values are: `computerCertStoreRoot`, `computerCertStoreIntermediate`, `userCertStoreIntermediate`.</span></span>|



## <a name="response"></a><span data-ttu-id="ad19e-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad19e-178">Response</span></span>
<span data-ttu-id="ad19e-179">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ad19e-179">If successful, this method returns a `200 OK` response code and an updated [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad19e-180">Пример</span><span class="sxs-lookup"><span data-stu-id="ad19e-180">Example</span></span>
### <a name="request"></a><span data-ttu-id="ad19e-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad19e-181">Request</span></span>
<span data-ttu-id="ad19e-182">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ad19e-182">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}
Content-type: application/json
Content-length: 419

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value",
  "destinationStore": "computerCertStoreIntermediate"
}
```

### <a name="response"></a><span data-ttu-id="ad19e-183">Ответ</span><span class="sxs-lookup"><span data-stu-id="ad19e-183">Response</span></span>
<span data-ttu-id="ad19e-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ad19e-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 597

{
  "@odata.type": "#microsoft.graph.windows81TrustedRootCertificate",
  "id": "3fb588f9-88f9-3fb5-f988-b53ff988b53f",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value",
  "destinationStore": "computerCertStoreIntermediate"
}
```





