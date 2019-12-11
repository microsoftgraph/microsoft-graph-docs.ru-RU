---
title: Создание Манажедаллдевицецертификатестате
description: Создание нового объекта Манажедаллдевицецертификатестате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a8ad91d9e7d6a5e02d25e72528c62e71a145c37f
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39947997"
---
# <a name="create-managedalldevicecertificatestate"></a><span data-ttu-id="eedff-103">Создание Манажедаллдевицецертификатестате</span><span class="sxs-lookup"><span data-stu-id="eedff-103">Create managedAllDeviceCertificateState</span></span>

> <span data-ttu-id="eedff-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eedff-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eedff-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eedff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eedff-106">Создание нового объекта [манажедаллдевицецертификатестате](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="eedff-106">Create a new [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eedff-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="eedff-107">Prerequisites</span></span>
<span data-ttu-id="eedff-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eedff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eedff-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eedff-110">Permission type</span></span>|<span data-ttu-id="eedff-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="eedff-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eedff-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eedff-112">Delegated (work or school account)</span></span>|<span data-ttu-id="eedff-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eedff-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="eedff-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eedff-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eedff-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eedff-115">Not supported.</span></span>|
|<span data-ttu-id="eedff-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eedff-116">Application</span></span>|<span data-ttu-id="eedff-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eedff-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eedff-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eedff-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates
```

## <a name="request-headers"></a><span data-ttu-id="eedff-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="eedff-119">Request headers</span></span>
|<span data-ttu-id="eedff-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="eedff-120">Header</span></span>|<span data-ttu-id="eedff-121">Значение</span><span class="sxs-lookup"><span data-stu-id="eedff-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eedff-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eedff-122">Authorization</span></span>|<span data-ttu-id="eedff-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eedff-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eedff-124">Accept</span><span class="sxs-lookup"><span data-stu-id="eedff-124">Accept</span></span>|<span data-ttu-id="eedff-125">application/json</span><span class="sxs-lookup"><span data-stu-id="eedff-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eedff-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="eedff-126">Request body</span></span>
<span data-ttu-id="eedff-127">В тексте запроса добавьте представление объекта Манажедаллдевицецертификатестате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eedff-127">In the request body, supply a JSON representation for the managedAllDeviceCertificateState object.</span></span>

<span data-ttu-id="eedff-128">В следующей таблице приведены свойства, необходимые при создании Манажедаллдевицецертификатестате.</span><span class="sxs-lookup"><span data-stu-id="eedff-128">The following table shows the properties that are required when you create the managedAllDeviceCertificateState.</span></span>

|<span data-ttu-id="eedff-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="eedff-129">Property</span></span>|<span data-ttu-id="eedff-130">Тип</span><span class="sxs-lookup"><span data-stu-id="eedff-130">Type</span></span>|<span data-ttu-id="eedff-131">Описание</span><span class="sxs-lookup"><span data-stu-id="eedff-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eedff-132">id</span><span class="sxs-lookup"><span data-stu-id="eedff-132">id</span></span>|<span data-ttu-id="eedff-133">Строка</span><span class="sxs-lookup"><span data-stu-id="eedff-133">String</span></span>|<span data-ttu-id="eedff-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="eedff-134">Key of the entity.</span></span>|
|<span data-ttu-id="eedff-135">цертификатеревокестатус</span><span class="sxs-lookup"><span data-stu-id="eedff-135">certificateRevokeStatus</span></span>|[<span data-ttu-id="eedff-136">цертификатеревокатионстатус</span><span class="sxs-lookup"><span data-stu-id="eedff-136">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="eedff-137">Отзыв состояния.</span><span class="sxs-lookup"><span data-stu-id="eedff-137">Revoke status.</span></span> <span data-ttu-id="eedff-138">Возможные значения: `none`, `pending`, `issued`, `failed`, `revoked`.</span><span class="sxs-lookup"><span data-stu-id="eedff-138">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="eedff-139">манажеддевицедисплайнаме</span><span class="sxs-lookup"><span data-stu-id="eedff-139">managedDeviceDisplayName</span></span>|<span data-ttu-id="eedff-140">Строка</span><span class="sxs-lookup"><span data-stu-id="eedff-140">String</span></span>|<span data-ttu-id="eedff-141">Отображаемое имя устройства</span><span class="sxs-lookup"><span data-stu-id="eedff-141">Device display name</span></span>|
|<span data-ttu-id="eedff-142">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="eedff-142">userPrincipalName</span></span>|<span data-ttu-id="eedff-143">String</span><span class="sxs-lookup"><span data-stu-id="eedff-143">String</span></span>|<span data-ttu-id="eedff-144">Имя субъекта-пользователя</span><span class="sxs-lookup"><span data-stu-id="eedff-144">User principal name</span></span>|
|<span data-ttu-id="eedff-145">цертификатикспиратиондатетиме</span><span class="sxs-lookup"><span data-stu-id="eedff-145">certificateExpirationDateTime</span></span>|<span data-ttu-id="eedff-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eedff-146">DateTimeOffset</span></span>|<span data-ttu-id="eedff-147">Дата окончания срока действия сертификата</span><span class="sxs-lookup"><span data-stu-id="eedff-147">Certificate expiry date</span></span>|
|<span data-ttu-id="eedff-148">цертификатеиссуернаме</span><span class="sxs-lookup"><span data-stu-id="eedff-148">certificateIssuerName</span></span>|<span data-ttu-id="eedff-149">Строка</span><span class="sxs-lookup"><span data-stu-id="eedff-149">String</span></span>|<span data-ttu-id="eedff-150">Издатель</span><span class="sxs-lookup"><span data-stu-id="eedff-150">Issuer</span></span>|
|<span data-ttu-id="eedff-151">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="eedff-151">certificateThumbprint</span></span>|<span data-ttu-id="eedff-152">Строка</span><span class="sxs-lookup"><span data-stu-id="eedff-152">String</span></span>|<span data-ttu-id="eedff-153">Отпечаток</span><span class="sxs-lookup"><span data-stu-id="eedff-153">Thumbprint</span></span>|
|<span data-ttu-id="eedff-154">цертификатесериалнумбер</span><span class="sxs-lookup"><span data-stu-id="eedff-154">certificateSerialNumber</span></span>|<span data-ttu-id="eedff-155">Строка</span><span class="sxs-lookup"><span data-stu-id="eedff-155">String</span></span>|<span data-ttu-id="eedff-156">Серийный номер</span><span class="sxs-lookup"><span data-stu-id="eedff-156">Serial number</span></span>|
|<span data-ttu-id="eedff-157">цертификатесубжектнаме</span><span class="sxs-lookup"><span data-stu-id="eedff-157">certificateSubjectName</span></span>|<span data-ttu-id="eedff-158">Строка</span><span class="sxs-lookup"><span data-stu-id="eedff-158">String</span></span>|<span data-ttu-id="eedff-159">Имя субъекта сертификата</span><span class="sxs-lookup"><span data-stu-id="eedff-159">Certificate subject name</span></span>|
|<span data-ttu-id="eedff-160">цертификатекэйусажес</span><span class="sxs-lookup"><span data-stu-id="eedff-160">certificateKeyUsages</span></span>|<span data-ttu-id="eedff-161">Int32</span><span class="sxs-lookup"><span data-stu-id="eedff-161">Int32</span></span>|<span data-ttu-id="eedff-162">Использование ключа</span><span class="sxs-lookup"><span data-stu-id="eedff-162">Key Usage</span></span>|
|<span data-ttu-id="eedff-163">цертификатикстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="eedff-163">certificateExtendedKeyUsages</span></span>|<span data-ttu-id="eedff-164">Строка</span><span class="sxs-lookup"><span data-stu-id="eedff-164">String</span></span>|<span data-ttu-id="eedff-165">Расширенное использование ключа</span><span class="sxs-lookup"><span data-stu-id="eedff-165">Enhanced Key Usage</span></span>|
|<span data-ttu-id="eedff-166">цертификатеиссуанцедатетиме</span><span class="sxs-lookup"><span data-stu-id="eedff-166">certificateIssuanceDateTime</span></span>|<span data-ttu-id="eedff-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eedff-167">DateTimeOffset</span></span>|<span data-ttu-id="eedff-168">Дата выпуска</span><span class="sxs-lookup"><span data-stu-id="eedff-168">Issuance date</span></span>|



## <a name="response"></a><span data-ttu-id="eedff-169">Ответ</span><span class="sxs-lookup"><span data-stu-id="eedff-169">Response</span></span>
<span data-ttu-id="eedff-170">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [манажедаллдевицецертификатестате](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="eedff-170">If successful, this method returns a `201 Created` response code and a [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eedff-171">Пример</span><span class="sxs-lookup"><span data-stu-id="eedff-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="eedff-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="eedff-172">Request</span></span>
<span data-ttu-id="eedff-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eedff-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates
Content-type: application/json
Content-length: 735

{
  "@odata.type": "#microsoft.graph.managedAllDeviceCertificateState",
  "certificateRevokeStatus": "pending",
  "managedDeviceDisplayName": "Managed Device Display Name value",
  "userPrincipalName": "User Principal Name value",
  "certificateExpirationDateTime": "2017-01-01T00:02:14.9489247-08:00",
  "certificateIssuerName": "Certificate Issuer Name value",
  "certificateThumbprint": "Certificate Thumbprint value",
  "certificateSerialNumber": "Certificate Serial Number value",
  "certificateSubjectName": "Certificate Subject Name value",
  "certificateKeyUsages": 4,
  "certificateExtendedKeyUsages": "Certificate Extended Key Usages value",
  "certificateIssuanceDateTime": "2016-12-31T23:59:41.5044473-08:00"
}
```

### <a name="response"></a><span data-ttu-id="eedff-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="eedff-174">Response</span></span>
<span data-ttu-id="eedff-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="eedff-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 784

{
  "@odata.type": "#microsoft.graph.managedAllDeviceCertificateState",
  "id": "987c6a17-6a17-987c-176a-7c98176a7c98",
  "certificateRevokeStatus": "pending",
  "managedDeviceDisplayName": "Managed Device Display Name value",
  "userPrincipalName": "User Principal Name value",
  "certificateExpirationDateTime": "2017-01-01T00:02:14.9489247-08:00",
  "certificateIssuerName": "Certificate Issuer Name value",
  "certificateThumbprint": "Certificate Thumbprint value",
  "certificateSerialNumber": "Certificate Serial Number value",
  "certificateSubjectName": "Certificate Subject Name value",
  "certificateKeyUsages": 4,
  "certificateExtendedKeyUsages": "Certificate Extended Key Usages value",
  "certificateIssuanceDateTime": "2016-12-31T23:59:41.5044473-08:00"
}
```





