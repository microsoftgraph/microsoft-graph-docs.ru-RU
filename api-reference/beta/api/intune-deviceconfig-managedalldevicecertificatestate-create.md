---
title: Создание Манажедаллдевицецертификатестате
description: Создание нового объекта Манажедаллдевицецертификатестате.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b0924b2b581f758c256072d26531391b51c86453
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43432221"
---
# <a name="create-managedalldevicecertificatestate"></a><span data-ttu-id="a2cc8-103">Создание Манажедаллдевицецертификатестате</span><span class="sxs-lookup"><span data-stu-id="a2cc8-103">Create managedAllDeviceCertificateState</span></span>

<span data-ttu-id="a2cc8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2cc8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a2cc8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2cc8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a2cc8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a2cc8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2cc8-107">Создание нового объекта [манажедаллдевицецертификатестате](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="a2cc8-107">Create a new [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a2cc8-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a2cc8-108">Prerequisites</span></span>
<span data-ttu-id="a2cc8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2cc8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2cc8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a2cc8-111">Permission type</span></span>|<span data-ttu-id="a2cc8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a2cc8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2cc8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a2cc8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a2cc8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2cc8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a2cc8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a2cc8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2cc8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2cc8-116">Not supported.</span></span>|
|<span data-ttu-id="a2cc8-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a2cc8-117">Application</span></span>|<span data-ttu-id="a2cc8-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2cc8-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2cc8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a2cc8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates
```

## <a name="request-headers"></a><span data-ttu-id="a2cc8-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a2cc8-120">Request headers</span></span>
|<span data-ttu-id="a2cc8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a2cc8-121">Header</span></span>|<span data-ttu-id="a2cc8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a2cc8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2cc8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2cc8-123">Authorization</span></span>|<span data-ttu-id="a2cc8-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a2cc8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2cc8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a2cc8-125">Accept</span></span>|<span data-ttu-id="a2cc8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a2cc8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2cc8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a2cc8-127">Request body</span></span>
<span data-ttu-id="a2cc8-128">В тексте запроса добавьте представление объекта Манажедаллдевицецертификатестате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a2cc8-128">In the request body, supply a JSON representation for the managedAllDeviceCertificateState object.</span></span>

<span data-ttu-id="a2cc8-129">В следующей таблице приведены свойства, необходимые при создании Манажедаллдевицецертификатестате.</span><span class="sxs-lookup"><span data-stu-id="a2cc8-129">The following table shows the properties that are required when you create the managedAllDeviceCertificateState.</span></span>

|<span data-ttu-id="a2cc8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a2cc8-130">Property</span></span>|<span data-ttu-id="a2cc8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a2cc8-131">Type</span></span>|<span data-ttu-id="a2cc8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a2cc8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2cc8-133">id</span><span class="sxs-lookup"><span data-stu-id="a2cc8-133">id</span></span>|<span data-ttu-id="a2cc8-134">Строка</span><span class="sxs-lookup"><span data-stu-id="a2cc8-134">String</span></span>|<span data-ttu-id="a2cc8-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a2cc8-135">Key of the entity.</span></span>|
|<span data-ttu-id="a2cc8-136">цертификатеревокестатус</span><span class="sxs-lookup"><span data-stu-id="a2cc8-136">certificateRevokeStatus</span></span>|[<span data-ttu-id="a2cc8-137">цертификатеревокатионстатус</span><span class="sxs-lookup"><span data-stu-id="a2cc8-137">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="a2cc8-138">Отзыв состояния.</span><span class="sxs-lookup"><span data-stu-id="a2cc8-138">Revoke status.</span></span> <span data-ttu-id="a2cc8-139">Возможные значения: `none`, `pending`, `issued`, `failed`, `revoked`.</span><span class="sxs-lookup"><span data-stu-id="a2cc8-139">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="a2cc8-140">манажеддевицедисплайнаме</span><span class="sxs-lookup"><span data-stu-id="a2cc8-140">managedDeviceDisplayName</span></span>|<span data-ttu-id="a2cc8-141">String</span><span class="sxs-lookup"><span data-stu-id="a2cc8-141">String</span></span>|<span data-ttu-id="a2cc8-142">Отображаемое имя устройства</span><span class="sxs-lookup"><span data-stu-id="a2cc8-142">Device display name</span></span>|
|<span data-ttu-id="a2cc8-143">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a2cc8-143">userPrincipalName</span></span>|<span data-ttu-id="a2cc8-144">String</span><span class="sxs-lookup"><span data-stu-id="a2cc8-144">String</span></span>|<span data-ttu-id="a2cc8-145">Имя субъекта-пользователя</span><span class="sxs-lookup"><span data-stu-id="a2cc8-145">User principal name</span></span>|
|<span data-ttu-id="a2cc8-146">цертификатикспиратиондатетиме</span><span class="sxs-lookup"><span data-stu-id="a2cc8-146">certificateExpirationDateTime</span></span>|<span data-ttu-id="a2cc8-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2cc8-147">DateTimeOffset</span></span>|<span data-ttu-id="a2cc8-148">Дата окончания срока действия сертификата</span><span class="sxs-lookup"><span data-stu-id="a2cc8-148">Certificate expiry date</span></span>|
|<span data-ttu-id="a2cc8-149">цертификатеиссуернаме</span><span class="sxs-lookup"><span data-stu-id="a2cc8-149">certificateIssuerName</span></span>|<span data-ttu-id="a2cc8-150">String</span><span class="sxs-lookup"><span data-stu-id="a2cc8-150">String</span></span>|<span data-ttu-id="a2cc8-151">Издатель</span><span class="sxs-lookup"><span data-stu-id="a2cc8-151">Issuer</span></span>|
|<span data-ttu-id="a2cc8-152">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="a2cc8-152">certificateThumbprint</span></span>|<span data-ttu-id="a2cc8-153">String</span><span class="sxs-lookup"><span data-stu-id="a2cc8-153">String</span></span>|<span data-ttu-id="a2cc8-154">Отпечаток</span><span class="sxs-lookup"><span data-stu-id="a2cc8-154">Thumbprint</span></span>|
|<span data-ttu-id="a2cc8-155">цертификатесериалнумбер</span><span class="sxs-lookup"><span data-stu-id="a2cc8-155">certificateSerialNumber</span></span>|<span data-ttu-id="a2cc8-156">String</span><span class="sxs-lookup"><span data-stu-id="a2cc8-156">String</span></span>|<span data-ttu-id="a2cc8-157">Серийный номер</span><span class="sxs-lookup"><span data-stu-id="a2cc8-157">Serial number</span></span>|
|<span data-ttu-id="a2cc8-158">цертификатесубжектнаме</span><span class="sxs-lookup"><span data-stu-id="a2cc8-158">certificateSubjectName</span></span>|<span data-ttu-id="a2cc8-159">String</span><span class="sxs-lookup"><span data-stu-id="a2cc8-159">String</span></span>|<span data-ttu-id="a2cc8-160">Имя субъекта сертификата</span><span class="sxs-lookup"><span data-stu-id="a2cc8-160">Certificate subject name</span></span>|
|<span data-ttu-id="a2cc8-161">цертификатекэйусажес</span><span class="sxs-lookup"><span data-stu-id="a2cc8-161">certificateKeyUsages</span></span>|<span data-ttu-id="a2cc8-162">Int32</span><span class="sxs-lookup"><span data-stu-id="a2cc8-162">Int32</span></span>|<span data-ttu-id="a2cc8-163">Использование ключа</span><span class="sxs-lookup"><span data-stu-id="a2cc8-163">Key Usage</span></span>|
|<span data-ttu-id="a2cc8-164">цертификатикстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="a2cc8-164">certificateExtendedKeyUsages</span></span>|<span data-ttu-id="a2cc8-165">String</span><span class="sxs-lookup"><span data-stu-id="a2cc8-165">String</span></span>|<span data-ttu-id="a2cc8-166">Расширенное использование ключа</span><span class="sxs-lookup"><span data-stu-id="a2cc8-166">Enhanced Key Usage</span></span>|
|<span data-ttu-id="a2cc8-167">цертификатеиссуанцедатетиме</span><span class="sxs-lookup"><span data-stu-id="a2cc8-167">certificateIssuanceDateTime</span></span>|<span data-ttu-id="a2cc8-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2cc8-168">DateTimeOffset</span></span>|<span data-ttu-id="a2cc8-169">Дата выпуска</span><span class="sxs-lookup"><span data-stu-id="a2cc8-169">Issuance date</span></span>|



## <a name="response"></a><span data-ttu-id="a2cc8-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2cc8-170">Response</span></span>
<span data-ttu-id="a2cc8-171">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [манажедаллдевицецертификатестате](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a2cc8-171">If successful, this method returns a `201 Created` response code and a [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2cc8-172">Пример</span><span class="sxs-lookup"><span data-stu-id="a2cc8-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="a2cc8-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="a2cc8-173">Request</span></span>
<span data-ttu-id="a2cc8-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a2cc8-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a2cc8-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2cc8-175">Response</span></span>
<span data-ttu-id="a2cc8-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a2cc8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



