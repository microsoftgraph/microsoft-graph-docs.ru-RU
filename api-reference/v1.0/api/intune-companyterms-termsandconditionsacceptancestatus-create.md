---
title: Создание объекта termsAndConditionsAcceptanceStatus
description: Создание объекта termsAndConditionsAcceptanceStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ec1b815b86e9ce7618dfdd5f66b32c9dd7737bb0
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759394"
---
# <a name="create-termsandconditionsacceptancestatus"></a><span data-ttu-id="44cbf-103">Создание объекта termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="44cbf-103">Create termsAndConditionsAcceptanceStatus</span></span>

<span data-ttu-id="44cbf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44cbf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="44cbf-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="44cbf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44cbf-106">Создание объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="44cbf-106">Create a new [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="44cbf-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="44cbf-107">Prerequisites</span></span>
<span data-ttu-id="44cbf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44cbf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44cbf-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="44cbf-110">Permission type</span></span>|<span data-ttu-id="44cbf-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="44cbf-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44cbf-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="44cbf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="44cbf-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44cbf-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="44cbf-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="44cbf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44cbf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44cbf-115">Not supported.</span></span>|
|<span data-ttu-id="44cbf-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="44cbf-116">Application</span></span>|<span data-ttu-id="44cbf-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44cbf-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="44cbf-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="44cbf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="44cbf-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="44cbf-119">Request headers</span></span>
|<span data-ttu-id="44cbf-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="44cbf-120">Header</span></span>|<span data-ttu-id="44cbf-121">Значение</span><span class="sxs-lookup"><span data-stu-id="44cbf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44cbf-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="44cbf-122">Authorization</span></span>|<span data-ttu-id="44cbf-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="44cbf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44cbf-124">Accept</span><span class="sxs-lookup"><span data-stu-id="44cbf-124">Accept</span></span>|<span data-ttu-id="44cbf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="44cbf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44cbf-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="44cbf-126">Request body</span></span>
<span data-ttu-id="44cbf-127">В тексте запроса добавьте представление объекта termsAndConditionsAcceptanceStatus в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="44cbf-127">In the request body, supply a JSON representation for the termsAndConditionsAcceptanceStatus object.</span></span>

<span data-ttu-id="44cbf-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта termsAndConditionsAcceptanceStatus.</span><span class="sxs-lookup"><span data-stu-id="44cbf-128">The following table shows the properties that are required when you create the termsAndConditionsAcceptanceStatus.</span></span>

|<span data-ttu-id="44cbf-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="44cbf-129">Property</span></span>|<span data-ttu-id="44cbf-130">Тип</span><span class="sxs-lookup"><span data-stu-id="44cbf-130">Type</span></span>|<span data-ttu-id="44cbf-131">Описание</span><span class="sxs-lookup"><span data-stu-id="44cbf-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44cbf-132">id</span><span class="sxs-lookup"><span data-stu-id="44cbf-132">id</span></span>|<span data-ttu-id="44cbf-133">String</span><span class="sxs-lookup"><span data-stu-id="44cbf-133">String</span></span>|<span data-ttu-id="44cbf-134">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="44cbf-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="44cbf-135">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="44cbf-135">userDisplayName</span></span>|<span data-ttu-id="44cbf-136">String</span><span class="sxs-lookup"><span data-stu-id="44cbf-136">String</span></span>|<span data-ttu-id="44cbf-137">Отображает имя пользователя, чье принятие представлено объектом.</span><span class="sxs-lookup"><span data-stu-id="44cbf-137">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="44cbf-138">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="44cbf-138">acceptedVersion</span></span>|<span data-ttu-id="44cbf-139">Int32</span><span class="sxs-lookup"><span data-stu-id="44cbf-139">Int32</span></span>|<span data-ttu-id="44cbf-140">Номер последней версии условий, принятых пользователем.</span><span class="sxs-lookup"><span data-stu-id="44cbf-140">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="44cbf-141">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="44cbf-141">acceptedDateTime</span></span>|<span data-ttu-id="44cbf-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44cbf-142">DateTimeOffset</span></span>|<span data-ttu-id="44cbf-143">Дата и время последнего принятия условий пользователем.</span><span class="sxs-lookup"><span data-stu-id="44cbf-143">DateTime when the terms were last accepted by the user.</span></span>|
|<span data-ttu-id="44cbf-144">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="44cbf-144">userPrincipalName</span></span>|<span data-ttu-id="44cbf-145">String</span><span class="sxs-lookup"><span data-stu-id="44cbf-145">String</span></span>|<span data-ttu-id="44cbf-146">UserPrincipalName пользователя, который принял этот термин.</span><span class="sxs-lookup"><span data-stu-id="44cbf-146">The userPrincipalName of the User that accepted the term.</span></span>|



## <a name="response"></a><span data-ttu-id="44cbf-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="44cbf-147">Response</span></span>
<span data-ttu-id="44cbf-148">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="44cbf-148">If successful, this method returns a `201 Created` response code and a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44cbf-149">Пример</span><span class="sxs-lookup"><span data-stu-id="44cbf-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="44cbf-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="44cbf-150">Request</span></span>
<span data-ttu-id="44cbf-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="44cbf-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
Content-type: application/json
Content-length: 264

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="44cbf-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="44cbf-152">Response</span></span>
<span data-ttu-id="44cbf-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="44cbf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 313

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "a045ce1a-ce1a-a045-1ace-45a01ace45a0",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00",
  "userPrincipalName": "User Principal Name value"
}
```




