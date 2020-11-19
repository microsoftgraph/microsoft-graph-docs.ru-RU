---
title: Обновление объекта termsAndConditionsAcceptanceStatus
description: Обновление свойств объекта termsAndConditionsAcceptanceStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3f94b8b5f4c9011c01f55899977f04a400824755
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49243816"
---
# <a name="update-termsandconditionsacceptancestatus"></a><span data-ttu-id="dca81-103">Обновление объекта termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="dca81-103">Update termsAndConditionsAcceptanceStatus</span></span>

<span data-ttu-id="dca81-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dca81-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dca81-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dca81-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dca81-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dca81-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dca81-107">Обновление свойств объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="dca81-107">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dca81-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="dca81-108">Prerequisites</span></span>
<span data-ttu-id="dca81-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dca81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dca81-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dca81-111">Permission type</span></span>|<span data-ttu-id="dca81-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dca81-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dca81-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dca81-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dca81-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dca81-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="dca81-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dca81-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dca81-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dca81-116">Not supported.</span></span>|
|<span data-ttu-id="dca81-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="dca81-117">Application</span></span>|<span data-ttu-id="dca81-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dca81-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dca81-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dca81-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="dca81-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="dca81-120">Request headers</span></span>
|<span data-ttu-id="dca81-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dca81-121">Header</span></span>|<span data-ttu-id="dca81-122">Значение</span><span class="sxs-lookup"><span data-stu-id="dca81-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dca81-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dca81-123">Authorization</span></span>|<span data-ttu-id="dca81-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dca81-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dca81-125">Accept</span><span class="sxs-lookup"><span data-stu-id="dca81-125">Accept</span></span>|<span data-ttu-id="dca81-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dca81-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dca81-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dca81-127">Request body</span></span>
<span data-ttu-id="dca81-128">В тексте запроса добавьте представление объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dca81-128">In the request body, supply a JSON representation for the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

<span data-ttu-id="dca81-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="dca81-129">The following table shows the properties that are required when you create the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span></span>

|<span data-ttu-id="dca81-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="dca81-130">Property</span></span>|<span data-ttu-id="dca81-131">Тип</span><span class="sxs-lookup"><span data-stu-id="dca81-131">Type</span></span>|<span data-ttu-id="dca81-132">Описание</span><span class="sxs-lookup"><span data-stu-id="dca81-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dca81-133">id</span><span class="sxs-lookup"><span data-stu-id="dca81-133">id</span></span>|<span data-ttu-id="dca81-134">String</span><span class="sxs-lookup"><span data-stu-id="dca81-134">String</span></span>|<span data-ttu-id="dca81-135">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="dca81-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="dca81-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="dca81-136">userDisplayName</span></span>|<span data-ttu-id="dca81-137">String</span><span class="sxs-lookup"><span data-stu-id="dca81-137">String</span></span>|<span data-ttu-id="dca81-138">Отображает имя пользователя, чье принятие представлено объектом.</span><span class="sxs-lookup"><span data-stu-id="dca81-138">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="dca81-139">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="dca81-139">acceptedVersion</span></span>|<span data-ttu-id="dca81-140">Int32</span><span class="sxs-lookup"><span data-stu-id="dca81-140">Int32</span></span>|<span data-ttu-id="dca81-141">Номер последней версии условий, принятых пользователем.</span><span class="sxs-lookup"><span data-stu-id="dca81-141">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="dca81-142">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="dca81-142">acceptedDateTime</span></span>|<span data-ttu-id="dca81-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dca81-143">DateTimeOffset</span></span>|<span data-ttu-id="dca81-144">Дата и время последнего принятия условий пользователем.</span><span class="sxs-lookup"><span data-stu-id="dca81-144">DateTime when the terms were last accepted by the user.</span></span>|
|<span data-ttu-id="dca81-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="dca81-145">userPrincipalName</span></span>|<span data-ttu-id="dca81-146">String</span><span class="sxs-lookup"><span data-stu-id="dca81-146">String</span></span>|<span data-ttu-id="dca81-147">UserPrincipalName пользователя, который принял термин.</span><span class="sxs-lookup"><span data-stu-id="dca81-147">The userPrincipalName of the User that accepted the term.</span></span>|



## <a name="response"></a><span data-ttu-id="dca81-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="dca81-148">Response</span></span>
<span data-ttu-id="dca81-149">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dca81-149">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dca81-150">Пример</span><span class="sxs-lookup"><span data-stu-id="dca81-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="dca81-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="dca81-151">Request</span></span>
<span data-ttu-id="dca81-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dca81-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
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

### <a name="response"></a><span data-ttu-id="dca81-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="dca81-153">Response</span></span>
<span data-ttu-id="dca81-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dca81-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




