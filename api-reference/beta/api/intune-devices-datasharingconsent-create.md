---
title: Создание Даташарингконсент
description: Создание нового объекта Даташарингконсент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4025245177cd4800ee707629940f1c4b4676d73f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42469932"
---
# <a name="create-datasharingconsent"></a><span data-ttu-id="36e40-103">Создание Даташарингконсент</span><span class="sxs-lookup"><span data-stu-id="36e40-103">Create dataSharingConsent</span></span>

<span data-ttu-id="36e40-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="36e40-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="36e40-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36e40-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="36e40-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="36e40-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36e40-107">Создание нового объекта [даташарингконсент](../resources/intune-devices-datasharingconsent.md) .</span><span class="sxs-lookup"><span data-stu-id="36e40-107">Create a new [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="36e40-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="36e40-108">Prerequisites</span></span>
<span data-ttu-id="36e40-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36e40-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36e40-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="36e40-111">Permission type</span></span>|<span data-ttu-id="36e40-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="36e40-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36e40-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="36e40-113">Delegated (work or school account)</span></span>|<span data-ttu-id="36e40-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36e40-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="36e40-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="36e40-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36e40-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36e40-116">Not supported.</span></span>|
|<span data-ttu-id="36e40-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="36e40-117">Application</span></span>|<span data-ttu-id="36e40-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36e40-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="36e40-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="36e40-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/dataSharingConsents
```

## <a name="request-headers"></a><span data-ttu-id="36e40-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="36e40-120">Request headers</span></span>
|<span data-ttu-id="36e40-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="36e40-121">Header</span></span>|<span data-ttu-id="36e40-122">Значение</span><span class="sxs-lookup"><span data-stu-id="36e40-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36e40-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="36e40-123">Authorization</span></span>|<span data-ttu-id="36e40-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="36e40-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36e40-125">Accept</span><span class="sxs-lookup"><span data-stu-id="36e40-125">Accept</span></span>|<span data-ttu-id="36e40-126">application/json</span><span class="sxs-lookup"><span data-stu-id="36e40-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36e40-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="36e40-127">Request body</span></span>
<span data-ttu-id="36e40-128">В тексте запроса добавьте представление объекта Даташарингконсент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="36e40-128">In the request body, supply a JSON representation for the dataSharingConsent object.</span></span>

<span data-ttu-id="36e40-129">В следующей таблице приведены свойства, необходимые при создании Даташарингконсент.</span><span class="sxs-lookup"><span data-stu-id="36e40-129">The following table shows the properties that are required when you create the dataSharingConsent.</span></span>

|<span data-ttu-id="36e40-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="36e40-130">Property</span></span>|<span data-ttu-id="36e40-131">Тип</span><span class="sxs-lookup"><span data-stu-id="36e40-131">Type</span></span>|<span data-ttu-id="36e40-132">Описание</span><span class="sxs-lookup"><span data-stu-id="36e40-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36e40-133">id</span><span class="sxs-lookup"><span data-stu-id="36e40-133">id</span></span>|<span data-ttu-id="36e40-134">String</span><span class="sxs-lookup"><span data-stu-id="36e40-134">String</span></span>|<span data-ttu-id="36e40-135">Идентификатор согласия общего доступа к данным</span><span class="sxs-lookup"><span data-stu-id="36e40-135">The data sharing consent Id</span></span>|
|<span data-ttu-id="36e40-136">сервицедисплайнаме</span><span class="sxs-lookup"><span data-stu-id="36e40-136">serviceDisplayName</span></span>|<span data-ttu-id="36e40-137">String</span><span class="sxs-lookup"><span data-stu-id="36e40-137">String</span></span>|<span data-ttu-id="36e40-138">Отображаемое имя рабочего процесса службы</span><span class="sxs-lookup"><span data-stu-id="36e40-138">The display name of the service work flow</span></span>|
|<span data-ttu-id="36e40-139">термсурл</span><span class="sxs-lookup"><span data-stu-id="36e40-139">termsUrl</span></span>|<span data-ttu-id="36e40-140">String</span><span class="sxs-lookup"><span data-stu-id="36e40-140">String</span></span>|<span data-ttu-id="36e40-141">Термсурл для согласия общего доступа к данным</span><span class="sxs-lookup"><span data-stu-id="36e40-141">The TermsUrl for the data sharing consent</span></span>|
|<span data-ttu-id="36e40-142">granted</span><span class="sxs-lookup"><span data-stu-id="36e40-142">granted</span></span>|<span data-ttu-id="36e40-143">Логический</span><span class="sxs-lookup"><span data-stu-id="36e40-143">Boolean</span></span>|<span data-ttu-id="36e40-144">Состояние предоставления согласия на общий доступ к данным</span><span class="sxs-lookup"><span data-stu-id="36e40-144">The granted state for the data sharing consent</span></span>|
|<span data-ttu-id="36e40-145">грантдатетиме</span><span class="sxs-lookup"><span data-stu-id="36e40-145">grantDateTime</span></span>|<span data-ttu-id="36e40-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36e40-146">DateTimeOffset</span></span>|<span data-ttu-id="36e40-147">Для этой учетной записи предоставлено согласие по времени</span><span class="sxs-lookup"><span data-stu-id="36e40-147">The time consent was granted for this account</span></span>|
|<span data-ttu-id="36e40-148">грантедбюпн</span><span class="sxs-lookup"><span data-stu-id="36e40-148">grantedByUpn</span></span>|<span data-ttu-id="36e40-149">String</span><span class="sxs-lookup"><span data-stu-id="36e40-149">String</span></span>|<span data-ttu-id="36e40-150">Имя участника-пользователя, которому назначено согласие для этой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="36e40-150">The Upn of the user that granted consent for this account</span></span>|
|<span data-ttu-id="36e40-151">грантедбюсерид</span><span class="sxs-lookup"><span data-stu-id="36e40-151">grantedByUserId</span></span>|<span data-ttu-id="36e40-152">String</span><span class="sxs-lookup"><span data-stu-id="36e40-152">String</span></span>|<span data-ttu-id="36e40-153">UserId пользователя, который предоставил согласие для этой учетной записи</span><span class="sxs-lookup"><span data-stu-id="36e40-153">The UserId of the user that granted consent for this account</span></span>|



## <a name="response"></a><span data-ttu-id="36e40-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="36e40-154">Response</span></span>
<span data-ttu-id="36e40-155">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [даташарингконсент](../resources/intune-devices-datasharingconsent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="36e40-155">If successful, this method returns a `201 Created` response code and a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36e40-156">Пример</span><span class="sxs-lookup"><span data-stu-id="36e40-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="36e40-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="36e40-157">Request</span></span>
<span data-ttu-id="36e40-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="36e40-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="36e40-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="36e40-159">Response</span></span>
<span data-ttu-id="36e40-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="36e40-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





