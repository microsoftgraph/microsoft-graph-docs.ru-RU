---
title: Обновление объекта telecomExpenseManagementPartner
description: Обновление свойств объекта telecomExpenseManagementPartner.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c9d3f218f17edfdea700059cbe8aed4e327d7cbc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48082177"
---
# <a name="update-telecomexpensemanagementpartner"></a><span data-ttu-id="cbdeb-103">Обновление объекта telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="cbdeb-103">Update telecomExpenseManagementPartner</span></span>

<span data-ttu-id="cbdeb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cbdeb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cbdeb-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cbdeb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cbdeb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cbdeb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cbdeb-107">Обновление свойств объекта [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="cbdeb-107">Update the properties of a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cbdeb-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="cbdeb-108">Prerequisites</span></span>
<span data-ttu-id="cbdeb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cbdeb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbdeb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cbdeb-111">Permission type</span></span>|<span data-ttu-id="cbdeb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cbdeb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cbdeb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cbdeb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cbdeb-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbdeb-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="cbdeb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cbdeb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cbdeb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cbdeb-116">Not supported.</span></span>|
|<span data-ttu-id="cbdeb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cbdeb-117">Application</span></span>|<span data-ttu-id="cbdeb-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbdeb-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cbdeb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cbdeb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="cbdeb-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cbdeb-120">Request headers</span></span>
|<span data-ttu-id="cbdeb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cbdeb-121">Header</span></span>|<span data-ttu-id="cbdeb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cbdeb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cbdeb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cbdeb-123">Authorization</span></span>|<span data-ttu-id="cbdeb-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cbdeb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cbdeb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cbdeb-125">Accept</span></span>|<span data-ttu-id="cbdeb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cbdeb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cbdeb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cbdeb-127">Request body</span></span>
<span data-ttu-id="cbdeb-128">В теле запроса добавьте представление объекта [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cbdeb-128">In the request body, supply a JSON representation for the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

<span data-ttu-id="cbdeb-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="cbdeb-129">The following table shows the properties that are required when you create the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span></span>

|<span data-ttu-id="cbdeb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="cbdeb-130">Property</span></span>|<span data-ttu-id="cbdeb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="cbdeb-131">Type</span></span>|<span data-ttu-id="cbdeb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="cbdeb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cbdeb-133">id</span><span class="sxs-lookup"><span data-stu-id="cbdeb-133">id</span></span>|<span data-ttu-id="cbdeb-134">Строка</span><span class="sxs-lookup"><span data-stu-id="cbdeb-134">String</span></span>|<span data-ttu-id="cbdeb-135">Уникальный идентификатор партнера TEM.</span><span class="sxs-lookup"><span data-stu-id="cbdeb-135">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="cbdeb-136">displayName</span><span class="sxs-lookup"><span data-stu-id="cbdeb-136">displayName</span></span>|<span data-ttu-id="cbdeb-137">Строка</span><span class="sxs-lookup"><span data-stu-id="cbdeb-137">String</span></span>|<span data-ttu-id="cbdeb-138">Отображаемое имя партнера TEM.</span><span class="sxs-lookup"><span data-stu-id="cbdeb-138">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="cbdeb-139">url</span><span class="sxs-lookup"><span data-stu-id="cbdeb-139">url</span></span>|<span data-ttu-id="cbdeb-140">String</span><span class="sxs-lookup"><span data-stu-id="cbdeb-140">String</span></span>|<span data-ttu-id="cbdeb-141">URL-адрес административной панели управления партнера TEM, где администратор может настроить службу TEM.</span><span class="sxs-lookup"><span data-stu-id="cbdeb-141">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="cbdeb-142">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="cbdeb-142">appAuthorized</span></span>|<span data-ttu-id="cbdeb-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="cbdeb-143">Boolean</span></span>|<span data-ttu-id="cbdeb-144">Определяет, разрешен ли доступ к Intune партнерскому приложению AAD.</span><span class="sxs-lookup"><span data-stu-id="cbdeb-144">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="cbdeb-145">enabled</span><span class="sxs-lookup"><span data-stu-id="cbdeb-145">enabled</span></span>|<span data-ttu-id="cbdeb-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="cbdeb-146">Boolean</span></span>|<span data-ttu-id="cbdeb-147">Определяет, включено или отключено сейчас подключение Intune к службе TEM.</span><span class="sxs-lookup"><span data-stu-id="cbdeb-147">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="cbdeb-148">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="cbdeb-148">lastConnectionDateTime</span></span>|<span data-ttu-id="cbdeb-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cbdeb-149">DateTimeOffset</span></span>|<span data-ttu-id="cbdeb-150">Метка времени последнего запроса, отправленного в службу Intune партнером TEM.</span><span class="sxs-lookup"><span data-stu-id="cbdeb-150">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="cbdeb-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="cbdeb-151">Response</span></span>
<span data-ttu-id="cbdeb-152">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="cbdeb-152">If successful, this method returns a `200 OK` response code and an updated [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cbdeb-153">Пример</span><span class="sxs-lookup"><span data-stu-id="cbdeb-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="cbdeb-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="cbdeb-154">Request</span></span>
<span data-ttu-id="cbdeb-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cbdeb-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
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

### <a name="response"></a><span data-ttu-id="cbdeb-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="cbdeb-156">Response</span></span>
<span data-ttu-id="cbdeb-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cbdeb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






