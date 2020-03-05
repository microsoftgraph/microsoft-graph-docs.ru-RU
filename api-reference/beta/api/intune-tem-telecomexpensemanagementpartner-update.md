---
title: Обновление объекта telecomExpenseManagementPartner
description: Обновление свойств объекта telecomExpenseManagementPartner.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c4829cddf4faccd8af34f46e5614047c4225b202
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42457771"
---
# <a name="update-telecomexpensemanagementpartner"></a><span data-ttu-id="353ff-103">Обновление объекта telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="353ff-103">Update telecomExpenseManagementPartner</span></span>

<span data-ttu-id="353ff-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="353ff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="353ff-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="353ff-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="353ff-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="353ff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="353ff-107">Обновление свойств объекта [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="353ff-107">Update the properties of a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="353ff-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="353ff-108">Prerequisites</span></span>
<span data-ttu-id="353ff-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="353ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="353ff-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="353ff-111">Permission type</span></span>|<span data-ttu-id="353ff-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="353ff-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="353ff-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="353ff-113">Delegated (work or school account)</span></span>|<span data-ttu-id="353ff-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="353ff-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="353ff-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="353ff-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="353ff-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="353ff-116">Not supported.</span></span>|
|<span data-ttu-id="353ff-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="353ff-117">Application</span></span>|<span data-ttu-id="353ff-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="353ff-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="353ff-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="353ff-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="353ff-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="353ff-120">Request headers</span></span>
|<span data-ttu-id="353ff-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="353ff-121">Header</span></span>|<span data-ttu-id="353ff-122">Значение</span><span class="sxs-lookup"><span data-stu-id="353ff-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="353ff-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="353ff-123">Authorization</span></span>|<span data-ttu-id="353ff-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="353ff-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="353ff-125">Accept</span><span class="sxs-lookup"><span data-stu-id="353ff-125">Accept</span></span>|<span data-ttu-id="353ff-126">application/json</span><span class="sxs-lookup"><span data-stu-id="353ff-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="353ff-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="353ff-127">Request body</span></span>
<span data-ttu-id="353ff-128">В теле запроса добавьте представление объекта [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="353ff-128">In the request body, supply a JSON representation for the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

<span data-ttu-id="353ff-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="353ff-129">The following table shows the properties that are required when you create the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span></span>

|<span data-ttu-id="353ff-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="353ff-130">Property</span></span>|<span data-ttu-id="353ff-131">Тип</span><span class="sxs-lookup"><span data-stu-id="353ff-131">Type</span></span>|<span data-ttu-id="353ff-132">Описание</span><span class="sxs-lookup"><span data-stu-id="353ff-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="353ff-133">id</span><span class="sxs-lookup"><span data-stu-id="353ff-133">id</span></span>|<span data-ttu-id="353ff-134">String</span><span class="sxs-lookup"><span data-stu-id="353ff-134">String</span></span>|<span data-ttu-id="353ff-135">Уникальный идентификатор партнера TEM.</span><span class="sxs-lookup"><span data-stu-id="353ff-135">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="353ff-136">displayName</span><span class="sxs-lookup"><span data-stu-id="353ff-136">displayName</span></span>|<span data-ttu-id="353ff-137">Строка</span><span class="sxs-lookup"><span data-stu-id="353ff-137">String</span></span>|<span data-ttu-id="353ff-138">Отображаемое имя партнера TEM.</span><span class="sxs-lookup"><span data-stu-id="353ff-138">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="353ff-139">url</span><span class="sxs-lookup"><span data-stu-id="353ff-139">url</span></span>|<span data-ttu-id="353ff-140">String</span><span class="sxs-lookup"><span data-stu-id="353ff-140">String</span></span>|<span data-ttu-id="353ff-141">URL-адрес административной панели управления партнера TEM, где администратор может настроить службу TEM.</span><span class="sxs-lookup"><span data-stu-id="353ff-141">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="353ff-142">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="353ff-142">appAuthorized</span></span>|<span data-ttu-id="353ff-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="353ff-143">Boolean</span></span>|<span data-ttu-id="353ff-144">Определяет, разрешен ли доступ к Intune партнерскому приложению AAD.</span><span class="sxs-lookup"><span data-stu-id="353ff-144">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="353ff-145">enabled</span><span class="sxs-lookup"><span data-stu-id="353ff-145">enabled</span></span>|<span data-ttu-id="353ff-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="353ff-146">Boolean</span></span>|<span data-ttu-id="353ff-147">Определяет, включено или отключено сейчас подключение Intune к службе TEM.</span><span class="sxs-lookup"><span data-stu-id="353ff-147">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="353ff-148">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="353ff-148">lastConnectionDateTime</span></span>|<span data-ttu-id="353ff-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="353ff-149">DateTimeOffset</span></span>|<span data-ttu-id="353ff-150">Метка времени последнего запроса, отправленного в службу Intune партнером TEM.</span><span class="sxs-lookup"><span data-stu-id="353ff-150">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="353ff-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="353ff-151">Response</span></span>
<span data-ttu-id="353ff-152">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="353ff-152">If successful, this method returns a `200 OK` response code and an updated [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="353ff-153">Пример</span><span class="sxs-lookup"><span data-stu-id="353ff-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="353ff-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="353ff-154">Request</span></span>
<span data-ttu-id="353ff-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="353ff-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="353ff-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="353ff-156">Response</span></span>
<span data-ttu-id="353ff-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="353ff-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





