---
title: Создание объекта termsAndConditionsAcceptanceStatus
description: Создание объекта termsAndConditionsAcceptanceStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 88e29e32ae772b6bc0b0b6fb4c395ab400190bbc
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133586"
---
# <a name="create-termsandconditionsacceptancestatus"></a><span data-ttu-id="751ce-103">Создание объекта termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="751ce-103">Create termsAndConditionsAcceptanceStatus</span></span>

<span data-ttu-id="751ce-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="751ce-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="751ce-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="751ce-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="751ce-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="751ce-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="751ce-107">Создание объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="751ce-107">Create a new [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="751ce-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="751ce-108">Prerequisites</span></span>
<span data-ttu-id="751ce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="751ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="751ce-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="751ce-111">Permission type</span></span>|<span data-ttu-id="751ce-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="751ce-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="751ce-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="751ce-113">Delegated (work or school account)</span></span>|<span data-ttu-id="751ce-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="751ce-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="751ce-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="751ce-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="751ce-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="751ce-116">Not supported.</span></span>|
|<span data-ttu-id="751ce-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="751ce-117">Application</span></span>|<span data-ttu-id="751ce-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="751ce-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="751ce-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="751ce-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="751ce-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="751ce-120">Request headers</span></span>
|<span data-ttu-id="751ce-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="751ce-121">Header</span></span>|<span data-ttu-id="751ce-122">Значение</span><span class="sxs-lookup"><span data-stu-id="751ce-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="751ce-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="751ce-123">Authorization</span></span>|<span data-ttu-id="751ce-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="751ce-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="751ce-125">Accept</span><span class="sxs-lookup"><span data-stu-id="751ce-125">Accept</span></span>|<span data-ttu-id="751ce-126">application/json</span><span class="sxs-lookup"><span data-stu-id="751ce-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="751ce-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="751ce-127">Request body</span></span>
<span data-ttu-id="751ce-128">В тексте запроса добавьте представление объекта termsAndConditionsAcceptanceStatus в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="751ce-128">In the request body, supply a JSON representation for the termsAndConditionsAcceptanceStatus object.</span></span>

<span data-ttu-id="751ce-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта termsAndConditionsAcceptanceStatus.</span><span class="sxs-lookup"><span data-stu-id="751ce-129">The following table shows the properties that are required when you create the termsAndConditionsAcceptanceStatus.</span></span>

|<span data-ttu-id="751ce-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="751ce-130">Property</span></span>|<span data-ttu-id="751ce-131">Тип</span><span class="sxs-lookup"><span data-stu-id="751ce-131">Type</span></span>|<span data-ttu-id="751ce-132">Описание</span><span class="sxs-lookup"><span data-stu-id="751ce-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="751ce-133">id</span><span class="sxs-lookup"><span data-stu-id="751ce-133">id</span></span>|<span data-ttu-id="751ce-134">Строка</span><span class="sxs-lookup"><span data-stu-id="751ce-134">String</span></span>|<span data-ttu-id="751ce-135">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="751ce-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="751ce-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="751ce-136">userDisplayName</span></span>|<span data-ttu-id="751ce-137">String</span><span class="sxs-lookup"><span data-stu-id="751ce-137">String</span></span>|<span data-ttu-id="751ce-138">Отображает имя пользователя, чье принятие представлено объектом.</span><span class="sxs-lookup"><span data-stu-id="751ce-138">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="751ce-139">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="751ce-139">acceptedVersion</span></span>|<span data-ttu-id="751ce-140">Int32</span><span class="sxs-lookup"><span data-stu-id="751ce-140">Int32</span></span>|<span data-ttu-id="751ce-141">Номер последней версии условий, принятых пользователем.</span><span class="sxs-lookup"><span data-stu-id="751ce-141">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="751ce-142">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="751ce-142">acceptedDateTime</span></span>|<span data-ttu-id="751ce-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="751ce-143">DateTimeOffset</span></span>|<span data-ttu-id="751ce-144">Дата и время последнего принятия условий пользователем.</span><span class="sxs-lookup"><span data-stu-id="751ce-144">DateTime when the terms were last accepted by the user.</span></span>|
|<span data-ttu-id="751ce-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="751ce-145">userPrincipalName</span></span>|<span data-ttu-id="751ce-146">String</span><span class="sxs-lookup"><span data-stu-id="751ce-146">String</span></span>|<span data-ttu-id="751ce-147">UserPrincipalName пользователя, который принял этот термин.</span><span class="sxs-lookup"><span data-stu-id="751ce-147">The userPrincipalName of the User that accepted the term.</span></span>|



## <a name="response"></a><span data-ttu-id="751ce-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="751ce-148">Response</span></span>
<span data-ttu-id="751ce-149">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="751ce-149">If successful, this method returns a `201 Created` response code and a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="751ce-150">Пример</span><span class="sxs-lookup"><span data-stu-id="751ce-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="751ce-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="751ce-151">Request</span></span>
<span data-ttu-id="751ce-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="751ce-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
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

### <a name="response"></a><span data-ttu-id="751ce-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="751ce-153">Response</span></span>
<span data-ttu-id="751ce-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="751ce-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




