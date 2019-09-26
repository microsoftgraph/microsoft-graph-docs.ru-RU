---
title: Обновление объекта termsAndConditionsAcceptanceStatus
description: Обновление свойств объекта termsAndConditionsAcceptanceStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5cf52934553af8d1fba8fca5a795f614b51f4223
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37170506"
---
# <a name="update-termsandconditionsacceptancestatus"></a><span data-ttu-id="953e2-103">Обновление объекта termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="953e2-103">Update termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="953e2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="953e2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="953e2-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="953e2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="953e2-106">Обновление свойств объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="953e2-106">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="953e2-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="953e2-107">Prerequisites</span></span>
<span data-ttu-id="953e2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="953e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="953e2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="953e2-110">Permission type</span></span>|<span data-ttu-id="953e2-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="953e2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="953e2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="953e2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="953e2-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="953e2-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="953e2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="953e2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="953e2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="953e2-115">Not supported.</span></span>|
|<span data-ttu-id="953e2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="953e2-116">Application</span></span>|<span data-ttu-id="953e2-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="953e2-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="953e2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="953e2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="953e2-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="953e2-119">Request headers</span></span>
|<span data-ttu-id="953e2-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="953e2-120">Header</span></span>|<span data-ttu-id="953e2-121">Значение</span><span class="sxs-lookup"><span data-stu-id="953e2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="953e2-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="953e2-122">Authorization</span></span>|<span data-ttu-id="953e2-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="953e2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="953e2-124">Accept</span><span class="sxs-lookup"><span data-stu-id="953e2-124">Accept</span></span>|<span data-ttu-id="953e2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="953e2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="953e2-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="953e2-126">Request body</span></span>
<span data-ttu-id="953e2-127">В тексте запроса добавьте представление объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="953e2-127">In the request body, supply a JSON representation for the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

<span data-ttu-id="953e2-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="953e2-128">The following table shows the properties that are required when you create the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span></span>

|<span data-ttu-id="953e2-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="953e2-129">Property</span></span>|<span data-ttu-id="953e2-130">Тип</span><span class="sxs-lookup"><span data-stu-id="953e2-130">Type</span></span>|<span data-ttu-id="953e2-131">Описание</span><span class="sxs-lookup"><span data-stu-id="953e2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="953e2-132">id</span><span class="sxs-lookup"><span data-stu-id="953e2-132">id</span></span>|<span data-ttu-id="953e2-133">Строка</span><span class="sxs-lookup"><span data-stu-id="953e2-133">String</span></span>|<span data-ttu-id="953e2-134">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="953e2-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="953e2-135">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="953e2-135">userDisplayName</span></span>|<span data-ttu-id="953e2-136">String</span><span class="sxs-lookup"><span data-stu-id="953e2-136">String</span></span>|<span data-ttu-id="953e2-137">Отображает имя пользователя, чье принятие представлено объектом.</span><span class="sxs-lookup"><span data-stu-id="953e2-137">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="953e2-138">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="953e2-138">acceptedVersion</span></span>|<span data-ttu-id="953e2-139">Int32</span><span class="sxs-lookup"><span data-stu-id="953e2-139">Int32</span></span>|<span data-ttu-id="953e2-140">Номер последней версии условий, принятых пользователем.</span><span class="sxs-lookup"><span data-stu-id="953e2-140">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="953e2-141">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="953e2-141">acceptedDateTime</span></span>|<span data-ttu-id="953e2-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="953e2-142">DateTimeOffset</span></span>|<span data-ttu-id="953e2-143">Дата и время последнего принятия условий пользователем.</span><span class="sxs-lookup"><span data-stu-id="953e2-143">DateTime when the terms were last accepted by the user.</span></span>|



## <a name="response"></a><span data-ttu-id="953e2-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="953e2-144">Response</span></span>
<span data-ttu-id="953e2-145">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="953e2-145">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="953e2-146">Пример</span><span class="sxs-lookup"><span data-stu-id="953e2-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="953e2-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="953e2-147">Request</span></span>
<span data-ttu-id="953e2-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="953e2-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```

### <a name="response"></a><span data-ttu-id="953e2-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="953e2-149">Response</span></span>
<span data-ttu-id="953e2-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="953e2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 260

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "a045ce1a-ce1a-a045-1ace-45a01ace45a0",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```




