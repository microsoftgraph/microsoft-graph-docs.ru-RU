---
title: Создание Даташарингконсент
description: Создание нового объекта Даташарингконсент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 27188e57b3fe087ef3950a4155dc9a789ef203bd
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36348874"
---
# <a name="create-datasharingconsent"></a><span data-ttu-id="c6493-103">Создание Даташарингконсент</span><span class="sxs-lookup"><span data-stu-id="c6493-103">Create dataSharingConsent</span></span>

> <span data-ttu-id="c6493-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6493-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c6493-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c6493-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6493-106">Создание нового объекта [даташарингконсент](../resources/intune-devices-datasharingconsent.md) .</span><span class="sxs-lookup"><span data-stu-id="c6493-106">Create a new [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c6493-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c6493-107">Prerequisites</span></span>
<span data-ttu-id="c6493-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6493-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6493-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c6493-110">Permission type</span></span>|<span data-ttu-id="c6493-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c6493-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c6493-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c6493-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c6493-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6493-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c6493-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c6493-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c6493-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6493-115">Not supported.</span></span>|
|<span data-ttu-id="c6493-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c6493-116">Application</span></span>|<span data-ttu-id="c6493-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6493-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c6493-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c6493-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/dataSharingConsents
```

## <a name="request-headers"></a><span data-ttu-id="c6493-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c6493-119">Request headers</span></span>
|<span data-ttu-id="c6493-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c6493-120">Header</span></span>|<span data-ttu-id="c6493-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c6493-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c6493-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c6493-122">Authorization</span></span>|<span data-ttu-id="c6493-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c6493-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c6493-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c6493-124">Accept</span></span>|<span data-ttu-id="c6493-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c6493-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6493-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c6493-126">Request body</span></span>
<span data-ttu-id="c6493-127">В тексте запроса добавьте представление объекта Даташарингконсент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c6493-127">In the request body, supply a JSON representation for the dataSharingConsent object.</span></span>

<span data-ttu-id="c6493-128">В следующей таблице приведены свойства, необходимые при создании Даташарингконсент.</span><span class="sxs-lookup"><span data-stu-id="c6493-128">The following table shows the properties that are required when you create the dataSharingConsent.</span></span>

|<span data-ttu-id="c6493-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c6493-129">Property</span></span>|<span data-ttu-id="c6493-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c6493-130">Type</span></span>|<span data-ttu-id="c6493-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c6493-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6493-132">id</span><span class="sxs-lookup"><span data-stu-id="c6493-132">id</span></span>|<span data-ttu-id="c6493-133">String</span><span class="sxs-lookup"><span data-stu-id="c6493-133">String</span></span>|<span data-ttu-id="c6493-134">Идентификатор согласия общего доступа к данным</span><span class="sxs-lookup"><span data-stu-id="c6493-134">The data sharing consent Id</span></span>|
|<span data-ttu-id="c6493-135">сервицедисплайнаме</span><span class="sxs-lookup"><span data-stu-id="c6493-135">serviceDisplayName</span></span>|<span data-ttu-id="c6493-136">String</span><span class="sxs-lookup"><span data-stu-id="c6493-136">String</span></span>|<span data-ttu-id="c6493-137">Отображаемое имя рабочего процесса службы</span><span class="sxs-lookup"><span data-stu-id="c6493-137">The display name of the service work flow</span></span>|
|<span data-ttu-id="c6493-138">термсурл</span><span class="sxs-lookup"><span data-stu-id="c6493-138">termsUrl</span></span>|<span data-ttu-id="c6493-139">String</span><span class="sxs-lookup"><span data-stu-id="c6493-139">String</span></span>|<span data-ttu-id="c6493-140">Термсурл для согласия общего доступа к данным</span><span class="sxs-lookup"><span data-stu-id="c6493-140">The TermsUrl for the data sharing consent</span></span>|
|<span data-ttu-id="c6493-141">granted</span><span class="sxs-lookup"><span data-stu-id="c6493-141">granted</span></span>|<span data-ttu-id="c6493-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6493-142">Boolean</span></span>|<span data-ttu-id="c6493-143">Состояние предоставления согласия на общий доступ к данным</span><span class="sxs-lookup"><span data-stu-id="c6493-143">The granted state for the data sharing consent</span></span>|
|<span data-ttu-id="c6493-144">грантдатетиме</span><span class="sxs-lookup"><span data-stu-id="c6493-144">grantDateTime</span></span>|<span data-ttu-id="c6493-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6493-145">DateTimeOffset</span></span>|<span data-ttu-id="c6493-146">Для этой учетной записи предоставлено согласие по времени</span><span class="sxs-lookup"><span data-stu-id="c6493-146">The time consent was granted for this account</span></span>|
|<span data-ttu-id="c6493-147">грантедбюпн</span><span class="sxs-lookup"><span data-stu-id="c6493-147">grantedByUpn</span></span>|<span data-ttu-id="c6493-148">String</span><span class="sxs-lookup"><span data-stu-id="c6493-148">String</span></span>|<span data-ttu-id="c6493-149">Имя участника-пользователя, которому назначено согласие для этой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="c6493-149">The Upn of the user that granted consent for this account</span></span>|
|<span data-ttu-id="c6493-150">грантедбюсерид</span><span class="sxs-lookup"><span data-stu-id="c6493-150">grantedByUserId</span></span>|<span data-ttu-id="c6493-151">String</span><span class="sxs-lookup"><span data-stu-id="c6493-151">String</span></span>|<span data-ttu-id="c6493-152">UserId пользователя, который предоставил согласие для этой учетной записи</span><span class="sxs-lookup"><span data-stu-id="c6493-152">The UserId of the user that granted consent for this account</span></span>|



## <a name="response"></a><span data-ttu-id="c6493-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6493-153">Response</span></span>
<span data-ttu-id="c6493-154">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [даташарингконсент](../resources/intune-devices-datasharingconsent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c6493-154">If successful, this method returns a `201 Created` response code and a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6493-155">Пример</span><span class="sxs-lookup"><span data-stu-id="c6493-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="c6493-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="c6493-156">Request</span></span>
<span data-ttu-id="c6493-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c6493-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c6493-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6493-158">Response</span></span>
<span data-ttu-id="c6493-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c6493-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






