---
title: Создание объекта termsAndConditionsAcceptanceStatus
description: Создание объекта termsAndConditionsAcceptanceStatus.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 154b995cf3e75cc66c2dbc600a79fe3ee56f8dd8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43446228"
---
# <a name="create-termsandconditionsacceptancestatus"></a><span data-ttu-id="fd448-103">Создание объекта termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="fd448-103">Create termsAndConditionsAcceptanceStatus</span></span>

<span data-ttu-id="fd448-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd448-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fd448-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fd448-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd448-106">Создание объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="fd448-106">Create a new [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fd448-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="fd448-107">Prerequisites</span></span>
<span data-ttu-id="fd448-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd448-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd448-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fd448-110">Permission type</span></span>|<span data-ttu-id="fd448-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fd448-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fd448-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fd448-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fd448-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd448-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fd448-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fd448-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd448-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd448-115">Not supported.</span></span>|
|<span data-ttu-id="fd448-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fd448-116">Application</span></span>|<span data-ttu-id="fd448-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd448-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd448-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fd448-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="fd448-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fd448-119">Request headers</span></span>
|<span data-ttu-id="fd448-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fd448-120">Header</span></span>|<span data-ttu-id="fd448-121">Значение</span><span class="sxs-lookup"><span data-stu-id="fd448-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fd448-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd448-122">Authorization</span></span>|<span data-ttu-id="fd448-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fd448-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fd448-124">Accept</span><span class="sxs-lookup"><span data-stu-id="fd448-124">Accept</span></span>|<span data-ttu-id="fd448-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fd448-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd448-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fd448-126">Request body</span></span>
<span data-ttu-id="fd448-127">В тексте запроса добавьте представление объекта termsAndConditionsAcceptanceStatus в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fd448-127">In the request body, supply a JSON representation for the termsAndConditionsAcceptanceStatus object.</span></span>

<span data-ttu-id="fd448-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта termsAndConditionsAcceptanceStatus.</span><span class="sxs-lookup"><span data-stu-id="fd448-128">The following table shows the properties that are required when you create the termsAndConditionsAcceptanceStatus.</span></span>

|<span data-ttu-id="fd448-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="fd448-129">Property</span></span>|<span data-ttu-id="fd448-130">Тип</span><span class="sxs-lookup"><span data-stu-id="fd448-130">Type</span></span>|<span data-ttu-id="fd448-131">Описание</span><span class="sxs-lookup"><span data-stu-id="fd448-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd448-132">id</span><span class="sxs-lookup"><span data-stu-id="fd448-132">id</span></span>|<span data-ttu-id="fd448-133">Строка</span><span class="sxs-lookup"><span data-stu-id="fd448-133">String</span></span>|<span data-ttu-id="fd448-134">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="fd448-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="fd448-135">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="fd448-135">userDisplayName</span></span>|<span data-ttu-id="fd448-136">String</span><span class="sxs-lookup"><span data-stu-id="fd448-136">String</span></span>|<span data-ttu-id="fd448-137">Отображает имя пользователя, чье принятие представлено объектом.</span><span class="sxs-lookup"><span data-stu-id="fd448-137">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="fd448-138">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="fd448-138">acceptedVersion</span></span>|<span data-ttu-id="fd448-139">Int32</span><span class="sxs-lookup"><span data-stu-id="fd448-139">Int32</span></span>|<span data-ttu-id="fd448-140">Номер последней версии условий, принятых пользователем.</span><span class="sxs-lookup"><span data-stu-id="fd448-140">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="fd448-141">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="fd448-141">acceptedDateTime</span></span>|<span data-ttu-id="fd448-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd448-142">DateTimeOffset</span></span>|<span data-ttu-id="fd448-143">Дата и время последнего принятия условий пользователем.</span><span class="sxs-lookup"><span data-stu-id="fd448-143">DateTime when the terms were last accepted by the user.</span></span>|



## <a name="response"></a><span data-ttu-id="fd448-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd448-144">Response</span></span>
<span data-ttu-id="fd448-145">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fd448-145">If successful, this method returns a `201 Created` response code and a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd448-146">Пример</span><span class="sxs-lookup"><span data-stu-id="fd448-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="fd448-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="fd448-147">Request</span></span>
<span data-ttu-id="fd448-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fd448-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```

### <a name="response"></a><span data-ttu-id="fd448-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd448-149">Response</span></span>
<span data-ttu-id="fd448-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fd448-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






