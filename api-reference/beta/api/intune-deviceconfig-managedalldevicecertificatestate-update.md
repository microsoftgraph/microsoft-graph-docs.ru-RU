---
title: Обновление Манажедаллдевицецертификатестате
description: Обновление свойств объекта Манажедаллдевицецертификатестате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aac2d6f42ee093c3af745d37da9917db20492006
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35726123"
---
# <a name="update-managedalldevicecertificatestate"></a><span data-ttu-id="9c5aa-103">Обновление Манажедаллдевицецертификатестате</span><span class="sxs-lookup"><span data-stu-id="9c5aa-103">Update managedAllDeviceCertificateState</span></span>

> <span data-ttu-id="9c5aa-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c5aa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9c5aa-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9c5aa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c5aa-106">Обновление свойств объекта [манажедаллдевицецертификатестате](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="9c5aa-106">Update the properties of a [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9c5aa-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9c5aa-107">Prerequisites</span></span>
<span data-ttu-id="9c5aa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c5aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c5aa-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9c5aa-110">Permission type</span></span>|<span data-ttu-id="9c5aa-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9c5aa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c5aa-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9c5aa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9c5aa-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c5aa-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9c5aa-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9c5aa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c5aa-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c5aa-115">Not supported.</span></span>|
|<span data-ttu-id="9c5aa-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9c5aa-116">Application</span></span>|<span data-ttu-id="9c5aa-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c5aa-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c5aa-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9c5aa-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates/{managedAllDeviceCertificateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="9c5aa-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9c5aa-119">Request headers</span></span>
|<span data-ttu-id="9c5aa-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9c5aa-120">Header</span></span>|<span data-ttu-id="9c5aa-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9c5aa-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9c5aa-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9c5aa-122">Authorization</span></span>|<span data-ttu-id="9c5aa-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9c5aa-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9c5aa-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9c5aa-124">Accept</span></span>|<span data-ttu-id="9c5aa-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9c5aa-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c5aa-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9c5aa-126">Request body</span></span>
<span data-ttu-id="9c5aa-127">В тексте запроса добавьте представление объекта [манажедаллдевицецертификатестате](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9c5aa-127">In the request body, supply a JSON representation for the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

<span data-ttu-id="9c5aa-128">В следующей таблице приведены свойства, необходимые при создании [манажедаллдевицецертификатестате](../resources/intune-deviceconfig-managedalldevicecertificatestate.md).</span><span class="sxs-lookup"><span data-stu-id="9c5aa-128">The following table shows the properties that are required when you create the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md).</span></span>

|<span data-ttu-id="9c5aa-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="9c5aa-129">Property</span></span>|<span data-ttu-id="9c5aa-130">Тип</span><span class="sxs-lookup"><span data-stu-id="9c5aa-130">Type</span></span>|<span data-ttu-id="9c5aa-131">Описание</span><span class="sxs-lookup"><span data-stu-id="9c5aa-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c5aa-132">id</span><span class="sxs-lookup"><span data-stu-id="9c5aa-132">id</span></span>|<span data-ttu-id="9c5aa-133">Строка</span><span class="sxs-lookup"><span data-stu-id="9c5aa-133">String</span></span>|<span data-ttu-id="9c5aa-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9c5aa-134">Key of the entity.</span></span>|
|<span data-ttu-id="9c5aa-135">Цертификатеревокестатус</span><span class="sxs-lookup"><span data-stu-id="9c5aa-135">certificateRevokeStatus</span></span>|[<span data-ttu-id="9c5aa-136">Цертификатеревокатионстатус</span><span class="sxs-lookup"><span data-stu-id="9c5aa-136">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="9c5aa-137">Отзыв состояния.</span><span class="sxs-lookup"><span data-stu-id="9c5aa-137">Revoke status.</span></span> <span data-ttu-id="9c5aa-138">Возможные значения: `none`, `pending`, `issued`, `failed`, `revoked`.</span><span class="sxs-lookup"><span data-stu-id="9c5aa-138">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="9c5aa-139">Манажеддевицедисплайнаме</span><span class="sxs-lookup"><span data-stu-id="9c5aa-139">managedDeviceDisplayName</span></span>|<span data-ttu-id="9c5aa-140">String</span><span class="sxs-lookup"><span data-stu-id="9c5aa-140">String</span></span>|<span data-ttu-id="9c5aa-141">Отображаемое имя устройства</span><span class="sxs-lookup"><span data-stu-id="9c5aa-141">Device display name</span></span>|
|<span data-ttu-id="9c5aa-142">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9c5aa-142">userPrincipalName</span></span>|<span data-ttu-id="9c5aa-143">String</span><span class="sxs-lookup"><span data-stu-id="9c5aa-143">String</span></span>|<span data-ttu-id="9c5aa-144">Имя субъекта-пользователя</span><span class="sxs-lookup"><span data-stu-id="9c5aa-144">User principal name</span></span>|
|<span data-ttu-id="9c5aa-145">Цертификатикспиратиондатетиме</span><span class="sxs-lookup"><span data-stu-id="9c5aa-145">certificateExpirationDateTime</span></span>|<span data-ttu-id="9c5aa-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c5aa-146">DateTimeOffset</span></span>|<span data-ttu-id="9c5aa-147">Дата окончания срока действия сертификата</span><span class="sxs-lookup"><span data-stu-id="9c5aa-147">Certificate expiry date</span></span>|
|<span data-ttu-id="9c5aa-148">Цертификатеиссуернаме</span><span class="sxs-lookup"><span data-stu-id="9c5aa-148">certificateIssuerName</span></span>|<span data-ttu-id="9c5aa-149">String</span><span class="sxs-lookup"><span data-stu-id="9c5aa-149">String</span></span>|<span data-ttu-id="9c5aa-150">Издатель</span><span class="sxs-lookup"><span data-stu-id="9c5aa-150">Issuer</span></span>|
|<span data-ttu-id="9c5aa-151">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="9c5aa-151">certificateThumbprint</span></span>|<span data-ttu-id="9c5aa-152">String</span><span class="sxs-lookup"><span data-stu-id="9c5aa-152">String</span></span>|<span data-ttu-id="9c5aa-153">Отпечаток</span><span class="sxs-lookup"><span data-stu-id="9c5aa-153">Thumbprint</span></span>|
|<span data-ttu-id="9c5aa-154">Цертификатесериалнумбер</span><span class="sxs-lookup"><span data-stu-id="9c5aa-154">certificateSerialNumber</span></span>|<span data-ttu-id="9c5aa-155">String</span><span class="sxs-lookup"><span data-stu-id="9c5aa-155">String</span></span>|<span data-ttu-id="9c5aa-156">Серийный номер</span><span class="sxs-lookup"><span data-stu-id="9c5aa-156">Serial number</span></span>|
|<span data-ttu-id="9c5aa-157">Цертификатесубжектнаме</span><span class="sxs-lookup"><span data-stu-id="9c5aa-157">certificateSubjectName</span></span>|<span data-ttu-id="9c5aa-158">String</span><span class="sxs-lookup"><span data-stu-id="9c5aa-158">String</span></span>|<span data-ttu-id="9c5aa-159">Имя субъекта сертификата</span><span class="sxs-lookup"><span data-stu-id="9c5aa-159">Certificate subject name</span></span>|
|<span data-ttu-id="9c5aa-160">Цертификатекэйусажес</span><span class="sxs-lookup"><span data-stu-id="9c5aa-160">certificateKeyUsages</span></span>|<span data-ttu-id="9c5aa-161">Int32</span><span class="sxs-lookup"><span data-stu-id="9c5aa-161">Int32</span></span>|<span data-ttu-id="9c5aa-162">Использование ключа</span><span class="sxs-lookup"><span data-stu-id="9c5aa-162">Key Usage</span></span>|
|<span data-ttu-id="9c5aa-163">Цертификатикстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="9c5aa-163">certificateExtendedKeyUsages</span></span>|<span data-ttu-id="9c5aa-164">String</span><span class="sxs-lookup"><span data-stu-id="9c5aa-164">String</span></span>|<span data-ttu-id="9c5aa-165">Расширенное использование ключа</span><span class="sxs-lookup"><span data-stu-id="9c5aa-165">Enhanced Key Usage</span></span>|
|<span data-ttu-id="9c5aa-166">Цертификатеиссуанцедатетиме</span><span class="sxs-lookup"><span data-stu-id="9c5aa-166">certificateIssuanceDateTime</span></span>|<span data-ttu-id="9c5aa-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c5aa-167">DateTimeOffset</span></span>|<span data-ttu-id="9c5aa-168">Дата выпуска</span><span class="sxs-lookup"><span data-stu-id="9c5aa-168">Issuance date</span></span>|



## <a name="response"></a><span data-ttu-id="9c5aa-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c5aa-169">Response</span></span>
<span data-ttu-id="9c5aa-170">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [манажедаллдевицецертификатестате](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9c5aa-170">If successful, this method returns a `200 OK` response code and an updated [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c5aa-171">Пример</span><span class="sxs-lookup"><span data-stu-id="9c5aa-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="9c5aa-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="9c5aa-172">Request</span></span>
<span data-ttu-id="9c5aa-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9c5aa-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9c5aa-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c5aa-174">Response</span></span>
<span data-ttu-id="9c5aa-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9c5aa-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





