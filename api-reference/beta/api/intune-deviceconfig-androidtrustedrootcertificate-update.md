---
title: Обновление androidTrustedRootCertificate
description: Обновление свойства объекта androidTrustedRootCertificate.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a38b8b0172f5b1c38e114f32364f78b5d8347392
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842107"
---
# <a name="update-androidtrustedrootcertificate"></a><span data-ttu-id="1cd67-103">Обновление androidTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="1cd67-103">Update androidTrustedRootCertificate</span></span>

> <span data-ttu-id="1cd67-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1cd67-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1cd67-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1cd67-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1cd67-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1cd67-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1cd67-107">Обновление свойства объекта [androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="1cd67-107">Update the properties of a [androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1cd67-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1cd67-108">Prerequisites</span></span>
<span data-ttu-id="1cd67-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1cd67-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1cd67-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1cd67-111">Permission type</span></span>|<span data-ttu-id="1cd67-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1cd67-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1cd67-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1cd67-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1cd67-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1cd67-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1cd67-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1cd67-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1cd67-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1cd67-116">Not supported.</span></span>|
|<span data-ttu-id="1cd67-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1cd67-117">Application</span></span>|<span data-ttu-id="1cd67-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1cd67-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1cd67-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1cd67-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidCertificateProfileBase/rootCertificate
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidEnterpriseWiFiConfiguration/rootCertificateForServerValidation
```

## <a name="request-headers"></a><span data-ttu-id="1cd67-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1cd67-120">Request headers</span></span>
|<span data-ttu-id="1cd67-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1cd67-121">Header</span></span>|<span data-ttu-id="1cd67-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1cd67-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1cd67-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1cd67-123">Authorization</span></span>|<span data-ttu-id="1cd67-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="1cd67-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1cd67-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1cd67-125">Accept</span></span>|<span data-ttu-id="1cd67-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1cd67-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1cd67-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1cd67-127">Request body</span></span>
<span data-ttu-id="1cd67-128">В тексте запроса укажите представление JSON для объекта [androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="1cd67-128">In the request body, supply a JSON representation for the [androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md) object.</span></span>

<span data-ttu-id="1cd67-129">В следующей таблице показаны свойства, которые необходимы для создания [androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="1cd67-129">The following table shows the properties that are required when you create the [androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md).</span></span>

|<span data-ttu-id="1cd67-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1cd67-130">Property</span></span>|<span data-ttu-id="1cd67-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1cd67-131">Type</span></span>|<span data-ttu-id="1cd67-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1cd67-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1cd67-133">id</span><span class="sxs-lookup"><span data-stu-id="1cd67-133">id</span></span>|<span data-ttu-id="1cd67-134">Строка</span><span class="sxs-lookup"><span data-stu-id="1cd67-134">String</span></span>|<span data-ttu-id="1cd67-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1cd67-135">Key of the entity.</span></span> <span data-ttu-id="1cd67-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1cd67-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1cd67-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1cd67-137">lastModifiedDateTime</span></span>|<span data-ttu-id="1cd67-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1cd67-138">DateTimeOffset</span></span>|<span data-ttu-id="1cd67-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="1cd67-139">DateTime the object was last modified.</span></span> <span data-ttu-id="1cd67-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1cd67-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1cd67-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1cd67-141">roleScopeTagIds</span></span>|<span data-ttu-id="1cd67-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1cd67-142">String collection</span></span>|<span data-ttu-id="1cd67-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="1cd67-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1cd67-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1cd67-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1cd67-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1cd67-145">supportsScopeTags</span></span>|<span data-ttu-id="1cd67-146">Логический</span><span class="sxs-lookup"><span data-stu-id="1cd67-146">Boolean</span></span>|<span data-ttu-id="1cd67-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="1cd67-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1cd67-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="1cd67-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1cd67-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="1cd67-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1cd67-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1cd67-150">This property is read-only.</span></span> <span data-ttu-id="1cd67-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1cd67-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1cd67-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1cd67-152">createdDateTime</span></span>|<span data-ttu-id="1cd67-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1cd67-153">DateTimeOffset</span></span>|<span data-ttu-id="1cd67-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="1cd67-154">DateTime the object was created.</span></span> <span data-ttu-id="1cd67-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1cd67-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1cd67-156">описание</span><span class="sxs-lookup"><span data-stu-id="1cd67-156">description</span></span>|<span data-ttu-id="1cd67-157">Строка</span><span class="sxs-lookup"><span data-stu-id="1cd67-157">String</span></span>|<span data-ttu-id="1cd67-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1cd67-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1cd67-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1cd67-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1cd67-160">displayName</span><span class="sxs-lookup"><span data-stu-id="1cd67-160">displayName</span></span>|<span data-ttu-id="1cd67-161">Строка</span><span class="sxs-lookup"><span data-stu-id="1cd67-161">String</span></span>|<span data-ttu-id="1cd67-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1cd67-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1cd67-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1cd67-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1cd67-164">version</span><span class="sxs-lookup"><span data-stu-id="1cd67-164">version</span></span>|<span data-ttu-id="1cd67-165">Int32</span><span class="sxs-lookup"><span data-stu-id="1cd67-165">Int32</span></span>|<span data-ttu-id="1cd67-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1cd67-166">Version of the device configuration.</span></span> <span data-ttu-id="1cd67-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1cd67-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1cd67-168">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="1cd67-168">trustedRootCertificate</span></span>|<span data-ttu-id="1cd67-169">Binary</span><span class="sxs-lookup"><span data-stu-id="1cd67-169">Binary</span></span>|<span data-ttu-id="1cd67-170">Доверенный корневой сертификат</span><span class="sxs-lookup"><span data-stu-id="1cd67-170">Trusted Root Certificate</span></span>|
|<span data-ttu-id="1cd67-171">certFileName</span><span class="sxs-lookup"><span data-stu-id="1cd67-171">certFileName</span></span>|<span data-ttu-id="1cd67-172">Строка</span><span class="sxs-lookup"><span data-stu-id="1cd67-172">String</span></span>|<span data-ttu-id="1cd67-173">Имя файла для отображения в пользовательском Интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="1cd67-173">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="1cd67-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="1cd67-174">Response</span></span>
<span data-ttu-id="1cd67-175">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1cd67-175">If successful, this method returns a `200 OK` response code and an updated [androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1cd67-176">Пример</span><span class="sxs-lookup"><span data-stu-id="1cd67-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="1cd67-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="1cd67-177">Request</span></span>
<span data-ttu-id="1cd67-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1cd67-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate
Content-type: application/json
Content-length: 363

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
  "certFileName": "Cert File Name value"
}
```

### <a name="response"></a><span data-ttu-id="1cd67-179">Ответ</span><span class="sxs-lookup"><span data-stu-id="1cd67-179">Response</span></span>
<span data-ttu-id="1cd67-p111">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1cd67-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 539

{
  "@odata.type": "#microsoft.graph.androidTrustedRootCertificate",
  "id": "7f8d751e-751e-7f8d-1e75-8d7f1e758d7f",
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
  "certFileName": "Cert File Name value"
}
```





