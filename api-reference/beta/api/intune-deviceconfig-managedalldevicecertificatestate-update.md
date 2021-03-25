---
title: Обновление managedAllDeviceCertificateState
description: Обновление свойств объекта managedAllDeviceCertificateState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: feb45298263ee3fe4a3d02ec03f729dd7d2d382f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51155143"
---
# <a name="update-managedalldevicecertificatestate"></a><span data-ttu-id="5ebdb-103">Обновление managedAllDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="5ebdb-103">Update managedAllDeviceCertificateState</span></span>

<span data-ttu-id="5ebdb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ebdb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5ebdb-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ebdb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5ebdb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5ebdb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ebdb-107">Обновление свойств объекта [managedAllDeviceCertificateState.](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)</span><span class="sxs-lookup"><span data-stu-id="5ebdb-107">Update the properties of a [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5ebdb-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5ebdb-108">Prerequisites</span></span>
<span data-ttu-id="5ebdb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ebdb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ebdb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5ebdb-111">Permission type</span></span>|<span data-ttu-id="5ebdb-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5ebdb-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ebdb-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5ebdb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5ebdb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ebdb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5ebdb-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5ebdb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ebdb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ebdb-116">Not supported.</span></span>|
|<span data-ttu-id="5ebdb-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="5ebdb-117">Application</span></span>|<span data-ttu-id="5ebdb-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ebdb-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ebdb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5ebdb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates/{managedAllDeviceCertificateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="5ebdb-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5ebdb-120">Request headers</span></span>
|<span data-ttu-id="5ebdb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5ebdb-121">Header</span></span>|<span data-ttu-id="5ebdb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5ebdb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ebdb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ebdb-123">Authorization</span></span>|<span data-ttu-id="5ebdb-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5ebdb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5ebdb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5ebdb-125">Accept</span></span>|<span data-ttu-id="5ebdb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5ebdb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ebdb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5ebdb-127">Request body</span></span>
<span data-ttu-id="5ebdb-128">В теле запроса поставляем представление JSON для [объекта managedAllDeviceCertificateState.](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)</span><span class="sxs-lookup"><span data-stu-id="5ebdb-128">In the request body, supply a JSON representation for the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

<span data-ttu-id="5ebdb-129">В следующей таблице показаны свойства, необходимые при создании [управляемогоAllDeviceCertificateState.](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)</span><span class="sxs-lookup"><span data-stu-id="5ebdb-129">The following table shows the properties that are required when you create the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md).</span></span>

|<span data-ttu-id="5ebdb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5ebdb-130">Property</span></span>|<span data-ttu-id="5ebdb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5ebdb-131">Type</span></span>|<span data-ttu-id="5ebdb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5ebdb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ebdb-133">id</span><span class="sxs-lookup"><span data-stu-id="5ebdb-133">id</span></span>|<span data-ttu-id="5ebdb-134">Строка</span><span class="sxs-lookup"><span data-stu-id="5ebdb-134">String</span></span>|<span data-ttu-id="5ebdb-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5ebdb-135">Key of the entity.</span></span>|
|<span data-ttu-id="5ebdb-136">certificateRevokeStatus</span><span class="sxs-lookup"><span data-stu-id="5ebdb-136">certificateRevokeStatus</span></span>|[<span data-ttu-id="5ebdb-137">certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="5ebdb-137">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="5ebdb-138">Отзови статус.</span><span class="sxs-lookup"><span data-stu-id="5ebdb-138">Revoke status.</span></span> <span data-ttu-id="5ebdb-139">Возможные значения: `none`, `pending`, `issued`, `failed`, `revoked`.</span><span class="sxs-lookup"><span data-stu-id="5ebdb-139">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="5ebdb-140">certificateRevokeStatusLastChangeDateTime</span><span class="sxs-lookup"><span data-stu-id="5ebdb-140">certificateRevokeStatusLastChangeDateTime</span></span>|<span data-ttu-id="5ebdb-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ebdb-141">DateTimeOffset</span></span>|<span data-ttu-id="5ebdb-142">Время последнего изменения состояния отвода</span><span class="sxs-lookup"><span data-stu-id="5ebdb-142">The time the revoke status was last changed</span></span>|
|<span data-ttu-id="5ebdb-143">managedDeviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="5ebdb-143">managedDeviceDisplayName</span></span>|<span data-ttu-id="5ebdb-144">Строка</span><span class="sxs-lookup"><span data-stu-id="5ebdb-144">String</span></span>|<span data-ttu-id="5ebdb-145">Имя отображения устройства</span><span class="sxs-lookup"><span data-stu-id="5ebdb-145">Device display name</span></span>|
|<span data-ttu-id="5ebdb-146">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5ebdb-146">userPrincipalName</span></span>|<span data-ttu-id="5ebdb-147">String</span><span class="sxs-lookup"><span data-stu-id="5ebdb-147">String</span></span>|<span data-ttu-id="5ebdb-148">Имя субъекта-пользователя</span><span class="sxs-lookup"><span data-stu-id="5ebdb-148">User principal name</span></span>|
|<span data-ttu-id="5ebdb-149">certificateExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="5ebdb-149">certificateExpirationDateTime</span></span>|<span data-ttu-id="5ebdb-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ebdb-150">DateTimeOffset</span></span>|<span data-ttu-id="5ebdb-151">Дата истечения срока действия сертификата</span><span class="sxs-lookup"><span data-stu-id="5ebdb-151">Certificate expiry date</span></span>|
|<span data-ttu-id="5ebdb-152">certificateIssuerName</span><span class="sxs-lookup"><span data-stu-id="5ebdb-152">certificateIssuerName</span></span>|<span data-ttu-id="5ebdb-153">Строка</span><span class="sxs-lookup"><span data-stu-id="5ebdb-153">String</span></span>|<span data-ttu-id="5ebdb-154">Издатель</span><span class="sxs-lookup"><span data-stu-id="5ebdb-154">Issuer</span></span>|
|<span data-ttu-id="5ebdb-155">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="5ebdb-155">certificateThumbprint</span></span>|<span data-ttu-id="5ebdb-156">Строка</span><span class="sxs-lookup"><span data-stu-id="5ebdb-156">String</span></span>|<span data-ttu-id="5ebdb-157">Thumbprint</span><span class="sxs-lookup"><span data-stu-id="5ebdb-157">Thumbprint</span></span>|
|<span data-ttu-id="5ebdb-158">certificateSerialNumber</span><span class="sxs-lookup"><span data-stu-id="5ebdb-158">certificateSerialNumber</span></span>|<span data-ttu-id="5ebdb-159">Строка</span><span class="sxs-lookup"><span data-stu-id="5ebdb-159">String</span></span>|<span data-ttu-id="5ebdb-160">Серийный номер</span><span class="sxs-lookup"><span data-stu-id="5ebdb-160">Serial number</span></span>|
|<span data-ttu-id="5ebdb-161">certificateSubjectName</span><span class="sxs-lookup"><span data-stu-id="5ebdb-161">certificateSubjectName</span></span>|<span data-ttu-id="5ebdb-162">Строка</span><span class="sxs-lookup"><span data-stu-id="5ebdb-162">String</span></span>|<span data-ttu-id="5ebdb-163">Имя субъекта сертификата</span><span class="sxs-lookup"><span data-stu-id="5ebdb-163">Certificate subject name</span></span>|
|<span data-ttu-id="5ebdb-164">certificateKeyUsages</span><span class="sxs-lookup"><span data-stu-id="5ebdb-164">certificateKeyUsages</span></span>|<span data-ttu-id="5ebdb-165">Int32</span><span class="sxs-lookup"><span data-stu-id="5ebdb-165">Int32</span></span>|<span data-ttu-id="5ebdb-166">Использование ключей</span><span class="sxs-lookup"><span data-stu-id="5ebdb-166">Key Usage</span></span>|
|<span data-ttu-id="5ebdb-167">certificateExtendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="5ebdb-167">certificateExtendedKeyUsages</span></span>|<span data-ttu-id="5ebdb-168">Строка</span><span class="sxs-lookup"><span data-stu-id="5ebdb-168">String</span></span>|<span data-ttu-id="5ebdb-169">Расширенное использование ключей</span><span class="sxs-lookup"><span data-stu-id="5ebdb-169">Enhanced Key Usage</span></span>|
|<span data-ttu-id="5ebdb-170">certificateIssuanceDateTime</span><span class="sxs-lookup"><span data-stu-id="5ebdb-170">certificateIssuanceDateTime</span></span>|<span data-ttu-id="5ebdb-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ebdb-171">DateTimeOffset</span></span>|<span data-ttu-id="5ebdb-172">Дата выпуска</span><span class="sxs-lookup"><span data-stu-id="5ebdb-172">Issuance date</span></span>|



## <a name="response"></a><span data-ttu-id="5ebdb-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ebdb-173">Response</span></span>
<span data-ttu-id="5ebdb-174">В случае успешной работы этот метод возвращает код ответа и обновленный `200 OK` [объект managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="5ebdb-174">If successful, this method returns a `200 OK` response code and an updated [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ebdb-175">Пример</span><span class="sxs-lookup"><span data-stu-id="5ebdb-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="5ebdb-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="5ebdb-176">Request</span></span>
<span data-ttu-id="5ebdb-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5ebdb-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates/{managedAllDeviceCertificateStateId}
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

### <a name="response"></a><span data-ttu-id="5ebdb-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ebdb-178">Response</span></span>
<span data-ttu-id="5ebdb-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5ebdb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




