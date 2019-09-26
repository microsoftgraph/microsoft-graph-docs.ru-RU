---
title: Обновление Манажедаллдевицецертификатестате
description: Обновление свойств объекта Манажедаллдевицецертификатестате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bc5b58cca354b3952a0b6b44baa7e863c0c8577d
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37183683"
---
# <a name="update-managedalldevicecertificatestate"></a><span data-ttu-id="c108d-103">Обновление Манажедаллдевицецертификатестате</span><span class="sxs-lookup"><span data-stu-id="c108d-103">Update managedAllDeviceCertificateState</span></span>

> <span data-ttu-id="c108d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c108d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c108d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c108d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c108d-106">Обновление свойств объекта [манажедаллдевицецертификатестате](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="c108d-106">Update the properties of a [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c108d-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c108d-107">Prerequisites</span></span>
<span data-ttu-id="c108d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c108d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c108d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c108d-110">Permission type</span></span>|<span data-ttu-id="c108d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c108d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c108d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c108d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c108d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c108d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c108d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c108d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c108d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c108d-115">Not supported.</span></span>|
|<span data-ttu-id="c108d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c108d-116">Application</span></span>|<span data-ttu-id="c108d-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c108d-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c108d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c108d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates/{managedAllDeviceCertificateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="c108d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c108d-119">Request headers</span></span>
|<span data-ttu-id="c108d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c108d-120">Header</span></span>|<span data-ttu-id="c108d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c108d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c108d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c108d-122">Authorization</span></span>|<span data-ttu-id="c108d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c108d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c108d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c108d-124">Accept</span></span>|<span data-ttu-id="c108d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c108d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c108d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c108d-126">Request body</span></span>
<span data-ttu-id="c108d-127">В тексте запроса добавьте представление объекта [манажедаллдевицецертификатестате](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c108d-127">In the request body, supply a JSON representation for the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

<span data-ttu-id="c108d-128">В следующей таблице приведены свойства, необходимые при создании [манажедаллдевицецертификатестате](../resources/intune-deviceconfig-managedalldevicecertificatestate.md).</span><span class="sxs-lookup"><span data-stu-id="c108d-128">The following table shows the properties that are required when you create the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md).</span></span>

|<span data-ttu-id="c108d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c108d-129">Property</span></span>|<span data-ttu-id="c108d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c108d-130">Type</span></span>|<span data-ttu-id="c108d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c108d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c108d-132">id</span><span class="sxs-lookup"><span data-stu-id="c108d-132">id</span></span>|<span data-ttu-id="c108d-133">Строка</span><span class="sxs-lookup"><span data-stu-id="c108d-133">String</span></span>|<span data-ttu-id="c108d-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c108d-134">Key of the entity.</span></span>|
|<span data-ttu-id="c108d-135">цертификатеревокестатус</span><span class="sxs-lookup"><span data-stu-id="c108d-135">certificateRevokeStatus</span></span>|[<span data-ttu-id="c108d-136">цертификатеревокатионстатус</span><span class="sxs-lookup"><span data-stu-id="c108d-136">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="c108d-137">Отзыв состояния.</span><span class="sxs-lookup"><span data-stu-id="c108d-137">Revoke status.</span></span> <span data-ttu-id="c108d-138">Возможные значения: `none`, `pending`, `issued`, `failed`, `revoked`.</span><span class="sxs-lookup"><span data-stu-id="c108d-138">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="c108d-139">манажеддевицедисплайнаме</span><span class="sxs-lookup"><span data-stu-id="c108d-139">managedDeviceDisplayName</span></span>|<span data-ttu-id="c108d-140">String.</span><span class="sxs-lookup"><span data-stu-id="c108d-140">String</span></span>|<span data-ttu-id="c108d-141">Отображаемое имя устройства</span><span class="sxs-lookup"><span data-stu-id="c108d-141">Device display name</span></span>|
|<span data-ttu-id="c108d-142">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c108d-142">userPrincipalName</span></span>|<span data-ttu-id="c108d-143">String</span><span class="sxs-lookup"><span data-stu-id="c108d-143">String</span></span>|<span data-ttu-id="c108d-144">Имя субъекта-пользователя</span><span class="sxs-lookup"><span data-stu-id="c108d-144">User principal name</span></span>|
|<span data-ttu-id="c108d-145">цертификатикспиратиондатетиме</span><span class="sxs-lookup"><span data-stu-id="c108d-145">certificateExpirationDateTime</span></span>|<span data-ttu-id="c108d-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c108d-146">DateTimeOffset</span></span>|<span data-ttu-id="c108d-147">Дата окончания срока действия сертификата</span><span class="sxs-lookup"><span data-stu-id="c108d-147">Certificate expiry date</span></span>|
|<span data-ttu-id="c108d-148">цертификатеиссуернаме</span><span class="sxs-lookup"><span data-stu-id="c108d-148">certificateIssuerName</span></span>|<span data-ttu-id="c108d-149">String.</span><span class="sxs-lookup"><span data-stu-id="c108d-149">String</span></span>|<span data-ttu-id="c108d-150">Издатель</span><span class="sxs-lookup"><span data-stu-id="c108d-150">Issuer</span></span>|
|<span data-ttu-id="c108d-151">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="c108d-151">certificateThumbprint</span></span>|<span data-ttu-id="c108d-152">String.</span><span class="sxs-lookup"><span data-stu-id="c108d-152">String</span></span>|<span data-ttu-id="c108d-153">Отпечаток</span><span class="sxs-lookup"><span data-stu-id="c108d-153">Thumbprint</span></span>|
|<span data-ttu-id="c108d-154">цертификатесериалнумбер</span><span class="sxs-lookup"><span data-stu-id="c108d-154">certificateSerialNumber</span></span>|<span data-ttu-id="c108d-155">String.</span><span class="sxs-lookup"><span data-stu-id="c108d-155">String</span></span>|<span data-ttu-id="c108d-156">Серийный номер</span><span class="sxs-lookup"><span data-stu-id="c108d-156">Serial number</span></span>|
|<span data-ttu-id="c108d-157">цертификатесубжектнаме</span><span class="sxs-lookup"><span data-stu-id="c108d-157">certificateSubjectName</span></span>|<span data-ttu-id="c108d-158">String.</span><span class="sxs-lookup"><span data-stu-id="c108d-158">String</span></span>|<span data-ttu-id="c108d-159">Имя субъекта сертификата</span><span class="sxs-lookup"><span data-stu-id="c108d-159">Certificate subject name</span></span>|
|<span data-ttu-id="c108d-160">цертификатекэйусажес</span><span class="sxs-lookup"><span data-stu-id="c108d-160">certificateKeyUsages</span></span>|<span data-ttu-id="c108d-161">Int32</span><span class="sxs-lookup"><span data-stu-id="c108d-161">Int32</span></span>|<span data-ttu-id="c108d-162">Использование ключа</span><span class="sxs-lookup"><span data-stu-id="c108d-162">Key Usage</span></span>|
|<span data-ttu-id="c108d-163">цертификатикстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="c108d-163">certificateExtendedKeyUsages</span></span>|<span data-ttu-id="c108d-164">String.</span><span class="sxs-lookup"><span data-stu-id="c108d-164">String</span></span>|<span data-ttu-id="c108d-165">Расширенное использование ключа</span><span class="sxs-lookup"><span data-stu-id="c108d-165">Enhanced Key Usage</span></span>|
|<span data-ttu-id="c108d-166">цертификатеиссуанцедатетиме</span><span class="sxs-lookup"><span data-stu-id="c108d-166">certificateIssuanceDateTime</span></span>|<span data-ttu-id="c108d-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c108d-167">DateTimeOffset</span></span>|<span data-ttu-id="c108d-168">Дата выпуска</span><span class="sxs-lookup"><span data-stu-id="c108d-168">Issuance date</span></span>|



## <a name="response"></a><span data-ttu-id="c108d-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="c108d-169">Response</span></span>
<span data-ttu-id="c108d-170">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [манажедаллдевицецертификатестате](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c108d-170">If successful, this method returns a `200 OK` response code and an updated [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c108d-171">Пример</span><span class="sxs-lookup"><span data-stu-id="c108d-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="c108d-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="c108d-172">Request</span></span>
<span data-ttu-id="c108d-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c108d-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c108d-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="c108d-174">Response</span></span>
<span data-ttu-id="c108d-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c108d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




