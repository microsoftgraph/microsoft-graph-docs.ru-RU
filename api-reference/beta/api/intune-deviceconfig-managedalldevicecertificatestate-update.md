---
title: Обновление Манажедаллдевицецертификатестате
description: Обновление свойств объекта Манажедаллдевицецертификатестате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f3e86964684f0b1e913b74aaad7ab587aad65e70
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39947962"
---
# <a name="update-managedalldevicecertificatestate"></a><span data-ttu-id="225ff-103">Обновление Манажедаллдевицецертификатестате</span><span class="sxs-lookup"><span data-stu-id="225ff-103">Update managedAllDeviceCertificateState</span></span>

> <span data-ttu-id="225ff-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="225ff-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="225ff-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="225ff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="225ff-106">Обновление свойств объекта [манажедаллдевицецертификатестате](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="225ff-106">Update the properties of a [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="225ff-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="225ff-107">Prerequisites</span></span>
<span data-ttu-id="225ff-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="225ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="225ff-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="225ff-110">Permission type</span></span>|<span data-ttu-id="225ff-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="225ff-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="225ff-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="225ff-112">Delegated (work or school account)</span></span>|<span data-ttu-id="225ff-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="225ff-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="225ff-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="225ff-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="225ff-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="225ff-115">Not supported.</span></span>|
|<span data-ttu-id="225ff-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="225ff-116">Application</span></span>|<span data-ttu-id="225ff-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="225ff-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="225ff-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="225ff-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates/{managedAllDeviceCertificateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="225ff-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="225ff-119">Request headers</span></span>
|<span data-ttu-id="225ff-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="225ff-120">Header</span></span>|<span data-ttu-id="225ff-121">Значение</span><span class="sxs-lookup"><span data-stu-id="225ff-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="225ff-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="225ff-122">Authorization</span></span>|<span data-ttu-id="225ff-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="225ff-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="225ff-124">Accept</span><span class="sxs-lookup"><span data-stu-id="225ff-124">Accept</span></span>|<span data-ttu-id="225ff-125">application/json</span><span class="sxs-lookup"><span data-stu-id="225ff-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="225ff-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="225ff-126">Request body</span></span>
<span data-ttu-id="225ff-127">В тексте запроса добавьте представление объекта [манажедаллдевицецертификатестате](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="225ff-127">In the request body, supply a JSON representation for the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

<span data-ttu-id="225ff-128">В следующей таблице приведены свойства, необходимые при создании [манажедаллдевицецертификатестате](../resources/intune-deviceconfig-managedalldevicecertificatestate.md).</span><span class="sxs-lookup"><span data-stu-id="225ff-128">The following table shows the properties that are required when you create the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md).</span></span>

|<span data-ttu-id="225ff-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="225ff-129">Property</span></span>|<span data-ttu-id="225ff-130">Тип</span><span class="sxs-lookup"><span data-stu-id="225ff-130">Type</span></span>|<span data-ttu-id="225ff-131">Описание</span><span class="sxs-lookup"><span data-stu-id="225ff-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="225ff-132">id</span><span class="sxs-lookup"><span data-stu-id="225ff-132">id</span></span>|<span data-ttu-id="225ff-133">Строка</span><span class="sxs-lookup"><span data-stu-id="225ff-133">String</span></span>|<span data-ttu-id="225ff-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="225ff-134">Key of the entity.</span></span>|
|<span data-ttu-id="225ff-135">цертификатеревокестатус</span><span class="sxs-lookup"><span data-stu-id="225ff-135">certificateRevokeStatus</span></span>|[<span data-ttu-id="225ff-136">цертификатеревокатионстатус</span><span class="sxs-lookup"><span data-stu-id="225ff-136">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="225ff-137">Отзыв состояния.</span><span class="sxs-lookup"><span data-stu-id="225ff-137">Revoke status.</span></span> <span data-ttu-id="225ff-138">Возможные значения: `none`, `pending`, `issued`, `failed`, `revoked`.</span><span class="sxs-lookup"><span data-stu-id="225ff-138">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="225ff-139">манажеддевицедисплайнаме</span><span class="sxs-lookup"><span data-stu-id="225ff-139">managedDeviceDisplayName</span></span>|<span data-ttu-id="225ff-140">Строка</span><span class="sxs-lookup"><span data-stu-id="225ff-140">String</span></span>|<span data-ttu-id="225ff-141">Отображаемое имя устройства</span><span class="sxs-lookup"><span data-stu-id="225ff-141">Device display name</span></span>|
|<span data-ttu-id="225ff-142">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="225ff-142">userPrincipalName</span></span>|<span data-ttu-id="225ff-143">String</span><span class="sxs-lookup"><span data-stu-id="225ff-143">String</span></span>|<span data-ttu-id="225ff-144">Имя субъекта-пользователя</span><span class="sxs-lookup"><span data-stu-id="225ff-144">User principal name</span></span>|
|<span data-ttu-id="225ff-145">цертификатикспиратиондатетиме</span><span class="sxs-lookup"><span data-stu-id="225ff-145">certificateExpirationDateTime</span></span>|<span data-ttu-id="225ff-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="225ff-146">DateTimeOffset</span></span>|<span data-ttu-id="225ff-147">Дата окончания срока действия сертификата</span><span class="sxs-lookup"><span data-stu-id="225ff-147">Certificate expiry date</span></span>|
|<span data-ttu-id="225ff-148">цертификатеиссуернаме</span><span class="sxs-lookup"><span data-stu-id="225ff-148">certificateIssuerName</span></span>|<span data-ttu-id="225ff-149">Строка</span><span class="sxs-lookup"><span data-stu-id="225ff-149">String</span></span>|<span data-ttu-id="225ff-150">Издатель</span><span class="sxs-lookup"><span data-stu-id="225ff-150">Issuer</span></span>|
|<span data-ttu-id="225ff-151">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="225ff-151">certificateThumbprint</span></span>|<span data-ttu-id="225ff-152">Строка</span><span class="sxs-lookup"><span data-stu-id="225ff-152">String</span></span>|<span data-ttu-id="225ff-153">Отпечаток</span><span class="sxs-lookup"><span data-stu-id="225ff-153">Thumbprint</span></span>|
|<span data-ttu-id="225ff-154">цертификатесериалнумбер</span><span class="sxs-lookup"><span data-stu-id="225ff-154">certificateSerialNumber</span></span>|<span data-ttu-id="225ff-155">Строка</span><span class="sxs-lookup"><span data-stu-id="225ff-155">String</span></span>|<span data-ttu-id="225ff-156">Серийный номер</span><span class="sxs-lookup"><span data-stu-id="225ff-156">Serial number</span></span>|
|<span data-ttu-id="225ff-157">цертификатесубжектнаме</span><span class="sxs-lookup"><span data-stu-id="225ff-157">certificateSubjectName</span></span>|<span data-ttu-id="225ff-158">Строка</span><span class="sxs-lookup"><span data-stu-id="225ff-158">String</span></span>|<span data-ttu-id="225ff-159">Имя субъекта сертификата</span><span class="sxs-lookup"><span data-stu-id="225ff-159">Certificate subject name</span></span>|
|<span data-ttu-id="225ff-160">цертификатекэйусажес</span><span class="sxs-lookup"><span data-stu-id="225ff-160">certificateKeyUsages</span></span>|<span data-ttu-id="225ff-161">Int32</span><span class="sxs-lookup"><span data-stu-id="225ff-161">Int32</span></span>|<span data-ttu-id="225ff-162">Использование ключа</span><span class="sxs-lookup"><span data-stu-id="225ff-162">Key Usage</span></span>|
|<span data-ttu-id="225ff-163">цертификатикстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="225ff-163">certificateExtendedKeyUsages</span></span>|<span data-ttu-id="225ff-164">Строка</span><span class="sxs-lookup"><span data-stu-id="225ff-164">String</span></span>|<span data-ttu-id="225ff-165">Расширенное использование ключа</span><span class="sxs-lookup"><span data-stu-id="225ff-165">Enhanced Key Usage</span></span>|
|<span data-ttu-id="225ff-166">цертификатеиссуанцедатетиме</span><span class="sxs-lookup"><span data-stu-id="225ff-166">certificateIssuanceDateTime</span></span>|<span data-ttu-id="225ff-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="225ff-167">DateTimeOffset</span></span>|<span data-ttu-id="225ff-168">Дата выпуска</span><span class="sxs-lookup"><span data-stu-id="225ff-168">Issuance date</span></span>|



## <a name="response"></a><span data-ttu-id="225ff-169">Ответ</span><span class="sxs-lookup"><span data-stu-id="225ff-169">Response</span></span>
<span data-ttu-id="225ff-170">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [манажедаллдевицецертификатестате](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="225ff-170">If successful, this method returns a `200 OK` response code and an updated [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="225ff-171">Пример</span><span class="sxs-lookup"><span data-stu-id="225ff-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="225ff-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="225ff-172">Request</span></span>
<span data-ttu-id="225ff-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="225ff-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates/{managedAllDeviceCertificateStateId}
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

### <a name="response"></a><span data-ttu-id="225ff-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="225ff-174">Response</span></span>
<span data-ttu-id="225ff-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="225ff-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





