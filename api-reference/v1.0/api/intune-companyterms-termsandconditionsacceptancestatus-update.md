---
title: Обновление объекта termsAndConditionsAcceptanceStatus
description: Обновление свойств объекта termsAndConditionsAcceptanceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 06169225518f6110cb571d53ba818cd8fece49e7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36019767"
---
# <a name="update-termsandconditionsacceptancestatus"></a><span data-ttu-id="d44e6-103">Обновление объекта termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="d44e6-103">Update termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="d44e6-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d44e6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d44e6-105">Обновление свойств объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="d44e6-105">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d44e6-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d44e6-106">Prerequisites</span></span>
<span data-ttu-id="d44e6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d44e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d44e6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d44e6-109">Permission type</span></span>|<span data-ttu-id="d44e6-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d44e6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d44e6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d44e6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d44e6-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d44e6-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d44e6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d44e6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d44e6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d44e6-114">Not supported.</span></span>|
|<span data-ttu-id="d44e6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d44e6-115">Application</span></span>|<span data-ttu-id="d44e6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d44e6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d44e6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d44e6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="d44e6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d44e6-118">Request headers</span></span>
|<span data-ttu-id="d44e6-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d44e6-119">Header</span></span>|<span data-ttu-id="d44e6-120">Значение</span><span class="sxs-lookup"><span data-stu-id="d44e6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d44e6-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d44e6-121">Authorization</span></span>|<span data-ttu-id="d44e6-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d44e6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d44e6-123">Accept</span><span class="sxs-lookup"><span data-stu-id="d44e6-123">Accept</span></span>|<span data-ttu-id="d44e6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d44e6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d44e6-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d44e6-125">Request body</span></span>
<span data-ttu-id="d44e6-126">В тексте запроса добавьте представление объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d44e6-126">In the request body, supply a JSON representation for the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

<span data-ttu-id="d44e6-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="d44e6-127">The following table shows the properties that are required when you create the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span></span>

|<span data-ttu-id="d44e6-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="d44e6-128">Property</span></span>|<span data-ttu-id="d44e6-129">Тип</span><span class="sxs-lookup"><span data-stu-id="d44e6-129">Type</span></span>|<span data-ttu-id="d44e6-130">Описание</span><span class="sxs-lookup"><span data-stu-id="d44e6-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d44e6-131">id</span><span class="sxs-lookup"><span data-stu-id="d44e6-131">id</span></span>|<span data-ttu-id="d44e6-132">Строка</span><span class="sxs-lookup"><span data-stu-id="d44e6-132">String</span></span>|<span data-ttu-id="d44e6-133">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="d44e6-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="d44e6-134">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="d44e6-134">userDisplayName</span></span>|<span data-ttu-id="d44e6-135">String</span><span class="sxs-lookup"><span data-stu-id="d44e6-135">String</span></span>|<span data-ttu-id="d44e6-136">Отображает имя пользователя, чье принятие представлено объектом.</span><span class="sxs-lookup"><span data-stu-id="d44e6-136">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="d44e6-137">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="d44e6-137">acceptedVersion</span></span>|<span data-ttu-id="d44e6-138">Int32</span><span class="sxs-lookup"><span data-stu-id="d44e6-138">Int32</span></span>|<span data-ttu-id="d44e6-139">Номер последней версии условий, принятых пользователем.</span><span class="sxs-lookup"><span data-stu-id="d44e6-139">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="d44e6-140">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="d44e6-140">acceptedDateTime</span></span>|<span data-ttu-id="d44e6-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d44e6-141">DateTimeOffset</span></span>|<span data-ttu-id="d44e6-142">Дата и время последнего принятия условий пользователем.</span><span class="sxs-lookup"><span data-stu-id="d44e6-142">DateTime when the terms were last accepted by the user.</span></span>|



## <a name="response"></a><span data-ttu-id="d44e6-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="d44e6-143">Response</span></span>
<span data-ttu-id="d44e6-144">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d44e6-144">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d44e6-145">Пример</span><span class="sxs-lookup"><span data-stu-id="d44e6-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="d44e6-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="d44e6-146">Request</span></span>
<span data-ttu-id="d44e6-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d44e6-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```

### <a name="response"></a><span data-ttu-id="d44e6-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="d44e6-148">Response</span></span>
<span data-ttu-id="d44e6-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d44e6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



