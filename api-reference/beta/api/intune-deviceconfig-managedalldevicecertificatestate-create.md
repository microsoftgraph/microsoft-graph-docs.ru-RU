---
title: Создание Манажедаллдевицецертификатестате
description: Создание нового объекта Манажедаллдевицецертификатестате.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 44c9b00511dc3bd8e4a1c9fb9226e6e62a80dc22
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "45122975"
---
# <a name="create-managedalldevicecertificatestate"></a><span data-ttu-id="42a45-103">Создание Манажедаллдевицецертификатестате</span><span class="sxs-lookup"><span data-stu-id="42a45-103">Create managedAllDeviceCertificateState</span></span>

<span data-ttu-id="42a45-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42a45-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="42a45-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42a45-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42a45-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="42a45-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42a45-107">Создание нового объекта [манажедаллдевицецертификатестате](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="42a45-107">Create a new [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42a45-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="42a45-108">Prerequisites</span></span>
<span data-ttu-id="42a45-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42a45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42a45-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="42a45-111">Permission type</span></span>|<span data-ttu-id="42a45-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="42a45-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42a45-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="42a45-113">Delegated (work or school account)</span></span>|<span data-ttu-id="42a45-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42a45-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="42a45-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="42a45-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42a45-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42a45-116">Not supported.</span></span>|
|<span data-ttu-id="42a45-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="42a45-117">Application</span></span>|<span data-ttu-id="42a45-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42a45-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="42a45-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="42a45-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates
```

## <a name="request-headers"></a><span data-ttu-id="42a45-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="42a45-120">Request headers</span></span>
|<span data-ttu-id="42a45-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="42a45-121">Header</span></span>|<span data-ttu-id="42a45-122">Значение</span><span class="sxs-lookup"><span data-stu-id="42a45-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42a45-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="42a45-123">Authorization</span></span>|<span data-ttu-id="42a45-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="42a45-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42a45-125">Accept</span><span class="sxs-lookup"><span data-stu-id="42a45-125">Accept</span></span>|<span data-ttu-id="42a45-126">application/json</span><span class="sxs-lookup"><span data-stu-id="42a45-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42a45-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="42a45-127">Request body</span></span>
<span data-ttu-id="42a45-128">В тексте запроса добавьте представление объекта Манажедаллдевицецертификатестате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="42a45-128">In the request body, supply a JSON representation for the managedAllDeviceCertificateState object.</span></span>

<span data-ttu-id="42a45-129">В следующей таблице приведены свойства, необходимые при создании Манажедаллдевицецертификатестате.</span><span class="sxs-lookup"><span data-stu-id="42a45-129">The following table shows the properties that are required when you create the managedAllDeviceCertificateState.</span></span>

|<span data-ttu-id="42a45-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="42a45-130">Property</span></span>|<span data-ttu-id="42a45-131">Тип</span><span class="sxs-lookup"><span data-stu-id="42a45-131">Type</span></span>|<span data-ttu-id="42a45-132">Описание</span><span class="sxs-lookup"><span data-stu-id="42a45-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42a45-133">id</span><span class="sxs-lookup"><span data-stu-id="42a45-133">id</span></span>|<span data-ttu-id="42a45-134">Строка</span><span class="sxs-lookup"><span data-stu-id="42a45-134">String</span></span>|<span data-ttu-id="42a45-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="42a45-135">Key of the entity.</span></span>|
|<span data-ttu-id="42a45-136">цертификатеревокестатус</span><span class="sxs-lookup"><span data-stu-id="42a45-136">certificateRevokeStatus</span></span>|[<span data-ttu-id="42a45-137">цертификатеревокатионстатус</span><span class="sxs-lookup"><span data-stu-id="42a45-137">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="42a45-138">Отзыв состояния.</span><span class="sxs-lookup"><span data-stu-id="42a45-138">Revoke status.</span></span> <span data-ttu-id="42a45-139">Возможные значения: `none`, `pending`, `issued`, `failed`, `revoked`.</span><span class="sxs-lookup"><span data-stu-id="42a45-139">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="42a45-140">цертификатеревокестатусластчанжедатетиме</span><span class="sxs-lookup"><span data-stu-id="42a45-140">certificateRevokeStatusLastChangeDateTime</span></span>|<span data-ttu-id="42a45-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42a45-141">DateTimeOffset</span></span>|<span data-ttu-id="42a45-142">Время последнего изменения состояния отзыва</span><span class="sxs-lookup"><span data-stu-id="42a45-142">The time the revoke status was last changed</span></span>|
|<span data-ttu-id="42a45-143">манажеддевицедисплайнаме</span><span class="sxs-lookup"><span data-stu-id="42a45-143">managedDeviceDisplayName</span></span>|<span data-ttu-id="42a45-144">String</span><span class="sxs-lookup"><span data-stu-id="42a45-144">String</span></span>|<span data-ttu-id="42a45-145">Отображаемое имя устройства</span><span class="sxs-lookup"><span data-stu-id="42a45-145">Device display name</span></span>|
|<span data-ttu-id="42a45-146">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="42a45-146">userPrincipalName</span></span>|<span data-ttu-id="42a45-147">String</span><span class="sxs-lookup"><span data-stu-id="42a45-147">String</span></span>|<span data-ttu-id="42a45-148">Имя субъекта-пользователя</span><span class="sxs-lookup"><span data-stu-id="42a45-148">User principal name</span></span>|
|<span data-ttu-id="42a45-149">цертификатикспиратиондатетиме</span><span class="sxs-lookup"><span data-stu-id="42a45-149">certificateExpirationDateTime</span></span>|<span data-ttu-id="42a45-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42a45-150">DateTimeOffset</span></span>|<span data-ttu-id="42a45-151">Дата окончания срока действия сертификата</span><span class="sxs-lookup"><span data-stu-id="42a45-151">Certificate expiry date</span></span>|
|<span data-ttu-id="42a45-152">цертификатеиссуернаме</span><span class="sxs-lookup"><span data-stu-id="42a45-152">certificateIssuerName</span></span>|<span data-ttu-id="42a45-153">String</span><span class="sxs-lookup"><span data-stu-id="42a45-153">String</span></span>|<span data-ttu-id="42a45-154">Издатель</span><span class="sxs-lookup"><span data-stu-id="42a45-154">Issuer</span></span>|
|<span data-ttu-id="42a45-155">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="42a45-155">certificateThumbprint</span></span>|<span data-ttu-id="42a45-156">String</span><span class="sxs-lookup"><span data-stu-id="42a45-156">String</span></span>|<span data-ttu-id="42a45-157">Отпечаток</span><span class="sxs-lookup"><span data-stu-id="42a45-157">Thumbprint</span></span>|
|<span data-ttu-id="42a45-158">цертификатесериалнумбер</span><span class="sxs-lookup"><span data-stu-id="42a45-158">certificateSerialNumber</span></span>|<span data-ttu-id="42a45-159">String</span><span class="sxs-lookup"><span data-stu-id="42a45-159">String</span></span>|<span data-ttu-id="42a45-160">Серийный номер</span><span class="sxs-lookup"><span data-stu-id="42a45-160">Serial number</span></span>|
|<span data-ttu-id="42a45-161">цертификатесубжектнаме</span><span class="sxs-lookup"><span data-stu-id="42a45-161">certificateSubjectName</span></span>|<span data-ttu-id="42a45-162">String</span><span class="sxs-lookup"><span data-stu-id="42a45-162">String</span></span>|<span data-ttu-id="42a45-163">Имя субъекта сертификата</span><span class="sxs-lookup"><span data-stu-id="42a45-163">Certificate subject name</span></span>|
|<span data-ttu-id="42a45-164">цертификатекэйусажес</span><span class="sxs-lookup"><span data-stu-id="42a45-164">certificateKeyUsages</span></span>|<span data-ttu-id="42a45-165">Int32</span><span class="sxs-lookup"><span data-stu-id="42a45-165">Int32</span></span>|<span data-ttu-id="42a45-166">Использование ключа</span><span class="sxs-lookup"><span data-stu-id="42a45-166">Key Usage</span></span>|
|<span data-ttu-id="42a45-167">цертификатикстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="42a45-167">certificateExtendedKeyUsages</span></span>|<span data-ttu-id="42a45-168">String</span><span class="sxs-lookup"><span data-stu-id="42a45-168">String</span></span>|<span data-ttu-id="42a45-169">Расширенное использование ключа</span><span class="sxs-lookup"><span data-stu-id="42a45-169">Enhanced Key Usage</span></span>|
|<span data-ttu-id="42a45-170">цертификатеиссуанцедатетиме</span><span class="sxs-lookup"><span data-stu-id="42a45-170">certificateIssuanceDateTime</span></span>|<span data-ttu-id="42a45-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42a45-171">DateTimeOffset</span></span>|<span data-ttu-id="42a45-172">Дата выпуска</span><span class="sxs-lookup"><span data-stu-id="42a45-172">Issuance date</span></span>|



## <a name="response"></a><span data-ttu-id="42a45-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="42a45-173">Response</span></span>
<span data-ttu-id="42a45-174">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [манажедаллдевицецертификатестате](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="42a45-174">If successful, this method returns a `201 Created` response code and a [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42a45-175">Пример</span><span class="sxs-lookup"><span data-stu-id="42a45-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="42a45-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="42a45-176">Request</span></span>
<span data-ttu-id="42a45-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="42a45-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates
Content-type: application/json
Content-length: 820

{
  "@odata.type": "#microsoft.graph.managedAllDeviceCertificateState",
  "certificateRevokeStatus": "pending",
  "certificateRevokeStatusLastChangeDateTime": "2016-12-31T23:59:34.9547208-08:00",
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

### <a name="response"></a><span data-ttu-id="42a45-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="42a45-178">Response</span></span>
<span data-ttu-id="42a45-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="42a45-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 869

{
  "@odata.type": "#microsoft.graph.managedAllDeviceCertificateState",
  "id": "987c6a17-6a17-987c-176a-7c98176a7c98",
  "certificateRevokeStatus": "pending",
  "certificateRevokeStatusLastChangeDateTime": "2016-12-31T23:59:34.9547208-08:00",
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



