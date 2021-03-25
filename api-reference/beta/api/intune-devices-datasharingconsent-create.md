---
title: Создание dataSharingConsent
description: Создание нового объекта dataSharingConsent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 87e9044fc48f857aa64c75f7a9b5579d8ae7573a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154429"
---
# <a name="create-datasharingconsent"></a><span data-ttu-id="483e6-103">Создание dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="483e6-103">Create dataSharingConsent</span></span>

<span data-ttu-id="483e6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="483e6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="483e6-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="483e6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="483e6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="483e6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="483e6-107">Создание нового [объекта dataSharingConsent.](../resources/intune-devices-datasharingconsent.md)</span><span class="sxs-lookup"><span data-stu-id="483e6-107">Create a new [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="483e6-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="483e6-108">Prerequisites</span></span>
<span data-ttu-id="483e6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="483e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="483e6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="483e6-111">Permission type</span></span>|<span data-ttu-id="483e6-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="483e6-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="483e6-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="483e6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="483e6-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="483e6-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="483e6-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="483e6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="483e6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="483e6-116">Not supported.</span></span>|
|<span data-ttu-id="483e6-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="483e6-117">Application</span></span>|<span data-ttu-id="483e6-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="483e6-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="483e6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="483e6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/dataSharingConsents
```

## <a name="request-headers"></a><span data-ttu-id="483e6-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="483e6-120">Request headers</span></span>
|<span data-ttu-id="483e6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="483e6-121">Header</span></span>|<span data-ttu-id="483e6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="483e6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="483e6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="483e6-123">Authorization</span></span>|<span data-ttu-id="483e6-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="483e6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="483e6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="483e6-125">Accept</span></span>|<span data-ttu-id="483e6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="483e6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="483e6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="483e6-127">Request body</span></span>
<span data-ttu-id="483e6-128">В теле запроса поставляем представление JSON для объекта dataSharingConsent.</span><span class="sxs-lookup"><span data-stu-id="483e6-128">In the request body, supply a JSON representation for the dataSharingConsent object.</span></span>

<span data-ttu-id="483e6-129">В следующей таблице показаны свойства, необходимые при создании dataSharingConsent.</span><span class="sxs-lookup"><span data-stu-id="483e6-129">The following table shows the properties that are required when you create the dataSharingConsent.</span></span>

|<span data-ttu-id="483e6-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="483e6-130">Property</span></span>|<span data-ttu-id="483e6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="483e6-131">Type</span></span>|<span data-ttu-id="483e6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="483e6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="483e6-133">id</span><span class="sxs-lookup"><span data-stu-id="483e6-133">id</span></span>|<span data-ttu-id="483e6-134">Строка</span><span class="sxs-lookup"><span data-stu-id="483e6-134">String</span></span>|<span data-ttu-id="483e6-135">ID согласия для общего доступа к данным</span><span class="sxs-lookup"><span data-stu-id="483e6-135">The data sharing consent Id</span></span>|
|<span data-ttu-id="483e6-136">serviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="483e6-136">serviceDisplayName</span></span>|<span data-ttu-id="483e6-137">Строка</span><span class="sxs-lookup"><span data-stu-id="483e6-137">String</span></span>|<span data-ttu-id="483e6-138">Имя отображения потока работы службы</span><span class="sxs-lookup"><span data-stu-id="483e6-138">The display name of the service work flow</span></span>|
|<span data-ttu-id="483e6-139">termsUrl</span><span class="sxs-lookup"><span data-stu-id="483e6-139">termsUrl</span></span>|<span data-ttu-id="483e6-140">Строка</span><span class="sxs-lookup"><span data-stu-id="483e6-140">String</span></span>|<span data-ttu-id="483e6-141">TermsUrl для согласия на обмен данными</span><span class="sxs-lookup"><span data-stu-id="483e6-141">The TermsUrl for the data sharing consent</span></span>|
|<span data-ttu-id="483e6-142">granted</span><span class="sxs-lookup"><span data-stu-id="483e6-142">granted</span></span>|<span data-ttu-id="483e6-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="483e6-143">Boolean</span></span>|<span data-ttu-id="483e6-144">Предоставлено состояние для согласия на обмен данными</span><span class="sxs-lookup"><span data-stu-id="483e6-144">The granted state for the data sharing consent</span></span>|
|<span data-ttu-id="483e6-145">grantDateTime</span><span class="sxs-lookup"><span data-stu-id="483e6-145">grantDateTime</span></span>|<span data-ttu-id="483e6-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="483e6-146">DateTimeOffset</span></span>|<span data-ttu-id="483e6-147">Для этой учетной записи было предоставлено согласие на время</span><span class="sxs-lookup"><span data-stu-id="483e6-147">The time consent was granted for this account</span></span>|
|<span data-ttu-id="483e6-148">grantedByUpn</span><span class="sxs-lookup"><span data-stu-id="483e6-148">grantedByUpn</span></span>|<span data-ttu-id="483e6-149">Строка</span><span class="sxs-lookup"><span data-stu-id="483e6-149">String</span></span>|<span data-ttu-id="483e6-150">Upn пользователя, который предоставил согласие для этой учетной записи</span><span class="sxs-lookup"><span data-stu-id="483e6-150">The Upn of the user that granted consent for this account</span></span>|
|<span data-ttu-id="483e6-151">grantedByUserId</span><span class="sxs-lookup"><span data-stu-id="483e6-151">grantedByUserId</span></span>|<span data-ttu-id="483e6-152">Строка</span><span class="sxs-lookup"><span data-stu-id="483e6-152">String</span></span>|<span data-ttu-id="483e6-153">UserId пользователя, который предоставил согласие для этой учетной записи</span><span class="sxs-lookup"><span data-stu-id="483e6-153">The UserId of the user that granted consent for this account</span></span>|



## <a name="response"></a><span data-ttu-id="483e6-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="483e6-154">Response</span></span>
<span data-ttu-id="483e6-155">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект dataSharingConsent](../resources/intune-devices-datasharingconsent.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="483e6-155">If successful, this method returns a `201 Created` response code and a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="483e6-156">Пример</span><span class="sxs-lookup"><span data-stu-id="483e6-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="483e6-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="483e6-157">Request</span></span>
<span data-ttu-id="483e6-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="483e6-158">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/dataSharingConsents
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

### <a name="response"></a><span data-ttu-id="483e6-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="483e6-159">Response</span></span>
<span data-ttu-id="483e6-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="483e6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




