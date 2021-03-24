---
title: Обновление dataSharingConsent
description: Обновление свойств объекта dataSharingConsent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0d617546464b1333af2b535bbc1c17f61fa03386
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146547"
---
# <a name="update-datasharingconsent"></a><span data-ttu-id="7f725-103">Обновление dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="7f725-103">Update dataSharingConsent</span></span>

<span data-ttu-id="7f725-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f725-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7f725-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f725-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f725-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7f725-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f725-107">Обновление свойств объекта [dataSharingConsent.](../resources/intune-devices-datasharingconsent.md)</span><span class="sxs-lookup"><span data-stu-id="7f725-107">Update the properties of a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7f725-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7f725-108">Prerequisites</span></span>
<span data-ttu-id="7f725-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f725-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f725-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7f725-111">Permission type</span></span>|<span data-ttu-id="7f725-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7f725-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f725-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7f725-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7f725-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f725-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7f725-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7f725-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f725-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f725-116">Not supported.</span></span>|
|<span data-ttu-id="7f725-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="7f725-117">Application</span></span>|<span data-ttu-id="7f725-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f725-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f725-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7f725-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/dataSharingConsents/{dataSharingConsentId}
```

## <a name="request-headers"></a><span data-ttu-id="7f725-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7f725-120">Request headers</span></span>
|<span data-ttu-id="7f725-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7f725-121">Header</span></span>|<span data-ttu-id="7f725-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7f725-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f725-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f725-123">Authorization</span></span>|<span data-ttu-id="7f725-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7f725-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f725-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7f725-125">Accept</span></span>|<span data-ttu-id="7f725-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7f725-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f725-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7f725-127">Request body</span></span>
<span data-ttu-id="7f725-128">В теле запроса поставляем представление JSON для [объекта dataSharingConsent.](../resources/intune-devices-datasharingconsent.md)</span><span class="sxs-lookup"><span data-stu-id="7f725-128">In the request body, supply a JSON representation for the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>

<span data-ttu-id="7f725-129">В следующей таблице показаны свойства, необходимые при создании [dataSharingConsent.](../resources/intune-devices-datasharingconsent.md)</span><span class="sxs-lookup"><span data-stu-id="7f725-129">The following table shows the properties that are required when you create the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md).</span></span>

|<span data-ttu-id="7f725-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7f725-130">Property</span></span>|<span data-ttu-id="7f725-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7f725-131">Type</span></span>|<span data-ttu-id="7f725-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7f725-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f725-133">id</span><span class="sxs-lookup"><span data-stu-id="7f725-133">id</span></span>|<span data-ttu-id="7f725-134">Строка</span><span class="sxs-lookup"><span data-stu-id="7f725-134">String</span></span>|<span data-ttu-id="7f725-135">ID согласия для общего доступа к данным</span><span class="sxs-lookup"><span data-stu-id="7f725-135">The data sharing consent Id</span></span>|
|<span data-ttu-id="7f725-136">serviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="7f725-136">serviceDisplayName</span></span>|<span data-ttu-id="7f725-137">Строка</span><span class="sxs-lookup"><span data-stu-id="7f725-137">String</span></span>|<span data-ttu-id="7f725-138">Имя отображения потока работы службы</span><span class="sxs-lookup"><span data-stu-id="7f725-138">The display name of the service work flow</span></span>|
|<span data-ttu-id="7f725-139">termsUrl</span><span class="sxs-lookup"><span data-stu-id="7f725-139">termsUrl</span></span>|<span data-ttu-id="7f725-140">Строка</span><span class="sxs-lookup"><span data-stu-id="7f725-140">String</span></span>|<span data-ttu-id="7f725-141">TermsUrl для согласия на обмен данными</span><span class="sxs-lookup"><span data-stu-id="7f725-141">The TermsUrl for the data sharing consent</span></span>|
|<span data-ttu-id="7f725-142">granted</span><span class="sxs-lookup"><span data-stu-id="7f725-142">granted</span></span>|<span data-ttu-id="7f725-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f725-143">Boolean</span></span>|<span data-ttu-id="7f725-144">Предоставлено состояние для согласия на обмен данными</span><span class="sxs-lookup"><span data-stu-id="7f725-144">The granted state for the data sharing consent</span></span>|
|<span data-ttu-id="7f725-145">grantDateTime</span><span class="sxs-lookup"><span data-stu-id="7f725-145">grantDateTime</span></span>|<span data-ttu-id="7f725-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f725-146">DateTimeOffset</span></span>|<span data-ttu-id="7f725-147">Для этой учетной записи было предоставлено согласие на время</span><span class="sxs-lookup"><span data-stu-id="7f725-147">The time consent was granted for this account</span></span>|
|<span data-ttu-id="7f725-148">grantedByUpn</span><span class="sxs-lookup"><span data-stu-id="7f725-148">grantedByUpn</span></span>|<span data-ttu-id="7f725-149">Строка</span><span class="sxs-lookup"><span data-stu-id="7f725-149">String</span></span>|<span data-ttu-id="7f725-150">Upn пользователя, который предоставил согласие для этой учетной записи</span><span class="sxs-lookup"><span data-stu-id="7f725-150">The Upn of the user that granted consent for this account</span></span>|
|<span data-ttu-id="7f725-151">grantedByUserId</span><span class="sxs-lookup"><span data-stu-id="7f725-151">grantedByUserId</span></span>|<span data-ttu-id="7f725-152">Строка</span><span class="sxs-lookup"><span data-stu-id="7f725-152">String</span></span>|<span data-ttu-id="7f725-153">UserId пользователя, который предоставил согласие для этой учетной записи</span><span class="sxs-lookup"><span data-stu-id="7f725-153">The UserId of the user that granted consent for this account</span></span>|



## <a name="response"></a><span data-ttu-id="7f725-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f725-154">Response</span></span>
<span data-ttu-id="7f725-155">В случае успешной работы этот метод возвращает код ответа и обновленный `200 OK` [объект dataSharingConsent](../resources/intune-devices-datasharingconsent.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7f725-155">If successful, this method returns a `200 OK` response code and an updated [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f725-156">Пример</span><span class="sxs-lookup"><span data-stu-id="7f725-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="7f725-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f725-157">Request</span></span>
<span data-ttu-id="7f725-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7f725-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/dataSharingConsents/{dataSharingConsentId}
Content-type: application/json
Content-length: 333

{
  "@odata.type": "#microsoft.graph.dataSharingConsent",
  "serviceDisplayName": "Service Display Name value",
  "termsUrl": "https://example.com/termsUrl/",
  "granted": true,
  "grantDateTime": "2016-12-31T23:59:55.7154191-08:00",
  "grantedByUpn": "Granted By Upn value",
  "grantedByUserId": "Granted By User Id value"
}
```

### <a name="response"></a><span data-ttu-id="7f725-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f725-159">Response</span></span>
<span data-ttu-id="7f725-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7f725-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 382

{
  "@odata.type": "#microsoft.graph.dataSharingConsent",
  "id": "333387f7-87f7-3333-f787-3333f7873333",
  "serviceDisplayName": "Service Display Name value",
  "termsUrl": "https://example.com/termsUrl/",
  "granted": true,
  "grantDateTime": "2016-12-31T23:59:55.7154191-08:00",
  "grantedByUpn": "Granted By Upn value",
  "grantedByUserId": "Granted By User Id value"
}
```




