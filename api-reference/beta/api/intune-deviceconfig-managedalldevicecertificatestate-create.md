---
title: Создание Манажедаллдевицецертификатестате
description: Создание нового объекта Манажедаллдевицецертификатестате.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 58f061bd89c3633651e40578e23db1f1f4836406
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792739"
---
# <a name="create-managedalldevicecertificatestate"></a><span data-ttu-id="157ee-103">Создание Манажедаллдевицецертификатестате</span><span class="sxs-lookup"><span data-stu-id="157ee-103">Create managedAllDeviceCertificateState</span></span>

<span data-ttu-id="157ee-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="157ee-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="157ee-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="157ee-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="157ee-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="157ee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="157ee-107">Создание нового объекта [манажедаллдевицецертификатестате](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="157ee-107">Create a new [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="157ee-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="157ee-108">Prerequisites</span></span>
<span data-ttu-id="157ee-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="157ee-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="157ee-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="157ee-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="157ee-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="157ee-111">Permission type</span></span>|<span data-ttu-id="157ee-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="157ee-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="157ee-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="157ee-113">Delegated (work or school account)</span></span>|<span data-ttu-id="157ee-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="157ee-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="157ee-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="157ee-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="157ee-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="157ee-116">Not supported.</span></span>|
|<span data-ttu-id="157ee-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="157ee-117">Application</span></span>|<span data-ttu-id="157ee-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="157ee-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="157ee-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="157ee-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates
```

## <a name="request-headers"></a><span data-ttu-id="157ee-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="157ee-120">Request headers</span></span>
|<span data-ttu-id="157ee-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="157ee-121">Header</span></span>|<span data-ttu-id="157ee-122">Значение</span><span class="sxs-lookup"><span data-stu-id="157ee-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="157ee-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="157ee-123">Authorization</span></span>|<span data-ttu-id="157ee-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="157ee-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="157ee-125">Accept</span><span class="sxs-lookup"><span data-stu-id="157ee-125">Accept</span></span>|<span data-ttu-id="157ee-126">application/json</span><span class="sxs-lookup"><span data-stu-id="157ee-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="157ee-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="157ee-127">Request body</span></span>
<span data-ttu-id="157ee-128">В тексте запроса добавьте представление объекта Манажедаллдевицецертификатестате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="157ee-128">In the request body, supply a JSON representation for the managedAllDeviceCertificateState object.</span></span>

<span data-ttu-id="157ee-129">В следующей таблице приведены свойства, необходимые при создании Манажедаллдевицецертификатестате.</span><span class="sxs-lookup"><span data-stu-id="157ee-129">The following table shows the properties that are required when you create the managedAllDeviceCertificateState.</span></span>

|<span data-ttu-id="157ee-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="157ee-130">Property</span></span>|<span data-ttu-id="157ee-131">Тип</span><span class="sxs-lookup"><span data-stu-id="157ee-131">Type</span></span>|<span data-ttu-id="157ee-132">Описание</span><span class="sxs-lookup"><span data-stu-id="157ee-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="157ee-133">id</span><span class="sxs-lookup"><span data-stu-id="157ee-133">id</span></span>|<span data-ttu-id="157ee-134">Строка</span><span class="sxs-lookup"><span data-stu-id="157ee-134">String</span></span>|<span data-ttu-id="157ee-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="157ee-135">Key of the entity.</span></span>|
|<span data-ttu-id="157ee-136">цертификатеревокестатус</span><span class="sxs-lookup"><span data-stu-id="157ee-136">certificateRevokeStatus</span></span>|[<span data-ttu-id="157ee-137">цертификатеревокатионстатус</span><span class="sxs-lookup"><span data-stu-id="157ee-137">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="157ee-138">Отзыв состояния.</span><span class="sxs-lookup"><span data-stu-id="157ee-138">Revoke status.</span></span> <span data-ttu-id="157ee-139">Возможные значения: `none`, `pending`, `issued`, `failed`, `revoked`.</span><span class="sxs-lookup"><span data-stu-id="157ee-139">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="157ee-140">манажеддевицедисплайнаме</span><span class="sxs-lookup"><span data-stu-id="157ee-140">managedDeviceDisplayName</span></span>|<span data-ttu-id="157ee-141">String</span><span class="sxs-lookup"><span data-stu-id="157ee-141">String</span></span>|<span data-ttu-id="157ee-142">Отображаемое имя устройства</span><span class="sxs-lookup"><span data-stu-id="157ee-142">Device display name</span></span>|
|<span data-ttu-id="157ee-143">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="157ee-143">userPrincipalName</span></span>|<span data-ttu-id="157ee-144">String</span><span class="sxs-lookup"><span data-stu-id="157ee-144">String</span></span>|<span data-ttu-id="157ee-145">Имя субъекта-пользователя</span><span class="sxs-lookup"><span data-stu-id="157ee-145">User principal name</span></span>|
|<span data-ttu-id="157ee-146">цертификатикспиратиондатетиме</span><span class="sxs-lookup"><span data-stu-id="157ee-146">certificateExpirationDateTime</span></span>|<span data-ttu-id="157ee-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="157ee-147">DateTimeOffset</span></span>|<span data-ttu-id="157ee-148">Дата окончания срока действия сертификата</span><span class="sxs-lookup"><span data-stu-id="157ee-148">Certificate expiry date</span></span>|
|<span data-ttu-id="157ee-149">цертификатеиссуернаме</span><span class="sxs-lookup"><span data-stu-id="157ee-149">certificateIssuerName</span></span>|<span data-ttu-id="157ee-150">String</span><span class="sxs-lookup"><span data-stu-id="157ee-150">String</span></span>|<span data-ttu-id="157ee-151">Издатель</span><span class="sxs-lookup"><span data-stu-id="157ee-151">Issuer</span></span>|
|<span data-ttu-id="157ee-152">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="157ee-152">certificateThumbprint</span></span>|<span data-ttu-id="157ee-153">String</span><span class="sxs-lookup"><span data-stu-id="157ee-153">String</span></span>|<span data-ttu-id="157ee-154">Отпечаток</span><span class="sxs-lookup"><span data-stu-id="157ee-154">Thumbprint</span></span>|
|<span data-ttu-id="157ee-155">цертификатесериалнумбер</span><span class="sxs-lookup"><span data-stu-id="157ee-155">certificateSerialNumber</span></span>|<span data-ttu-id="157ee-156">String</span><span class="sxs-lookup"><span data-stu-id="157ee-156">String</span></span>|<span data-ttu-id="157ee-157">Серийный номер</span><span class="sxs-lookup"><span data-stu-id="157ee-157">Serial number</span></span>|
|<span data-ttu-id="157ee-158">цертификатесубжектнаме</span><span class="sxs-lookup"><span data-stu-id="157ee-158">certificateSubjectName</span></span>|<span data-ttu-id="157ee-159">String</span><span class="sxs-lookup"><span data-stu-id="157ee-159">String</span></span>|<span data-ttu-id="157ee-160">Имя субъекта сертификата</span><span class="sxs-lookup"><span data-stu-id="157ee-160">Certificate subject name</span></span>|
|<span data-ttu-id="157ee-161">цертификатекэйусажес</span><span class="sxs-lookup"><span data-stu-id="157ee-161">certificateKeyUsages</span></span>|<span data-ttu-id="157ee-162">Int32</span><span class="sxs-lookup"><span data-stu-id="157ee-162">Int32</span></span>|<span data-ttu-id="157ee-163">Использование ключа</span><span class="sxs-lookup"><span data-stu-id="157ee-163">Key Usage</span></span>|
|<span data-ttu-id="157ee-164">цертификатикстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="157ee-164">certificateExtendedKeyUsages</span></span>|<span data-ttu-id="157ee-165">String</span><span class="sxs-lookup"><span data-stu-id="157ee-165">String</span></span>|<span data-ttu-id="157ee-166">Расширенное использование ключа</span><span class="sxs-lookup"><span data-stu-id="157ee-166">Enhanced Key Usage</span></span>|
|<span data-ttu-id="157ee-167">цертификатеиссуанцедатетиме</span><span class="sxs-lookup"><span data-stu-id="157ee-167">certificateIssuanceDateTime</span></span>|<span data-ttu-id="157ee-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="157ee-168">DateTimeOffset</span></span>|<span data-ttu-id="157ee-169">Дата выпуска</span><span class="sxs-lookup"><span data-stu-id="157ee-169">Issuance date</span></span>|
|<span data-ttu-id="157ee-170">цертификатеревокестатусластчанжедатетиме</span><span class="sxs-lookup"><span data-stu-id="157ee-170">certificateRevokeStatusLastChangeDateTime</span></span>|<span data-ttu-id="157ee-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="157ee-171">DateTimeOffset</span></span>|<span data-ttu-id="157ee-172">Время последнего изменения состояния отзыва</span><span class="sxs-lookup"><span data-stu-id="157ee-172">The time the revoke status was last changed</span></span>|



## <a name="response"></a><span data-ttu-id="157ee-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="157ee-173">Response</span></span>
<span data-ttu-id="157ee-174">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [манажедаллдевицецертификатестате](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="157ee-174">If successful, this method returns a `201 Created` response code and a [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="157ee-175">Пример</span><span class="sxs-lookup"><span data-stu-id="157ee-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="157ee-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="157ee-176">Request</span></span>
<span data-ttu-id="157ee-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="157ee-177">Here is an example of the request.</span></span>
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
  "certificateIssuanceDateTime": "2016-12-31T23:59:41.5044473-08:00",
  "certificateRevokeStatusLastChangeDateTime": "2016-12-31T23:59:41.5044473-08:00"
}
```

### <a name="response"></a><span data-ttu-id="157ee-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="157ee-178">Response</span></span>
<span data-ttu-id="157ee-179">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="157ee-179">Here is an example of the response.</span></span> <span data-ttu-id="157ee-180">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="157ee-180">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="157ee-181">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="157ee-181">All of the properties will be returned from an actual call.</span></span>
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
  "certificateIssuanceDateTime": "2016-12-31T23:59:41.5044473-08:00",
  "certificateRevokeStatusLastChangeDateTime": "2016-12-31T23:59:41.5044473-08:00"
}
```



