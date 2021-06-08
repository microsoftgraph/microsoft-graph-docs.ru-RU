---
title: Создание telecomExpenseManagementPartner
description: Создание объекта telecomExpenseManagementPartner.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: deada7598a04b1d1de96eb586d7429a613411f32
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757874"
---
# <a name="create-telecomexpensemanagementpartner"></a><span data-ttu-id="ab88c-103">Создание telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="ab88c-103">Create telecomExpenseManagementPartner</span></span>

<span data-ttu-id="ab88c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab88c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ab88c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ab88c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab88c-106">Создание объекта [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="ab88c-106">Create a new [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ab88c-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ab88c-107">Prerequisites</span></span>
<span data-ttu-id="ab88c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab88c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab88c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ab88c-110">Permission type</span></span>|<span data-ttu-id="ab88c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ab88c-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab88c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ab88c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ab88c-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab88c-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ab88c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ab88c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab88c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab88c-115">Not supported.</span></span>|
|<span data-ttu-id="ab88c-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="ab88c-116">Application</span></span>|<span data-ttu-id="ab88c-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab88c-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab88c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ab88c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/telecomExpenseManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="ab88c-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ab88c-119">Request headers</span></span>
|<span data-ttu-id="ab88c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ab88c-120">Header</span></span>|<span data-ttu-id="ab88c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ab88c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab88c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab88c-122">Authorization</span></span>|<span data-ttu-id="ab88c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ab88c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ab88c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ab88c-124">Accept</span></span>|<span data-ttu-id="ab88c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ab88c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab88c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ab88c-126">Request body</span></span>
<span data-ttu-id="ab88c-127">В теле запроса добавьте представление объекта telecomExpenseManagementPartner в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ab88c-127">In the request body, supply a JSON representation for the telecomExpenseManagementPartner object.</span></span>

<span data-ttu-id="ab88c-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта telecomExpenseManagementPartner.</span><span class="sxs-lookup"><span data-stu-id="ab88c-128">The following table shows the properties that are required when you create the telecomExpenseManagementPartner.</span></span>

|<span data-ttu-id="ab88c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ab88c-129">Property</span></span>|<span data-ttu-id="ab88c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ab88c-130">Type</span></span>|<span data-ttu-id="ab88c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ab88c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab88c-132">id</span><span class="sxs-lookup"><span data-stu-id="ab88c-132">id</span></span>|<span data-ttu-id="ab88c-133">String</span><span class="sxs-lookup"><span data-stu-id="ab88c-133">String</span></span>|<span data-ttu-id="ab88c-134">Уникальный идентификатор партнера TEM.</span><span class="sxs-lookup"><span data-stu-id="ab88c-134">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="ab88c-135">displayName</span><span class="sxs-lookup"><span data-stu-id="ab88c-135">displayName</span></span>|<span data-ttu-id="ab88c-136">String</span><span class="sxs-lookup"><span data-stu-id="ab88c-136">String</span></span>|<span data-ttu-id="ab88c-137">Отображаемое имя партнера TEM.</span><span class="sxs-lookup"><span data-stu-id="ab88c-137">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="ab88c-138">url</span><span class="sxs-lookup"><span data-stu-id="ab88c-138">url</span></span>|<span data-ttu-id="ab88c-139">String</span><span class="sxs-lookup"><span data-stu-id="ab88c-139">String</span></span>|<span data-ttu-id="ab88c-140">URL-адрес административной панели управления партнера TEM, где администратор может настроить службу TEM.</span><span class="sxs-lookup"><span data-stu-id="ab88c-140">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="ab88c-141">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="ab88c-141">appAuthorized</span></span>|<span data-ttu-id="ab88c-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab88c-142">Boolean</span></span>|<span data-ttu-id="ab88c-143">Определяет, разрешен ли доступ к Intune партнерскому приложению AAD.</span><span class="sxs-lookup"><span data-stu-id="ab88c-143">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="ab88c-144">enabled</span><span class="sxs-lookup"><span data-stu-id="ab88c-144">enabled</span></span>|<span data-ttu-id="ab88c-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab88c-145">Boolean</span></span>|<span data-ttu-id="ab88c-146">Определяет, включено или отключено сейчас подключение Intune к службе TEM.</span><span class="sxs-lookup"><span data-stu-id="ab88c-146">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="ab88c-147">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="ab88c-147">lastConnectionDateTime</span></span>|<span data-ttu-id="ab88c-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab88c-148">DateTimeOffset</span></span>|<span data-ttu-id="ab88c-149">Метка времени последнего запроса, отправленного в службу Intune партнером TEM.</span><span class="sxs-lookup"><span data-stu-id="ab88c-149">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="ab88c-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab88c-150">Response</span></span>
<span data-ttu-id="ab88c-151">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ab88c-151">If successful, this method returns a `201 Created` response code and a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab88c-152">Пример</span><span class="sxs-lookup"><span data-stu-id="ab88c-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="ab88c-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="ab88c-153">Request</span></span>
<span data-ttu-id="ab88c-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ab88c-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/telecomExpenseManagementPartners
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

### <a name="response"></a><span data-ttu-id="ab88c-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab88c-155">Response</span></span>
<span data-ttu-id="ab88c-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ab88c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




