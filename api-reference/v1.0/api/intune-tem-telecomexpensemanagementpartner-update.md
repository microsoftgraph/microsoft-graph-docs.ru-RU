---
title: Обновление объекта telecomExpenseManagementPartner
description: Обновление свойств объекта telecomExpenseManagementPartner.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a642e05ce730f1ebfb23a9b9c634555dd73b726f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511910"
---
# <a name="update-telecomexpensemanagementpartner"></a><span data-ttu-id="92166-103">Обновление объекта telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="92166-103">Update telecomExpenseManagementPartner</span></span>

<span data-ttu-id="92166-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92166-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="92166-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="92166-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92166-106">Обновление свойств объекта [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="92166-106">Update the properties of a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92166-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="92166-107">Prerequisites</span></span>
<span data-ttu-id="92166-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92166-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92166-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="92166-110">Permission type</span></span>|<span data-ttu-id="92166-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="92166-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92166-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="92166-112">Delegated (work or school account)</span></span>|<span data-ttu-id="92166-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92166-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="92166-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="92166-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92166-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92166-115">Not supported.</span></span>|
|<span data-ttu-id="92166-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="92166-116">Application</span></span>|<span data-ttu-id="92166-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92166-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="92166-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="92166-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="92166-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="92166-119">Request headers</span></span>
|<span data-ttu-id="92166-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="92166-120">Header</span></span>|<span data-ttu-id="92166-121">Значение</span><span class="sxs-lookup"><span data-stu-id="92166-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92166-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="92166-122">Authorization</span></span>|<span data-ttu-id="92166-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="92166-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92166-124">Accept</span><span class="sxs-lookup"><span data-stu-id="92166-124">Accept</span></span>|<span data-ttu-id="92166-125">application/json</span><span class="sxs-lookup"><span data-stu-id="92166-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92166-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="92166-126">Request body</span></span>
<span data-ttu-id="92166-127">В теле запроса добавьте представление объекта [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="92166-127">In the request body, supply a JSON representation for the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

<span data-ttu-id="92166-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="92166-128">The following table shows the properties that are required when you create the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span></span>

|<span data-ttu-id="92166-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="92166-129">Property</span></span>|<span data-ttu-id="92166-130">Тип</span><span class="sxs-lookup"><span data-stu-id="92166-130">Type</span></span>|<span data-ttu-id="92166-131">Описание</span><span class="sxs-lookup"><span data-stu-id="92166-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92166-132">id</span><span class="sxs-lookup"><span data-stu-id="92166-132">id</span></span>|<span data-ttu-id="92166-133">String</span><span class="sxs-lookup"><span data-stu-id="92166-133">String</span></span>|<span data-ttu-id="92166-134">Уникальный идентификатор партнера TEM.</span><span class="sxs-lookup"><span data-stu-id="92166-134">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="92166-135">displayName</span><span class="sxs-lookup"><span data-stu-id="92166-135">displayName</span></span>|<span data-ttu-id="92166-136">Строка</span><span class="sxs-lookup"><span data-stu-id="92166-136">String</span></span>|<span data-ttu-id="92166-137">Отображаемое имя партнера TEM.</span><span class="sxs-lookup"><span data-stu-id="92166-137">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="92166-138">url</span><span class="sxs-lookup"><span data-stu-id="92166-138">url</span></span>|<span data-ttu-id="92166-139">String</span><span class="sxs-lookup"><span data-stu-id="92166-139">String</span></span>|<span data-ttu-id="92166-140">URL-адрес административной панели управления партнера TEM, где администратор может настроить службу TEM.</span><span class="sxs-lookup"><span data-stu-id="92166-140">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="92166-141">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="92166-141">appAuthorized</span></span>|<span data-ttu-id="92166-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="92166-142">Boolean</span></span>|<span data-ttu-id="92166-143">Определяет, разрешен ли доступ к Intune партнерскому приложению AAD.</span><span class="sxs-lookup"><span data-stu-id="92166-143">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="92166-144">enabled</span><span class="sxs-lookup"><span data-stu-id="92166-144">enabled</span></span>|<span data-ttu-id="92166-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="92166-145">Boolean</span></span>|<span data-ttu-id="92166-146">Определяет, включено или отключено сейчас подключение Intune к службе TEM.</span><span class="sxs-lookup"><span data-stu-id="92166-146">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="92166-147">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="92166-147">lastConnectionDateTime</span></span>|<span data-ttu-id="92166-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92166-148">DateTimeOffset</span></span>|<span data-ttu-id="92166-149">Метка времени последнего запроса, отправленного в службу Intune партнером TEM.</span><span class="sxs-lookup"><span data-stu-id="92166-149">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="92166-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="92166-150">Response</span></span>
<span data-ttu-id="92166-151">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="92166-151">If successful, this method returns a `200 OK` response code and an updated [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92166-152">Пример</span><span class="sxs-lookup"><span data-stu-id="92166-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="92166-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="92166-153">Request</span></span>
<span data-ttu-id="92166-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="92166-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
Content-type: application/json
Content-length: 248

{
  "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
  "displayName": "Display Name value",
  "url": "Url value",
  "appAuthorized": true,
  "enabled": true,
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```

### <a name="response"></a><span data-ttu-id="92166-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="92166-155">Response</span></span>
<span data-ttu-id="92166-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="92166-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 297

{
  "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
  "id": "47a3b399-b399-47a3-99b3-a34799b3a347",
  "displayName": "Display Name value",
  "url": "Url value",
  "appAuthorized": true,
  "enabled": true,
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```




