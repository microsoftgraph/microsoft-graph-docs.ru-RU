---
title: Создание Манажедаллдевицецертификатестате
description: Создание нового объекта Манажедаллдевицецертификатестате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 50877255e069c70749ae77b515d7f45a90398a33
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36338590"
---
# <a name="create-managedalldevicecertificatestate"></a><span data-ttu-id="111fc-103">Создание Манажедаллдевицецертификатестате</span><span class="sxs-lookup"><span data-stu-id="111fc-103">Create managedAllDeviceCertificateState</span></span>

> <span data-ttu-id="111fc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="111fc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="111fc-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="111fc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="111fc-106">Создание нового объекта [манажедаллдевицецертификатестате](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="111fc-106">Create a new [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="111fc-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="111fc-107">Prerequisites</span></span>
<span data-ttu-id="111fc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="111fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="111fc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="111fc-110">Permission type</span></span>|<span data-ttu-id="111fc-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="111fc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="111fc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="111fc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="111fc-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="111fc-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="111fc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="111fc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="111fc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="111fc-115">Not supported.</span></span>|
|<span data-ttu-id="111fc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="111fc-116">Application</span></span>|<span data-ttu-id="111fc-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="111fc-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="111fc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="111fc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates
```

## <a name="request-headers"></a><span data-ttu-id="111fc-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="111fc-119">Request headers</span></span>
|<span data-ttu-id="111fc-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="111fc-120">Header</span></span>|<span data-ttu-id="111fc-121">Значение</span><span class="sxs-lookup"><span data-stu-id="111fc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="111fc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="111fc-122">Authorization</span></span>|<span data-ttu-id="111fc-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="111fc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="111fc-124">Accept</span><span class="sxs-lookup"><span data-stu-id="111fc-124">Accept</span></span>|<span data-ttu-id="111fc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="111fc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="111fc-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="111fc-126">Request body</span></span>
<span data-ttu-id="111fc-127">В тексте запроса добавьте представление объекта Манажедаллдевицецертификатестате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="111fc-127">In the request body, supply a JSON representation for the managedAllDeviceCertificateState object.</span></span>

<span data-ttu-id="111fc-128">В следующей таблице приведены свойства, необходимые при создании Манажедаллдевицецертификатестате.</span><span class="sxs-lookup"><span data-stu-id="111fc-128">The following table shows the properties that are required when you create the managedAllDeviceCertificateState.</span></span>

|<span data-ttu-id="111fc-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="111fc-129">Property</span></span>|<span data-ttu-id="111fc-130">Тип</span><span class="sxs-lookup"><span data-stu-id="111fc-130">Type</span></span>|<span data-ttu-id="111fc-131">Описание</span><span class="sxs-lookup"><span data-stu-id="111fc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="111fc-132">id</span><span class="sxs-lookup"><span data-stu-id="111fc-132">id</span></span>|<span data-ttu-id="111fc-133">Строка</span><span class="sxs-lookup"><span data-stu-id="111fc-133">String</span></span>|<span data-ttu-id="111fc-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="111fc-134">Key of the entity.</span></span>|
|<span data-ttu-id="111fc-135">цертификатеревокестатус</span><span class="sxs-lookup"><span data-stu-id="111fc-135">certificateRevokeStatus</span></span>|[<span data-ttu-id="111fc-136">цертификатеревокатионстатус</span><span class="sxs-lookup"><span data-stu-id="111fc-136">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="111fc-137">Отзыв состояния.</span><span class="sxs-lookup"><span data-stu-id="111fc-137">Revoke status.</span></span> <span data-ttu-id="111fc-138">Возможные значения: `none`, `pending`, `issued`, `failed`, `revoked`.</span><span class="sxs-lookup"><span data-stu-id="111fc-138">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="111fc-139">манажеддевицедисплайнаме</span><span class="sxs-lookup"><span data-stu-id="111fc-139">managedDeviceDisplayName</span></span>|<span data-ttu-id="111fc-140">String</span><span class="sxs-lookup"><span data-stu-id="111fc-140">String</span></span>|<span data-ttu-id="111fc-141">Отображаемое имя устройства</span><span class="sxs-lookup"><span data-stu-id="111fc-141">Device display name</span></span>|
|<span data-ttu-id="111fc-142">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="111fc-142">userPrincipalName</span></span>|<span data-ttu-id="111fc-143">String</span><span class="sxs-lookup"><span data-stu-id="111fc-143">String</span></span>|<span data-ttu-id="111fc-144">Имя субъекта-пользователя</span><span class="sxs-lookup"><span data-stu-id="111fc-144">User principal name</span></span>|
|<span data-ttu-id="111fc-145">цертификатикспиратиондатетиме</span><span class="sxs-lookup"><span data-stu-id="111fc-145">certificateExpirationDateTime</span></span>|<span data-ttu-id="111fc-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="111fc-146">DateTimeOffset</span></span>|<span data-ttu-id="111fc-147">Дата окончания срока действия сертификата</span><span class="sxs-lookup"><span data-stu-id="111fc-147">Certificate expiry date</span></span>|
|<span data-ttu-id="111fc-148">цертификатеиссуернаме</span><span class="sxs-lookup"><span data-stu-id="111fc-148">certificateIssuerName</span></span>|<span data-ttu-id="111fc-149">String</span><span class="sxs-lookup"><span data-stu-id="111fc-149">String</span></span>|<span data-ttu-id="111fc-150">Издатель</span><span class="sxs-lookup"><span data-stu-id="111fc-150">Issuer</span></span>|
|<span data-ttu-id="111fc-151">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="111fc-151">certificateThumbprint</span></span>|<span data-ttu-id="111fc-152">String</span><span class="sxs-lookup"><span data-stu-id="111fc-152">String</span></span>|<span data-ttu-id="111fc-153">Отпечаток</span><span class="sxs-lookup"><span data-stu-id="111fc-153">Thumbprint</span></span>|
|<span data-ttu-id="111fc-154">цертификатесериалнумбер</span><span class="sxs-lookup"><span data-stu-id="111fc-154">certificateSerialNumber</span></span>|<span data-ttu-id="111fc-155">String</span><span class="sxs-lookup"><span data-stu-id="111fc-155">String</span></span>|<span data-ttu-id="111fc-156">Серийный номер</span><span class="sxs-lookup"><span data-stu-id="111fc-156">Serial number</span></span>|
|<span data-ttu-id="111fc-157">цертификатесубжектнаме</span><span class="sxs-lookup"><span data-stu-id="111fc-157">certificateSubjectName</span></span>|<span data-ttu-id="111fc-158">String</span><span class="sxs-lookup"><span data-stu-id="111fc-158">String</span></span>|<span data-ttu-id="111fc-159">Имя субъекта сертификата</span><span class="sxs-lookup"><span data-stu-id="111fc-159">Certificate subject name</span></span>|
|<span data-ttu-id="111fc-160">цертификатекэйусажес</span><span class="sxs-lookup"><span data-stu-id="111fc-160">certificateKeyUsages</span></span>|<span data-ttu-id="111fc-161">Int32</span><span class="sxs-lookup"><span data-stu-id="111fc-161">Int32</span></span>|<span data-ttu-id="111fc-162">Использование ключа</span><span class="sxs-lookup"><span data-stu-id="111fc-162">Key Usage</span></span>|
|<span data-ttu-id="111fc-163">цертификатикстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="111fc-163">certificateExtendedKeyUsages</span></span>|<span data-ttu-id="111fc-164">String</span><span class="sxs-lookup"><span data-stu-id="111fc-164">String</span></span>|<span data-ttu-id="111fc-165">Расширенное использование ключа</span><span class="sxs-lookup"><span data-stu-id="111fc-165">Enhanced Key Usage</span></span>|
|<span data-ttu-id="111fc-166">цертификатеиссуанцедатетиме</span><span class="sxs-lookup"><span data-stu-id="111fc-166">certificateIssuanceDateTime</span></span>|<span data-ttu-id="111fc-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="111fc-167">DateTimeOffset</span></span>|<span data-ttu-id="111fc-168">Дата выпуска</span><span class="sxs-lookup"><span data-stu-id="111fc-168">Issuance date</span></span>|



## <a name="response"></a><span data-ttu-id="111fc-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="111fc-169">Response</span></span>
<span data-ttu-id="111fc-170">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [манажедаллдевицецертификатестате](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="111fc-170">If successful, this method returns a `201 Created` response code and a [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="111fc-171">Пример</span><span class="sxs-lookup"><span data-stu-id="111fc-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="111fc-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="111fc-172">Request</span></span>
<span data-ttu-id="111fc-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="111fc-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="111fc-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="111fc-174">Response</span></span>
<span data-ttu-id="111fc-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="111fc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






