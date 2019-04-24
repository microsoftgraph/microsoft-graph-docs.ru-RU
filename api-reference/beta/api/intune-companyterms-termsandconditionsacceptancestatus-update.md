---
title: Обновление объекта termsAndConditionsAcceptanceStatus
description: Обновление свойств объекта termsAndConditionsAcceptanceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 726257a07a268bb2475e84d545a8c63b21c40431
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32482664"
---
# <a name="update-termsandconditionsacceptancestatus"></a><span data-ttu-id="17490-103">Обновление объекта termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="17490-103">Update termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="17490-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17490-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="17490-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="17490-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17490-106">Обновление свойств объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="17490-106">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="17490-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="17490-107">Prerequisites</span></span>
<span data-ttu-id="17490-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17490-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17490-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="17490-110">Permission type</span></span>|<span data-ttu-id="17490-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="17490-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17490-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="17490-112">Delegated (work or school account)</span></span>|<span data-ttu-id="17490-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17490-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="17490-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="17490-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17490-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17490-115">Not supported.</span></span>|
|<span data-ttu-id="17490-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="17490-116">Application</span></span>|<span data-ttu-id="17490-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17490-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="17490-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="17490-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="17490-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="17490-119">Request headers</span></span>
|<span data-ttu-id="17490-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="17490-120">Header</span></span>|<span data-ttu-id="17490-121">Значение</span><span class="sxs-lookup"><span data-stu-id="17490-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17490-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="17490-122">Authorization</span></span>|<span data-ttu-id="17490-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="17490-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17490-124">Accept</span><span class="sxs-lookup"><span data-stu-id="17490-124">Accept</span></span>|<span data-ttu-id="17490-125">application/json</span><span class="sxs-lookup"><span data-stu-id="17490-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17490-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="17490-126">Request body</span></span>
<span data-ttu-id="17490-127">В тексте запроса добавьте представление объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="17490-127">In the request body, supply a JSON representation for the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

<span data-ttu-id="17490-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="17490-128">The following table shows the properties that are required when you create the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span></span>

|<span data-ttu-id="17490-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="17490-129">Property</span></span>|<span data-ttu-id="17490-130">Тип</span><span class="sxs-lookup"><span data-stu-id="17490-130">Type</span></span>|<span data-ttu-id="17490-131">Описание</span><span class="sxs-lookup"><span data-stu-id="17490-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17490-132">id</span><span class="sxs-lookup"><span data-stu-id="17490-132">id</span></span>|<span data-ttu-id="17490-133">String</span><span class="sxs-lookup"><span data-stu-id="17490-133">String</span></span>|<span data-ttu-id="17490-134">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="17490-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="17490-135">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="17490-135">userDisplayName</span></span>|<span data-ttu-id="17490-136">String</span><span class="sxs-lookup"><span data-stu-id="17490-136">String</span></span>|<span data-ttu-id="17490-137">Отображает имя пользователя, чье принятие представлено объектом.</span><span class="sxs-lookup"><span data-stu-id="17490-137">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="17490-138">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="17490-138">acceptedVersion</span></span>|<span data-ttu-id="17490-139">Int32</span><span class="sxs-lookup"><span data-stu-id="17490-139">Int32</span></span>|<span data-ttu-id="17490-140">Номер последней версии условий, принятых пользователем.</span><span class="sxs-lookup"><span data-stu-id="17490-140">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="17490-141">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="17490-141">acceptedDateTime</span></span>|<span data-ttu-id="17490-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17490-142">DateTimeOffset</span></span>|<span data-ttu-id="17490-143">Дата и время последнего принятия условий пользователем.</span><span class="sxs-lookup"><span data-stu-id="17490-143">DateTime when the terms were last accepted by the user.</span></span>|



## <a name="response"></a><span data-ttu-id="17490-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="17490-144">Response</span></span>
<span data-ttu-id="17490-145">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="17490-145">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17490-146">Пример</span><span class="sxs-lookup"><span data-stu-id="17490-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="17490-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="17490-147">Request</span></span>
<span data-ttu-id="17490-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="17490-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="17490-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="17490-149">Response</span></span>
<span data-ttu-id="17490-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="17490-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





