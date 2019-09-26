---
title: Обновление Девицеманажементдериведкредентиалсеттингс
description: Обновление свойств объекта Девицеманажементдериведкредентиалсеттингс.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e077181184d0309339288e775884291aeb48a28c
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37194504"
---
# <a name="update-devicemanagementderivedcredentialsettings"></a><span data-ttu-id="e719f-103">Обновление Девицеманажементдериведкредентиалсеттингс</span><span class="sxs-lookup"><span data-stu-id="e719f-103">Update deviceManagementDerivedCredentialSettings</span></span>

> <span data-ttu-id="e719f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e719f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e719f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e719f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e719f-106">Обновление свойств объекта [девицеманажементдериведкредентиалсеттингс](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="e719f-106">Update the properties of a [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e719f-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e719f-107">Prerequisites</span></span>
<span data-ttu-id="e719f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e719f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e719f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e719f-110">Permission type</span></span>|<span data-ttu-id="e719f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e719f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e719f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e719f-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="e719f-113">&nbsp; &nbsp; **Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="e719f-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="e719f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e719f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="e719f-115">&nbsp;&nbsp; **Политика доступа к ресурсам**</span><span class="sxs-lookup"><span data-stu-id="e719f-115">&nbsp; &nbsp; **Resource Access Policy**</span></span> | <span data-ttu-id="e719f-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e719f-116">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e719f-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e719f-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e719f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e719f-118">Not supported.</span></span>|
|<span data-ttu-id="e719f-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e719f-119">Application</span></span>||
| <span data-ttu-id="e719f-120">&nbsp; &nbsp; **Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="e719f-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="e719f-121">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e719f-121">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="e719f-122">&nbsp;&nbsp; **Политика доступа к ресурсам**</span><span class="sxs-lookup"><span data-stu-id="e719f-122">&nbsp; &nbsp; **Resource Access Policy**</span></span> | <span data-ttu-id="e719f-123">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e719f-123">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e719f-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e719f-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/derivedCredentials/{deviceManagementDerivedCredentialSettingsId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/derivedCredentialSettings
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosVpnConfiguration/derivedCredentialSettings
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEnterpriseWiFiConfiguration/derivedCredentialSettings
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEasEmailProfileConfiguration/derivedCredentialSettings
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosDerivedCredentialAuthenticationConfiguration/derivedCredentialSettings
```

## <a name="request-headers"></a><span data-ttu-id="e719f-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e719f-125">Request headers</span></span>
|<span data-ttu-id="e719f-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e719f-126">Header</span></span>|<span data-ttu-id="e719f-127">Значение</span><span class="sxs-lookup"><span data-stu-id="e719f-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e719f-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e719f-128">Authorization</span></span>|<span data-ttu-id="e719f-129">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e719f-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e719f-130">Accept</span><span class="sxs-lookup"><span data-stu-id="e719f-130">Accept</span></span>|<span data-ttu-id="e719f-131">application/json</span><span class="sxs-lookup"><span data-stu-id="e719f-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e719f-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e719f-132">Request body</span></span>
<span data-ttu-id="e719f-133">В тексте запроса добавьте представление объекта [девицеманажементдериведкредентиалсеттингс](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e719f-133">In the request body, supply a JSON representation for the [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object.</span></span>

<span data-ttu-id="e719f-134">В следующей таблице приведены свойства, необходимые при создании [девицеманажементдериведкредентиалсеттингс](../resources/intune-shared-devicemanagementderivedcredentialsettings.md).</span><span class="sxs-lookup"><span data-stu-id="e719f-134">The following table shows the properties that are required when you create the [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md).</span></span>

|<span data-ttu-id="e719f-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="e719f-135">Property</span></span>|<span data-ttu-id="e719f-136">Тип</span><span class="sxs-lookup"><span data-stu-id="e719f-136">Type</span></span>|<span data-ttu-id="e719f-137">Описание</span><span class="sxs-lookup"><span data-stu-id="e719f-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e719f-138">id</span><span class="sxs-lookup"><span data-stu-id="e719f-138">id</span></span>|<span data-ttu-id="e719f-139">String</span><span class="sxs-lookup"><span data-stu-id="e719f-139">String</span></span>|<span data-ttu-id="e719f-140">Уникальный идентификатор для производных учетных данных</span><span class="sxs-lookup"><span data-stu-id="e719f-140">Unique identifier for the Derived Credential</span></span>|
|<span data-ttu-id="e719f-141">**Политика RA**</span><span class="sxs-lookup"><span data-stu-id="e719f-141">**RA Policy**</span></span>|
|<span data-ttu-id="e719f-142">helpUrl</span><span class="sxs-lookup"><span data-stu-id="e719f-142">helpUrl</span></span>|<span data-ttu-id="e719f-143">String.</span><span class="sxs-lookup"><span data-stu-id="e719f-143">String</span></span>|<span data-ttu-id="e719f-144">URL-адрес, который будет доступен конечным пользователям для получения производных учетных данных с помощью корпоративного портала.</span><span class="sxs-lookup"><span data-stu-id="e719f-144">The URL that will be accessible to end users as they retrieve a derived credential using the Company Portal.</span></span>|
|<span data-ttu-id="e719f-145">displayName</span><span class="sxs-lookup"><span data-stu-id="e719f-145">displayName</span></span>|<span data-ttu-id="e719f-146">Строка</span><span class="sxs-lookup"><span data-stu-id="e719f-146">String</span></span>|<span data-ttu-id="e719f-147">Отображаемое имя профиля.</span><span class="sxs-lookup"><span data-stu-id="e719f-147">The display name for the profile.</span></span>|
|<span data-ttu-id="e719f-148">имени</span><span class="sxs-lookup"><span data-stu-id="e719f-148">issuer</span></span>|[<span data-ttu-id="e719f-149">deviceManagementDerivedCredentialIssuer</span><span class="sxs-lookup"><span data-stu-id="e719f-149">deviceManagementDerivedCredentialIssuer</span></span>](../resources/intune-shared-devicemanagementderivedcredentialissuer.md)|<span data-ttu-id="e719f-150">Производный поставщик учетных данных, который будет использоваться.</span><span class="sxs-lookup"><span data-stu-id="e719f-150">The derived credential provider to use.</span></span> <span data-ttu-id="e719f-151">Возможные значения: `intercede`, `entrustDatacard`, `purebred`.</span><span class="sxs-lookup"><span data-stu-id="e719f-151">Possible values are: `intercede`, `entrustDatacard`, `purebred`.</span></span>|
|<span data-ttu-id="e719f-152">notificationType</span><span class="sxs-lookup"><span data-stu-id="e719f-152">notificationType</span></span>|[<span data-ttu-id="e719f-153">deviceManagementDerivedCredentialNotificationType</span><span class="sxs-lookup"><span data-stu-id="e719f-153">deviceManagementDerivedCredentialNotificationType</span></span>](../resources/intune-shared-devicemanagementderivedcredentialnotificationtype.md)|<span data-ttu-id="e719f-154">Методы, используемые для информирования конечного пользователя об открытии корпоративного портала для доставки в сеть Wi-Fi, VPN или профилей электронной почты, использующих сертификаты для устройства.</span><span class="sxs-lookup"><span data-stu-id="e719f-154">The methods used to inform the end user to open Company Portal to deliver Wi-Fi, VPN, or email profiles that use certificates to the device.</span></span> <span data-ttu-id="e719f-155">Возможные значения: `none`, `companyPortal`, `email`.</span><span class="sxs-lookup"><span data-stu-id="e719f-155">Possible values are: `none`, `companyPortal`, `email`.</span></span>|


## <a name="response"></a><span data-ttu-id="e719f-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="e719f-156">Response</span></span>
<span data-ttu-id="e719f-157">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементдериведкредентиалсеттингс](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e719f-157">If successful, this method returns a `200 OK` response code and an updated [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e719f-158">Пример</span><span class="sxs-lookup"><span data-stu-id="e719f-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="e719f-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="e719f-159">Request</span></span>
<span data-ttu-id="e719f-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e719f-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/derivedCredentialSettings
Content-type: application/json
Content-length: 83

{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings"
}
```

### <a name="response"></a><span data-ttu-id="e719f-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="e719f-161">Response</span></span>
<span data-ttu-id="e719f-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e719f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 132

{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings",
  "id": "bc650741-0741-bc65-4107-65bc410765bc"
}
```





