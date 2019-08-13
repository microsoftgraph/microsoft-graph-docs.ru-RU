---
title: Обновление Манажедаллдевицецертификатестате
description: Обновление свойств объекта Манажедаллдевицецертификатестате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 520afd6fb7b2980b8c263dff2f44b52ac2c2f610
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36345619"
---
# <a name="update-managedalldevicecertificatestate"></a><span data-ttu-id="c708f-103">Обновление Манажедаллдевицецертификатестате</span><span class="sxs-lookup"><span data-stu-id="c708f-103">Update managedAllDeviceCertificateState</span></span>

> <span data-ttu-id="c708f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c708f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c708f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c708f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c708f-106">Обновление свойств объекта [манажедаллдевицецертификатестате](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="c708f-106">Update the properties of a [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c708f-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c708f-107">Prerequisites</span></span>
<span data-ttu-id="c708f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c708f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c708f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c708f-110">Permission type</span></span>|<span data-ttu-id="c708f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c708f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c708f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c708f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c708f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c708f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c708f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c708f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c708f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c708f-115">Not supported.</span></span>|
|<span data-ttu-id="c708f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c708f-116">Application</span></span>|<span data-ttu-id="c708f-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c708f-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c708f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c708f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates/{managedAllDeviceCertificateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="c708f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c708f-119">Request headers</span></span>
|<span data-ttu-id="c708f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c708f-120">Header</span></span>|<span data-ttu-id="c708f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c708f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c708f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c708f-122">Authorization</span></span>|<span data-ttu-id="c708f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c708f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c708f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c708f-124">Accept</span></span>|<span data-ttu-id="c708f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c708f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c708f-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c708f-126">Request body</span></span>
<span data-ttu-id="c708f-127">В тексте запроса добавьте представление объекта [манажедаллдевицецертификатестате](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c708f-127">In the request body, supply a JSON representation for the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

<span data-ttu-id="c708f-128">В следующей таблице приведены свойства, необходимые при создании [манажедаллдевицецертификатестате](../resources/intune-deviceconfig-managedalldevicecertificatestate.md).</span><span class="sxs-lookup"><span data-stu-id="c708f-128">The following table shows the properties that are required when you create the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md).</span></span>

|<span data-ttu-id="c708f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c708f-129">Property</span></span>|<span data-ttu-id="c708f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c708f-130">Type</span></span>|<span data-ttu-id="c708f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c708f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c708f-132">id</span><span class="sxs-lookup"><span data-stu-id="c708f-132">id</span></span>|<span data-ttu-id="c708f-133">Строка</span><span class="sxs-lookup"><span data-stu-id="c708f-133">String</span></span>|<span data-ttu-id="c708f-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c708f-134">Key of the entity.</span></span>|
|<span data-ttu-id="c708f-135">цертификатеревокестатус</span><span class="sxs-lookup"><span data-stu-id="c708f-135">certificateRevokeStatus</span></span>|[<span data-ttu-id="c708f-136">цертификатеревокатионстатус</span><span class="sxs-lookup"><span data-stu-id="c708f-136">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="c708f-137">Отзыв состояния.</span><span class="sxs-lookup"><span data-stu-id="c708f-137">Revoke status.</span></span> <span data-ttu-id="c708f-138">Возможные значения: `none`, `pending`, `issued`, `failed`, `revoked`.</span><span class="sxs-lookup"><span data-stu-id="c708f-138">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="c708f-139">манажеддевицедисплайнаме</span><span class="sxs-lookup"><span data-stu-id="c708f-139">managedDeviceDisplayName</span></span>|<span data-ttu-id="c708f-140">String</span><span class="sxs-lookup"><span data-stu-id="c708f-140">String</span></span>|<span data-ttu-id="c708f-141">Отображаемое имя устройства</span><span class="sxs-lookup"><span data-stu-id="c708f-141">Device display name</span></span>|
|<span data-ttu-id="c708f-142">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c708f-142">userPrincipalName</span></span>|<span data-ttu-id="c708f-143">String</span><span class="sxs-lookup"><span data-stu-id="c708f-143">String</span></span>|<span data-ttu-id="c708f-144">Имя субъекта-пользователя</span><span class="sxs-lookup"><span data-stu-id="c708f-144">User principal name</span></span>|
|<span data-ttu-id="c708f-145">цертификатикспиратиондатетиме</span><span class="sxs-lookup"><span data-stu-id="c708f-145">certificateExpirationDateTime</span></span>|<span data-ttu-id="c708f-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c708f-146">DateTimeOffset</span></span>|<span data-ttu-id="c708f-147">Дата окончания срока действия сертификата</span><span class="sxs-lookup"><span data-stu-id="c708f-147">Certificate expiry date</span></span>|
|<span data-ttu-id="c708f-148">цертификатеиссуернаме</span><span class="sxs-lookup"><span data-stu-id="c708f-148">certificateIssuerName</span></span>|<span data-ttu-id="c708f-149">String</span><span class="sxs-lookup"><span data-stu-id="c708f-149">String</span></span>|<span data-ttu-id="c708f-150">Издатель</span><span class="sxs-lookup"><span data-stu-id="c708f-150">Issuer</span></span>|
|<span data-ttu-id="c708f-151">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="c708f-151">certificateThumbprint</span></span>|<span data-ttu-id="c708f-152">String</span><span class="sxs-lookup"><span data-stu-id="c708f-152">String</span></span>|<span data-ttu-id="c708f-153">Отпечаток</span><span class="sxs-lookup"><span data-stu-id="c708f-153">Thumbprint</span></span>|
|<span data-ttu-id="c708f-154">цертификатесериалнумбер</span><span class="sxs-lookup"><span data-stu-id="c708f-154">certificateSerialNumber</span></span>|<span data-ttu-id="c708f-155">String</span><span class="sxs-lookup"><span data-stu-id="c708f-155">String</span></span>|<span data-ttu-id="c708f-156">Серийный номер</span><span class="sxs-lookup"><span data-stu-id="c708f-156">Serial number</span></span>|
|<span data-ttu-id="c708f-157">цертификатесубжектнаме</span><span class="sxs-lookup"><span data-stu-id="c708f-157">certificateSubjectName</span></span>|<span data-ttu-id="c708f-158">String</span><span class="sxs-lookup"><span data-stu-id="c708f-158">String</span></span>|<span data-ttu-id="c708f-159">Имя субъекта сертификата</span><span class="sxs-lookup"><span data-stu-id="c708f-159">Certificate subject name</span></span>|
|<span data-ttu-id="c708f-160">цертификатекэйусажес</span><span class="sxs-lookup"><span data-stu-id="c708f-160">certificateKeyUsages</span></span>|<span data-ttu-id="c708f-161">Int32</span><span class="sxs-lookup"><span data-stu-id="c708f-161">Int32</span></span>|<span data-ttu-id="c708f-162">Использование ключа</span><span class="sxs-lookup"><span data-stu-id="c708f-162">Key Usage</span></span>|
|<span data-ttu-id="c708f-163">цертификатикстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="c708f-163">certificateExtendedKeyUsages</span></span>|<span data-ttu-id="c708f-164">String</span><span class="sxs-lookup"><span data-stu-id="c708f-164">String</span></span>|<span data-ttu-id="c708f-165">Расширенное использование ключа</span><span class="sxs-lookup"><span data-stu-id="c708f-165">Enhanced Key Usage</span></span>|
|<span data-ttu-id="c708f-166">цертификатеиссуанцедатетиме</span><span class="sxs-lookup"><span data-stu-id="c708f-166">certificateIssuanceDateTime</span></span>|<span data-ttu-id="c708f-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c708f-167">DateTimeOffset</span></span>|<span data-ttu-id="c708f-168">Дата выпуска</span><span class="sxs-lookup"><span data-stu-id="c708f-168">Issuance date</span></span>|



## <a name="response"></a><span data-ttu-id="c708f-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="c708f-169">Response</span></span>
<span data-ttu-id="c708f-170">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [манажедаллдевицецертификатестате](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c708f-170">If successful, this method returns a `200 OK` response code and an updated [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c708f-171">Пример</span><span class="sxs-lookup"><span data-stu-id="c708f-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="c708f-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="c708f-172">Request</span></span>
<span data-ttu-id="c708f-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c708f-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c708f-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="c708f-174">Response</span></span>
<span data-ttu-id="c708f-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c708f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






