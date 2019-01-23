---
title: Создание dataSharingConsent
description: Создание нового объекта dataSharingConsent.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 686f8e5ddb56c53224d467bc6ac31cfdb5b6858c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406950"
---
# <a name="create-datasharingconsent"></a><span data-ttu-id="af57c-103">Создание dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="af57c-103">Create dataSharingConsent</span></span>

> <span data-ttu-id="af57c-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="af57c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="af57c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af57c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="af57c-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="af57c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af57c-107">Создание нового объекта [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) .</span><span class="sxs-lookup"><span data-stu-id="af57c-107">Create a new [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="af57c-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="af57c-108">Prerequisites</span></span>
<span data-ttu-id="af57c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="af57c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="af57c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="af57c-111">Permission type</span></span>|<span data-ttu-id="af57c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="af57c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af57c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="af57c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="af57c-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af57c-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="af57c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="af57c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af57c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af57c-116">Not supported.</span></span>|
|<span data-ttu-id="af57c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="af57c-117">Application</span></span>|<span data-ttu-id="af57c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af57c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="af57c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="af57c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/dataSharingConsents
```

## <a name="request-headers"></a><span data-ttu-id="af57c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="af57c-120">Request headers</span></span>
|<span data-ttu-id="af57c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="af57c-121">Header</span></span>|<span data-ttu-id="af57c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="af57c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af57c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="af57c-123">Authorization</span></span>|<span data-ttu-id="af57c-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="af57c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af57c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="af57c-125">Accept</span></span>|<span data-ttu-id="af57c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="af57c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af57c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="af57c-127">Request body</span></span>
<span data-ttu-id="af57c-128">В тексте запроса укажите представление JSON для объекта dataSharingConsent.</span><span class="sxs-lookup"><span data-stu-id="af57c-128">In the request body, supply a JSON representation for the dataSharingConsent object.</span></span>

<span data-ttu-id="af57c-129">В следующей таблице показаны свойства, которые необходимы для создания dataSharingConsent.</span><span class="sxs-lookup"><span data-stu-id="af57c-129">The following table shows the properties that are required when you create the dataSharingConsent.</span></span>

|<span data-ttu-id="af57c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="af57c-130">Property</span></span>|<span data-ttu-id="af57c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="af57c-131">Type</span></span>|<span data-ttu-id="af57c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="af57c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af57c-133">id</span><span class="sxs-lookup"><span data-stu-id="af57c-133">id</span></span>|<span data-ttu-id="af57c-134">String</span><span class="sxs-lookup"><span data-stu-id="af57c-134">String</span></span>|<span data-ttu-id="af57c-135">Разрешения общего доступа данных идентификатор</span><span class="sxs-lookup"><span data-stu-id="af57c-135">The data sharing consent Id</span></span>|
|<span data-ttu-id="af57c-136">Отображаемое_имя_службы</span><span class="sxs-lookup"><span data-stu-id="af57c-136">serviceDisplayName</span></span>|<span data-ttu-id="af57c-137">String</span><span class="sxs-lookup"><span data-stu-id="af57c-137">String</span></span>|<span data-ttu-id="af57c-138">Отображаемое имя службы рабочих процессов</span><span class="sxs-lookup"><span data-stu-id="af57c-138">The display name of the service work flow</span></span>|
|<span data-ttu-id="af57c-139">termsUrl</span><span class="sxs-lookup"><span data-stu-id="af57c-139">termsUrl</span></span>|<span data-ttu-id="af57c-140">String</span><span class="sxs-lookup"><span data-stu-id="af57c-140">String</span></span>|<span data-ttu-id="af57c-141">TermsUrl для данных, общий доступ к согласия</span><span class="sxs-lookup"><span data-stu-id="af57c-141">The TermsUrl for the data sharing consent</span></span>|
|<span data-ttu-id="af57c-142">предоставлено</span><span class="sxs-lookup"><span data-stu-id="af57c-142">granted</span></span>|<span data-ttu-id="af57c-143">Логический</span><span class="sxs-lookup"><span data-stu-id="af57c-143">Boolean</span></span>|<span data-ttu-id="af57c-144">Предоставленные состояний для данных, общий доступ к согласия</span><span class="sxs-lookup"><span data-stu-id="af57c-144">The granted state for the data sharing consent</span></span>|
|<span data-ttu-id="af57c-145">grantDateTime</span><span class="sxs-lookup"><span data-stu-id="af57c-145">grantDateTime</span></span>|<span data-ttu-id="af57c-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af57c-146">DateTimeOffset</span></span>|<span data-ttu-id="af57c-147">Были предоставлены разрешения времени для этой учетной записи</span><span class="sxs-lookup"><span data-stu-id="af57c-147">The time consent was granted for this account</span></span>|
|<span data-ttu-id="af57c-148">grantedByUpn</span><span class="sxs-lookup"><span data-stu-id="af57c-148">grantedByUpn</span></span>|<span data-ttu-id="af57c-149">String</span><span class="sxs-lookup"><span data-stu-id="af57c-149">String</span></span>|<span data-ttu-id="af57c-150">Имя участника-пользователя, которой предоставлены разрешения для этой учетной записи</span><span class="sxs-lookup"><span data-stu-id="af57c-150">The Upn of the user that granted consent for this account</span></span>|
|<span data-ttu-id="af57c-151">grantedByUserId</span><span class="sxs-lookup"><span data-stu-id="af57c-151">grantedByUserId</span></span>|<span data-ttu-id="af57c-152">String</span><span class="sxs-lookup"><span data-stu-id="af57c-152">String</span></span>|<span data-ttu-id="af57c-153">Идентификатор пользователя, который предоставлены разрешения для этой учетной записи пользователя</span><span class="sxs-lookup"><span data-stu-id="af57c-153">The UserId of the user that granted consent for this account</span></span>|



## <a name="response"></a><span data-ttu-id="af57c-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="af57c-154">Response</span></span>
<span data-ttu-id="af57c-155">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="af57c-155">If successful, this method returns a `201 Created` response code and a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af57c-156">Пример</span><span class="sxs-lookup"><span data-stu-id="af57c-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="af57c-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="af57c-157">Request</span></span>
<span data-ttu-id="af57c-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="af57c-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="af57c-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="af57c-159">Response</span></span>
<span data-ttu-id="af57c-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="af57c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




