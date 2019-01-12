---
title: Создание dataSharingConsent
description: Создание нового объекта dataSharingConsent.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 83d329072b6e18f8ecbb745769e872c76fdae86b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919080"
---
# <a name="create-datasharingconsent"></a><span data-ttu-id="db0b9-103">Создание dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="db0b9-103">Create dataSharingConsent</span></span>

> <span data-ttu-id="db0b9-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="db0b9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="db0b9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db0b9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="db0b9-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="db0b9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="db0b9-107">Создание нового объекта [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) .</span><span class="sxs-lookup"><span data-stu-id="db0b9-107">Create a new [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="db0b9-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="db0b9-108">Prerequisites</span></span>
<span data-ttu-id="db0b9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db0b9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db0b9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="db0b9-111">Permission type</span></span>|<span data-ttu-id="db0b9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="db0b9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="db0b9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="db0b9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="db0b9-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db0b9-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="db0b9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="db0b9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db0b9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db0b9-116">Not supported.</span></span>|
|<span data-ttu-id="db0b9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="db0b9-117">Application</span></span>|<span data-ttu-id="db0b9-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db0b9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="db0b9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="db0b9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/dataSharingConsents
```

## <a name="request-headers"></a><span data-ttu-id="db0b9-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="db0b9-120">Request headers</span></span>
|<span data-ttu-id="db0b9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="db0b9-121">Header</span></span>|<span data-ttu-id="db0b9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="db0b9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="db0b9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="db0b9-123">Authorization</span></span>|<span data-ttu-id="db0b9-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="db0b9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="db0b9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="db0b9-125">Accept</span></span>|<span data-ttu-id="db0b9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="db0b9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="db0b9-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="db0b9-127">Request body</span></span>
<span data-ttu-id="db0b9-128">В тексте запроса укажите представление JSON для объекта dataSharingConsent.</span><span class="sxs-lookup"><span data-stu-id="db0b9-128">In the request body, supply a JSON representation for the dataSharingConsent object.</span></span>

<span data-ttu-id="db0b9-129">В следующей таблице показаны свойства, которые необходимы для создания dataSharingConsent.</span><span class="sxs-lookup"><span data-stu-id="db0b9-129">The following table shows the properties that are required when you create the dataSharingConsent.</span></span>

|<span data-ttu-id="db0b9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="db0b9-130">Property</span></span>|<span data-ttu-id="db0b9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="db0b9-131">Type</span></span>|<span data-ttu-id="db0b9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="db0b9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db0b9-133">id</span><span class="sxs-lookup"><span data-stu-id="db0b9-133">id</span></span>|<span data-ttu-id="db0b9-134">String</span><span class="sxs-lookup"><span data-stu-id="db0b9-134">String</span></span>|<span data-ttu-id="db0b9-135">Разрешения общего доступа данных идентификатор</span><span class="sxs-lookup"><span data-stu-id="db0b9-135">The data sharing consent Id</span></span>|
|<span data-ttu-id="db0b9-136">Отображаемое_имя_службы</span><span class="sxs-lookup"><span data-stu-id="db0b9-136">serviceDisplayName</span></span>|<span data-ttu-id="db0b9-137">String</span><span class="sxs-lookup"><span data-stu-id="db0b9-137">String</span></span>|<span data-ttu-id="db0b9-138">Отображаемое имя службы рабочих процессов</span><span class="sxs-lookup"><span data-stu-id="db0b9-138">The display name of the service work flow</span></span>|
|<span data-ttu-id="db0b9-139">termsUrl</span><span class="sxs-lookup"><span data-stu-id="db0b9-139">termsUrl</span></span>|<span data-ttu-id="db0b9-140">String</span><span class="sxs-lookup"><span data-stu-id="db0b9-140">String</span></span>|<span data-ttu-id="db0b9-141">TermsUrl для данных, общий доступ к согласия</span><span class="sxs-lookup"><span data-stu-id="db0b9-141">The TermsUrl for the data sharing consent</span></span>|
|<span data-ttu-id="db0b9-142">предоставлено</span><span class="sxs-lookup"><span data-stu-id="db0b9-142">granted</span></span>|<span data-ttu-id="db0b9-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="db0b9-143">Boolean</span></span>|<span data-ttu-id="db0b9-144">Предоставленные состояний для данных, общий доступ к согласия</span><span class="sxs-lookup"><span data-stu-id="db0b9-144">The granted state for the data sharing consent</span></span>|
|<span data-ttu-id="db0b9-145">grantDateTime</span><span class="sxs-lookup"><span data-stu-id="db0b9-145">grantDateTime</span></span>|<span data-ttu-id="db0b9-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db0b9-146">DateTimeOffset</span></span>|<span data-ttu-id="db0b9-147">Были предоставлены разрешения времени для этой учетной записи</span><span class="sxs-lookup"><span data-stu-id="db0b9-147">The time consent was granted for this account</span></span>|
|<span data-ttu-id="db0b9-148">grantedByUpn</span><span class="sxs-lookup"><span data-stu-id="db0b9-148">grantedByUpn</span></span>|<span data-ttu-id="db0b9-149">String</span><span class="sxs-lookup"><span data-stu-id="db0b9-149">String</span></span>|<span data-ttu-id="db0b9-150">Имя участника-пользователя, которой предоставлены разрешения для этой учетной записи</span><span class="sxs-lookup"><span data-stu-id="db0b9-150">The Upn of the user that granted consent for this account</span></span>|
|<span data-ttu-id="db0b9-151">grantedByUserId</span><span class="sxs-lookup"><span data-stu-id="db0b9-151">grantedByUserId</span></span>|<span data-ttu-id="db0b9-152">String</span><span class="sxs-lookup"><span data-stu-id="db0b9-152">String</span></span>|<span data-ttu-id="db0b9-153">Идентификатор пользователя, который предоставлены разрешения для этой учетной записи пользователя</span><span class="sxs-lookup"><span data-stu-id="db0b9-153">The UserId of the user that granted consent for this account</span></span>|



## <a name="response"></a><span data-ttu-id="db0b9-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="db0b9-154">Response</span></span>
<span data-ttu-id="db0b9-155">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="db0b9-155">If successful, this method returns a `201 Created` response code and a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db0b9-156">Пример</span><span class="sxs-lookup"><span data-stu-id="db0b9-156">Example</span></span>
### <a name="request"></a><span data-ttu-id="db0b9-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="db0b9-157">Request</span></span>
<span data-ttu-id="db0b9-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="db0b9-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="db0b9-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="db0b9-159">Response</span></span>
<span data-ttu-id="db0b9-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="db0b9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





