---
title: Обновление объекта telecomExpenseManagementPartner
description: Обновление свойств объекта telecomExpenseManagementPartner.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9444a5529bb5aebc60de25d1876e6302969fc94e
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37361198"
---
# <a name="update-telecomexpensemanagementpartner"></a><span data-ttu-id="e46b4-103">Обновление объекта telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="e46b4-103">Update telecomExpenseManagementPartner</span></span>

> <span data-ttu-id="e46b4-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e46b4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e46b4-105">Обновление свойств объекта [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="e46b4-105">Update the properties of a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e46b4-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e46b4-106">Prerequisites</span></span>
<span data-ttu-id="e46b4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e46b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e46b4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e46b4-109">Permission type</span></span>|<span data-ttu-id="e46b4-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e46b4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e46b4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e46b4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e46b4-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e46b4-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e46b4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e46b4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e46b4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e46b4-114">Not supported.</span></span>|
|<span data-ttu-id="e46b4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e46b4-115">Application</span></span>|<span data-ttu-id="e46b4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e46b4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e46b4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e46b4-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="e46b4-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e46b4-118">Request headers</span></span>
|<span data-ttu-id="e46b4-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e46b4-119">Header</span></span>|<span data-ttu-id="e46b4-120">Значение</span><span class="sxs-lookup"><span data-stu-id="e46b4-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e46b4-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e46b4-121">Authorization</span></span>|<span data-ttu-id="e46b4-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e46b4-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e46b4-123">Accept</span><span class="sxs-lookup"><span data-stu-id="e46b4-123">Accept</span></span>|<span data-ttu-id="e46b4-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e46b4-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e46b4-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e46b4-125">Request body</span></span>
<span data-ttu-id="e46b4-126">В теле запроса добавьте представление объекта [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e46b4-126">In the request body, supply a JSON representation for the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

<span data-ttu-id="e46b4-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="e46b4-127">The following table shows the properties that are required when you create the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span></span>

|<span data-ttu-id="e46b4-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="e46b4-128">Property</span></span>|<span data-ttu-id="e46b4-129">Тип</span><span class="sxs-lookup"><span data-stu-id="e46b4-129">Type</span></span>|<span data-ttu-id="e46b4-130">Описание</span><span class="sxs-lookup"><span data-stu-id="e46b4-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e46b4-131">id</span><span class="sxs-lookup"><span data-stu-id="e46b4-131">id</span></span>|<span data-ttu-id="e46b4-132">String</span><span class="sxs-lookup"><span data-stu-id="e46b4-132">String</span></span>|<span data-ttu-id="e46b4-133">Уникальный идентификатор партнера TEM.</span><span class="sxs-lookup"><span data-stu-id="e46b4-133">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="e46b4-134">displayName</span><span class="sxs-lookup"><span data-stu-id="e46b4-134">displayName</span></span>|<span data-ttu-id="e46b4-135">Строка</span><span class="sxs-lookup"><span data-stu-id="e46b4-135">String</span></span>|<span data-ttu-id="e46b4-136">Отображаемое имя партнера TEM.</span><span class="sxs-lookup"><span data-stu-id="e46b4-136">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="e46b4-137">url</span><span class="sxs-lookup"><span data-stu-id="e46b4-137">url</span></span>|<span data-ttu-id="e46b4-138">String</span><span class="sxs-lookup"><span data-stu-id="e46b4-138">String</span></span>|<span data-ttu-id="e46b4-139">URL-адрес административной панели управления партнера TEM, где администратор может настроить службу TEM.</span><span class="sxs-lookup"><span data-stu-id="e46b4-139">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="e46b4-140">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="e46b4-140">appAuthorized</span></span>|<span data-ttu-id="e46b4-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="e46b4-141">Boolean</span></span>|<span data-ttu-id="e46b4-142">Определяет, разрешен ли доступ к Intune партнерскому приложению AAD.</span><span class="sxs-lookup"><span data-stu-id="e46b4-142">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="e46b4-143">enabled</span><span class="sxs-lookup"><span data-stu-id="e46b4-143">enabled</span></span>|<span data-ttu-id="e46b4-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="e46b4-144">Boolean</span></span>|<span data-ttu-id="e46b4-145">Определяет, включено или отключено сейчас подключение Intune к службе TEM.</span><span class="sxs-lookup"><span data-stu-id="e46b4-145">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="e46b4-146">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="e46b4-146">lastConnectionDateTime</span></span>|<span data-ttu-id="e46b4-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e46b4-147">DateTimeOffset</span></span>|<span data-ttu-id="e46b4-148">Метка времени последнего запроса, отправленного в службу Intune партнером TEM.</span><span class="sxs-lookup"><span data-stu-id="e46b4-148">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="e46b4-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="e46b4-149">Response</span></span>
<span data-ttu-id="e46b4-150">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e46b4-150">If successful, this method returns a `200 OK` response code and an updated [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e46b4-151">Пример</span><span class="sxs-lookup"><span data-stu-id="e46b4-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="e46b4-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="e46b4-152">Request</span></span>
<span data-ttu-id="e46b4-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e46b4-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e46b4-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="e46b4-154">Response</span></span>
<span data-ttu-id="e46b4-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e46b4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




