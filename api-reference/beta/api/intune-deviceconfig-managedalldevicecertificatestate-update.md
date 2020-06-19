---
title: Обновление Манажедаллдевицецертификатестате
description: Обновление свойств объекта Манажедаллдевицецертификатестате.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5a54626104faa00e443efe1d430fbd53eb9784dd
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792718"
---
# <a name="update-managedalldevicecertificatestate"></a><span data-ttu-id="65e33-103">Обновление Манажедаллдевицецертификатестате</span><span class="sxs-lookup"><span data-stu-id="65e33-103">Update managedAllDeviceCertificateState</span></span>

<span data-ttu-id="65e33-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65e33-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="65e33-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65e33-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65e33-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="65e33-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65e33-107">Обновление свойств объекта [манажедаллдевицецертификатестате](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="65e33-107">Update the properties of a [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="65e33-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="65e33-108">Prerequisites</span></span>
<span data-ttu-id="65e33-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="65e33-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="65e33-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65e33-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65e33-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="65e33-111">Permission type</span></span>|<span data-ttu-id="65e33-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="65e33-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65e33-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="65e33-113">Delegated (work or school account)</span></span>|<span data-ttu-id="65e33-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65e33-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="65e33-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="65e33-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65e33-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65e33-116">Not supported.</span></span>|
|<span data-ttu-id="65e33-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="65e33-117">Application</span></span>|<span data-ttu-id="65e33-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65e33-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="65e33-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="65e33-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates/{managedAllDeviceCertificateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="65e33-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="65e33-120">Request headers</span></span>
|<span data-ttu-id="65e33-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="65e33-121">Header</span></span>|<span data-ttu-id="65e33-122">Значение</span><span class="sxs-lookup"><span data-stu-id="65e33-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65e33-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="65e33-123">Authorization</span></span>|<span data-ttu-id="65e33-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="65e33-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65e33-125">Accept</span><span class="sxs-lookup"><span data-stu-id="65e33-125">Accept</span></span>|<span data-ttu-id="65e33-126">application/json</span><span class="sxs-lookup"><span data-stu-id="65e33-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65e33-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="65e33-127">Request body</span></span>
<span data-ttu-id="65e33-128">В тексте запроса добавьте представление объекта [манажедаллдевицецертификатестате](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="65e33-128">In the request body, supply a JSON representation for the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

<span data-ttu-id="65e33-129">В следующей таблице приведены свойства, необходимые при создании [манажедаллдевицецертификатестате](../resources/intune-deviceconfig-managedalldevicecertificatestate.md).</span><span class="sxs-lookup"><span data-stu-id="65e33-129">The following table shows the properties that are required when you create the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md).</span></span>

|<span data-ttu-id="65e33-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="65e33-130">Property</span></span>|<span data-ttu-id="65e33-131">Тип</span><span class="sxs-lookup"><span data-stu-id="65e33-131">Type</span></span>|<span data-ttu-id="65e33-132">Описание</span><span class="sxs-lookup"><span data-stu-id="65e33-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65e33-133">id</span><span class="sxs-lookup"><span data-stu-id="65e33-133">id</span></span>|<span data-ttu-id="65e33-134">Строка</span><span class="sxs-lookup"><span data-stu-id="65e33-134">String</span></span>|<span data-ttu-id="65e33-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="65e33-135">Key of the entity.</span></span>|
|<span data-ttu-id="65e33-136">цертификатеревокестатус</span><span class="sxs-lookup"><span data-stu-id="65e33-136">certificateRevokeStatus</span></span>|[<span data-ttu-id="65e33-137">цертификатеревокатионстатус</span><span class="sxs-lookup"><span data-stu-id="65e33-137">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="65e33-138">Отзыв состояния.</span><span class="sxs-lookup"><span data-stu-id="65e33-138">Revoke status.</span></span> <span data-ttu-id="65e33-139">Возможные значения: `none`, `pending`, `issued`, `failed`, `revoked`.</span><span class="sxs-lookup"><span data-stu-id="65e33-139">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="65e33-140">манажеддевицедисплайнаме</span><span class="sxs-lookup"><span data-stu-id="65e33-140">managedDeviceDisplayName</span></span>|<span data-ttu-id="65e33-141">String</span><span class="sxs-lookup"><span data-stu-id="65e33-141">String</span></span>|<span data-ttu-id="65e33-142">Отображаемое имя устройства</span><span class="sxs-lookup"><span data-stu-id="65e33-142">Device display name</span></span>|
|<span data-ttu-id="65e33-143">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="65e33-143">userPrincipalName</span></span>|<span data-ttu-id="65e33-144">String</span><span class="sxs-lookup"><span data-stu-id="65e33-144">String</span></span>|<span data-ttu-id="65e33-145">Имя субъекта-пользователя</span><span class="sxs-lookup"><span data-stu-id="65e33-145">User principal name</span></span>|
|<span data-ttu-id="65e33-146">цертификатикспиратиондатетиме</span><span class="sxs-lookup"><span data-stu-id="65e33-146">certificateExpirationDateTime</span></span>|<span data-ttu-id="65e33-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65e33-147">DateTimeOffset</span></span>|<span data-ttu-id="65e33-148">Дата окончания срока действия сертификата</span><span class="sxs-lookup"><span data-stu-id="65e33-148">Certificate expiry date</span></span>|
|<span data-ttu-id="65e33-149">цертификатеиссуернаме</span><span class="sxs-lookup"><span data-stu-id="65e33-149">certificateIssuerName</span></span>|<span data-ttu-id="65e33-150">String</span><span class="sxs-lookup"><span data-stu-id="65e33-150">String</span></span>|<span data-ttu-id="65e33-151">Издатель</span><span class="sxs-lookup"><span data-stu-id="65e33-151">Issuer</span></span>|
|<span data-ttu-id="65e33-152">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="65e33-152">certificateThumbprint</span></span>|<span data-ttu-id="65e33-153">String</span><span class="sxs-lookup"><span data-stu-id="65e33-153">String</span></span>|<span data-ttu-id="65e33-154">Отпечаток</span><span class="sxs-lookup"><span data-stu-id="65e33-154">Thumbprint</span></span>|
|<span data-ttu-id="65e33-155">цертификатесериалнумбер</span><span class="sxs-lookup"><span data-stu-id="65e33-155">certificateSerialNumber</span></span>|<span data-ttu-id="65e33-156">String</span><span class="sxs-lookup"><span data-stu-id="65e33-156">String</span></span>|<span data-ttu-id="65e33-157">Серийный номер</span><span class="sxs-lookup"><span data-stu-id="65e33-157">Serial number</span></span>|
|<span data-ttu-id="65e33-158">цертификатесубжектнаме</span><span class="sxs-lookup"><span data-stu-id="65e33-158">certificateSubjectName</span></span>|<span data-ttu-id="65e33-159">String</span><span class="sxs-lookup"><span data-stu-id="65e33-159">String</span></span>|<span data-ttu-id="65e33-160">Имя субъекта сертификата</span><span class="sxs-lookup"><span data-stu-id="65e33-160">Certificate subject name</span></span>|
|<span data-ttu-id="65e33-161">цертификатекэйусажес</span><span class="sxs-lookup"><span data-stu-id="65e33-161">certificateKeyUsages</span></span>|<span data-ttu-id="65e33-162">Int32</span><span class="sxs-lookup"><span data-stu-id="65e33-162">Int32</span></span>|<span data-ttu-id="65e33-163">Использование ключа</span><span class="sxs-lookup"><span data-stu-id="65e33-163">Key Usage</span></span>|
|<span data-ttu-id="65e33-164">цертификатикстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="65e33-164">certificateExtendedKeyUsages</span></span>|<span data-ttu-id="65e33-165">String</span><span class="sxs-lookup"><span data-stu-id="65e33-165">String</span></span>|<span data-ttu-id="65e33-166">Расширенное использование ключа</span><span class="sxs-lookup"><span data-stu-id="65e33-166">Enhanced Key Usage</span></span>|
|<span data-ttu-id="65e33-167">цертификатеиссуанцедатетиме</span><span class="sxs-lookup"><span data-stu-id="65e33-167">certificateIssuanceDateTime</span></span>|<span data-ttu-id="65e33-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65e33-168">DateTimeOffset</span></span>|<span data-ttu-id="65e33-169">Дата выпуска</span><span class="sxs-lookup"><span data-stu-id="65e33-169">Issuance date</span></span>|
|<span data-ttu-id="65e33-170">цертификатеревокестатусластчанжедатетиме</span><span class="sxs-lookup"><span data-stu-id="65e33-170">certificateRevokeStatusLastChangeDateTime</span></span>|<span data-ttu-id="65e33-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65e33-171">DateTimeOffset</span></span>|<span data-ttu-id="65e33-172">Время последнего изменения состояния отзыва</span><span class="sxs-lookup"><span data-stu-id="65e33-172">The time the revoke status was last changed</span></span>|



## <a name="response"></a><span data-ttu-id="65e33-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="65e33-173">Response</span></span>
<span data-ttu-id="65e33-174">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [манажедаллдевицецертификатестате](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="65e33-174">If successful, this method returns a `200 OK` response code and an updated [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65e33-175">Пример</span><span class="sxs-lookup"><span data-stu-id="65e33-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="65e33-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="65e33-176">Request</span></span>
<span data-ttu-id="65e33-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="65e33-177">Here is an example of the request.</span></span>
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
  "certificateIssuanceDateTime": "2016-12-31T23:59:41.5044473-08:00",
  "certificateRevokeStatusLastChangeDateTime": "2016-12-31T23:59:41.5044473-08:00"
}
```

### <a name="response"></a><span data-ttu-id="65e33-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="65e33-178">Response</span></span>
<span data-ttu-id="65e33-179">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="65e33-179">Here is an example of the response.</span></span> <span data-ttu-id="65e33-180">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="65e33-180">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="65e33-181">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="65e33-181">All of the properties will be returned from an actual call.</span></span>
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
  "certificateIssuanceDateTime": "2016-12-31T23:59:41.5044473-08:00",
  "certificateRevokeStatusLastChangeDateTime": "2016-12-31T23:59:41.5044473-08:00"
}
```



