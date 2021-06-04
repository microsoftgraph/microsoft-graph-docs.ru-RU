---
title: Обновление объекта telecomExpenseManagementPartner
description: Обновление свойств объекта telecomExpenseManagementPartner.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 52280b8ebc9ffa6c82fce8e630737034f6c862e6
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52743086"
---
# <a name="update-telecomexpensemanagementpartner"></a><span data-ttu-id="0d44f-103">Обновление объекта telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="0d44f-103">Update telecomExpenseManagementPartner</span></span>

<span data-ttu-id="0d44f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d44f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0d44f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0d44f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d44f-106">Обновление свойств объекта [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="0d44f-106">Update the properties of a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0d44f-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0d44f-107">Prerequisites</span></span>
<span data-ttu-id="0d44f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d44f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d44f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0d44f-110">Permission type</span></span>|<span data-ttu-id="0d44f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0d44f-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d44f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0d44f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0d44f-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d44f-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0d44f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0d44f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d44f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d44f-115">Not supported.</span></span>|
|<span data-ttu-id="0d44f-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="0d44f-116">Application</span></span>|<span data-ttu-id="0d44f-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d44f-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d44f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0d44f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="0d44f-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0d44f-119">Request headers</span></span>
|<span data-ttu-id="0d44f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0d44f-120">Header</span></span>|<span data-ttu-id="0d44f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0d44f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d44f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d44f-122">Authorization</span></span>|<span data-ttu-id="0d44f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0d44f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d44f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0d44f-124">Accept</span></span>|<span data-ttu-id="0d44f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0d44f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d44f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0d44f-126">Request body</span></span>
<span data-ttu-id="0d44f-127">В теле запроса добавьте представление объекта [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0d44f-127">In the request body, supply a JSON representation for the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

<span data-ttu-id="0d44f-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="0d44f-128">The following table shows the properties that are required when you create the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span></span>

|<span data-ttu-id="0d44f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="0d44f-129">Property</span></span>|<span data-ttu-id="0d44f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0d44f-130">Type</span></span>|<span data-ttu-id="0d44f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0d44f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d44f-132">id</span><span class="sxs-lookup"><span data-stu-id="0d44f-132">id</span></span>|<span data-ttu-id="0d44f-133">String</span><span class="sxs-lookup"><span data-stu-id="0d44f-133">String</span></span>|<span data-ttu-id="0d44f-134">Уникальный идентификатор партнера TEM.</span><span class="sxs-lookup"><span data-stu-id="0d44f-134">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="0d44f-135">displayName</span><span class="sxs-lookup"><span data-stu-id="0d44f-135">displayName</span></span>|<span data-ttu-id="0d44f-136">String</span><span class="sxs-lookup"><span data-stu-id="0d44f-136">String</span></span>|<span data-ttu-id="0d44f-137">Отображаемое имя партнера TEM.</span><span class="sxs-lookup"><span data-stu-id="0d44f-137">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="0d44f-138">url</span><span class="sxs-lookup"><span data-stu-id="0d44f-138">url</span></span>|<span data-ttu-id="0d44f-139">String</span><span class="sxs-lookup"><span data-stu-id="0d44f-139">String</span></span>|<span data-ttu-id="0d44f-140">URL-адрес административной панели управления партнера TEM, где администратор может настроить службу TEM.</span><span class="sxs-lookup"><span data-stu-id="0d44f-140">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="0d44f-141">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="0d44f-141">appAuthorized</span></span>|<span data-ttu-id="0d44f-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="0d44f-142">Boolean</span></span>|<span data-ttu-id="0d44f-143">Определяет, разрешен ли доступ к Intune партнерскому приложению AAD.</span><span class="sxs-lookup"><span data-stu-id="0d44f-143">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="0d44f-144">enabled</span><span class="sxs-lookup"><span data-stu-id="0d44f-144">enabled</span></span>|<span data-ttu-id="0d44f-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="0d44f-145">Boolean</span></span>|<span data-ttu-id="0d44f-146">Определяет, включено или отключено сейчас подключение Intune к службе TEM.</span><span class="sxs-lookup"><span data-stu-id="0d44f-146">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="0d44f-147">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="0d44f-147">lastConnectionDateTime</span></span>|<span data-ttu-id="0d44f-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d44f-148">DateTimeOffset</span></span>|<span data-ttu-id="0d44f-149">Метка времени последнего запроса, отправленного в службу Intune партнером TEM.</span><span class="sxs-lookup"><span data-stu-id="0d44f-149">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="0d44f-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d44f-150">Response</span></span>
<span data-ttu-id="0d44f-151">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0d44f-151">If successful, this method returns a `200 OK` response code and an updated [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d44f-152">Пример</span><span class="sxs-lookup"><span data-stu-id="0d44f-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="0d44f-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d44f-153">Request</span></span>
<span data-ttu-id="0d44f-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0d44f-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0d44f-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d44f-155">Response</span></span>
<span data-ttu-id="0d44f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0d44f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




