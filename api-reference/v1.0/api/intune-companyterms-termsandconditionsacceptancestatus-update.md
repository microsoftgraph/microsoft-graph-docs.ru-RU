---
title: Обновление объекта termsAndConditionsAcceptanceStatus
description: Обновление свойств объекта termsAndConditionsAcceptanceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e6cbb67f852a89322cae6455b13d97b80872bbf9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32580230"
---
# <a name="update-termsandconditionsacceptancestatus"></a><span data-ttu-id="ec000-103">Обновление объекта termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="ec000-103">Update termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="ec000-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ec000-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec000-105">Обновление свойств объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="ec000-105">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ec000-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ec000-106">Prerequisites</span></span>
<span data-ttu-id="ec000-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec000-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec000-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ec000-109">Permission type</span></span>|<span data-ttu-id="ec000-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ec000-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec000-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ec000-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ec000-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec000-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ec000-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ec000-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec000-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec000-114">Not supported.</span></span>|
|<span data-ttu-id="ec000-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ec000-115">Application</span></span>|<span data-ttu-id="ec000-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec000-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec000-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ec000-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="ec000-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ec000-118">Request headers</span></span>
|<span data-ttu-id="ec000-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ec000-119">Header</span></span>|<span data-ttu-id="ec000-120">Значение</span><span class="sxs-lookup"><span data-stu-id="ec000-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ec000-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ec000-121">Authorization</span></span>|<span data-ttu-id="ec000-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ec000-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ec000-123">Accept</span><span class="sxs-lookup"><span data-stu-id="ec000-123">Accept</span></span>|<span data-ttu-id="ec000-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ec000-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec000-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ec000-125">Request body</span></span>
<span data-ttu-id="ec000-126">В тексте запроса добавьте представление объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ec000-126">In the request body, supply a JSON representation for the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

<span data-ttu-id="ec000-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="ec000-127">The following table shows the properties that are required when you create the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span></span>

|<span data-ttu-id="ec000-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="ec000-128">Property</span></span>|<span data-ttu-id="ec000-129">Тип</span><span class="sxs-lookup"><span data-stu-id="ec000-129">Type</span></span>|<span data-ttu-id="ec000-130">Описание</span><span class="sxs-lookup"><span data-stu-id="ec000-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec000-131">id</span><span class="sxs-lookup"><span data-stu-id="ec000-131">id</span></span>|<span data-ttu-id="ec000-132">String</span><span class="sxs-lookup"><span data-stu-id="ec000-132">String</span></span>|<span data-ttu-id="ec000-133">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="ec000-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="ec000-134">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="ec000-134">userDisplayName</span></span>|<span data-ttu-id="ec000-135">String</span><span class="sxs-lookup"><span data-stu-id="ec000-135">String</span></span>|<span data-ttu-id="ec000-136">Отображает имя пользователя, чье принятие представлено объектом.</span><span class="sxs-lookup"><span data-stu-id="ec000-136">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="ec000-137">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="ec000-137">acceptedVersion</span></span>|<span data-ttu-id="ec000-138">Int32</span><span class="sxs-lookup"><span data-stu-id="ec000-138">Int32</span></span>|<span data-ttu-id="ec000-139">Номер последней версии условий, принятых пользователем.</span><span class="sxs-lookup"><span data-stu-id="ec000-139">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="ec000-140">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="ec000-140">acceptedDateTime</span></span>|<span data-ttu-id="ec000-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec000-141">DateTimeOffset</span></span>|<span data-ttu-id="ec000-142">Дата и время последнего принятия условий пользователем.</span><span class="sxs-lookup"><span data-stu-id="ec000-142">DateTime when the terms were last accepted by the user.</span></span>|



## <a name="response"></a><span data-ttu-id="ec000-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec000-143">Response</span></span>
<span data-ttu-id="ec000-144">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ec000-144">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec000-145">Пример</span><span class="sxs-lookup"><span data-stu-id="ec000-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="ec000-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="ec000-146">Request</span></span>
<span data-ttu-id="ec000-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ec000-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ec000-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec000-148">Response</span></span>
<span data-ttu-id="ec000-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ec000-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



